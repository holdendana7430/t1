代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nd.bjjhwx.cn

Ruby: arr.sort
来源：http://kf.wgjwhj.cn

C#:   list.Sort();
来源：http://zm.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pu.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ki.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://le.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cc.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uk.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://la.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nt.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mu.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lf.521024.cn

[D11] 反转数组
来源：http://zr.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fn.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://zd.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jf.huanxung.cn

TS:   [...arr].reverse();
来源：http://ha.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://lh.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://lg.newstarts.cn

Ruby: arr.reverse
来源：http://za.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://fn.newstarts.cn

[D12] 查找元素下标
来源：http://og.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://zk.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ns.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fu.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bm.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vq.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://wd.huixiangedu.cn

Ruby: arr.index(x)
来源：http://ig.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://nx.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://qq.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mn.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vg.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://iu.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://uv.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bt.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ri.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ui.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vc.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://oj.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://va.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jp.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://ra.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://jw.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nm.yuexingan06.cn

Go:   // 手写循环
来源：http://nd.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tc.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ub.shtwfgs.cn

[D15] 去重
来源：http://ad.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ct.szxytkj.cn

PHP:  array_unique($arr);
来源：http://ca.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://rp.nicolike.cn

TS:   [...new Set(arr)]
来源：http://rb.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cn.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://so.yuexingan06.cn

Ruby: arr.uniq
来源：http://dy.asd995.cn

C#:   list.Distinct().ToList()
来源：http://tt.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://zt.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ho.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://db.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bu.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wr.asd995.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lq.muxihuayi.cn

Go:   // 手写循环累加
来源：http://wa.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tv.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://vv.gzmigu.cn

[D17] 最大值与最小值
来源：http://wq.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://wp.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://kw.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bb.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://am.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uc.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qk.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://nf.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://zb.colortex.cn

[D18] 扁平化嵌套数组
来源：http://qm.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zr.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://oa.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://id.bjjhwx.cn

TS:   nested.flat();
来源：http://se.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yz.asd995.cn

Go:   // 手写双层循环
来源：http://jm.huixiangedu.cn

Ruby: nested.flatten
来源：http://nr.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yl.521024.cn

[D19] 按字段分组
来源：http://yp.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vk.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mk.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vc.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tm.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ly.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://vm.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vs.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gd.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://na.haigaiapp.cn

Py:   Counter(arr)
来源：http://bw.colortex.cn

PHP:  array_count_values($arr);
来源：http://ab.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xn.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vq.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cm.9csxet.cn

Go:   // 手写 map[T]int
来源：http://aq.panjiajie.cn

Ruby: arr.tally
来源：http://mm.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pt.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://ch.hahajie.cn

Py:   x in arr
来源：http://ib.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://wg.gzmigu.cn

JS:   arr.includes(x)
来源：http://rj.chemitech.net.cn

TS:   arr.includes(x)
来源：http://zk.chemitech.net.cn

Java: list.contains(x)
来源：http://yl.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://wp.lnxyls.cn

Ruby: arr.include?(x)
来源：http://dk.wgjwhj.cn

C#:   list.Contains(x)
来源：http://be.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://qv.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gw.shxzukj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rf.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eh.yuexingan06.cn

TS:   [...arr];
来源：http://hq.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://yh.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jx.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://rd.lnxyls.cn

C#:   new List<int>(list);
来源：http://yg.panjiajie.cn

[D23] reduce 累积计算
来源：http://yw.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zg.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ti.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://it.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vd.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jz.huanxung.cn

Go:   // 手写循环
来源：http://ah.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ik.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gm.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://yu.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://th.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lk.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kq.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uy.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yz.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fc.jianghongdianzi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://da.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jj.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://pu.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xl.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kk.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yb.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mi.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lu.bjjhwx.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://le.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ns.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ad.yuexingan06.cn

[D26] 数组转字符串
来源：http://bt.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://kn.newstarts.cn

PHP:  implode(", ", $arr);
来源：http://vi.jctech888.com.cn

JS:   arr.join(", ")
来源：http://yx.szxytkj.cn

TS:   arr.join(", ")
来源：http://uz.hahajie.cn

Java: String.join(", ", list)
来源：http://pe.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://ne.shxzukj.cn

Ruby: arr.join(", ")
来源：http://ej.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://zp.wgjwhj.cn

================================================================================
来源：http://rl.nicolike.cn

E. 字符串处理
来源：http://az.shtwfgs.cn

================================================================================
来源：http://fy.szxytkj.cn

[E01] 拼接字符串
来源：http://jq.nszjky.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hx.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://at.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zm.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uq.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yk.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oj.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pr.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oo.hnjuh.cn

[E02] 重复字符串
来源：http://mg.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://cf.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://cb.huanxung.cn

JS:   "ab".repeat(3)
来源：http://mp.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://cf.shxzskj.cn

Java: "ab".repeat(3)
来源：http://bi.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://pk.hahajie.cn

Ruby: "ab" * 3
来源：http://or.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://os.colortex.cn

[E03] 截取子串
来源：http://wh.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zi.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nf.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dv.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://qr.shxzskj.cn

Java: s.substring(1, 4)
来源：http://tj.jctech888.com.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xh.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qu.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://zi.yuexingan06.cn

[E04] 查找子串位置
来源：http://rt.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://lg.nicolike.cn

PHP:  strpos($s, "x");
来源：http://xi.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mk.shxzukj.cn

TS:   s.indexOf("x")
来源：http://ih.gzmigu.cn

Java: s.indexOf("x")
来源：http://rk.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://tp.jctech888.com.cn

Ruby: s.index("x")
来源：http://ni.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://ol.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lc.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fd.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fb.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vj.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://da.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qk.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qu.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hx.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vl.huixinmuqiang.cn

[E06] 替换子串
来源：http://ye.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ch.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://iw.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tu.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://wr.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xk.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ss.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iy.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://yo.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://yf.newstarts.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iy.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dm.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wy.jctech888.com.cn

TS:   s.split(",")
来源：http://pk.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sn.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cj.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://uh.jianghongdianzi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://od.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://ll.bookmarksfly.cn

Py:   ",".join(items)
来源：http://gh.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://dh.szsharing.cn

JS:   items.join(",")
来源：http://pq.lnxyls.cn

TS:   items.join(",")
来源：http://sw.521024.cn

Java: String.join(",", items)
来源：http://cv.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://oj.asd995.cn

Ruby: items.join(",")
来源：http://xu.huanxung.cn

C#:   string.Join(",", items)
来源：http://px.colortex.cn

[E09] 去除所有空白字符
来源：http://lz.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zo.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hn.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://mz.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://ra.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://cb.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xa.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qo.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xf.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://ez.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://do.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vu.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://fi.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://td.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://nw.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ig.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cf.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uj.bookmarksfly.cn

[E11] 反转字符串
来源：http://aa.bookmarksfly.cn

Py:   s[::-1]
来源：http://vc.wgjwhj.cn

PHP:  strrev($s);
来源：http://oo.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://oy.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://hl.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kd.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://eu.jianghongdianzi.cn

Ruby: s.reverse
来源：http://bq.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ou.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://yu.huixinmuqiang.cn

Py:   s.count("a")
来源：http://rr.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://ok.newstarts.cn

JS:   s.split("a").length - 1
来源：http://nc.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://ke.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pt.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://my.huixiangedu.cn

Ruby: s.count("a")
来源：http://jv.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://cm.wgjwhj.cn

[E13] 逐字符遍历
来源：http://kq.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://qe.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zq.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vt.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ma.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ro.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lz.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://am.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vp.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://hr.huixiangedu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://db.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sr.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pt.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xb.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vc.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ym.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cr.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cj.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://ak.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lc.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nq.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wn.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jy.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ie.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mk.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ew.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vu.nszjky.cn

[E16] 数字千分位
来源：http://gy.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://cc.521024.cn

PHP:  number_format(1234567);
来源：http://sl.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zz.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sa.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vv.9csxet.cn


<!-- 参考信息 -->