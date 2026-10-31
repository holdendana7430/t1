代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vi.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yh.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jw.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://kn.bjjhwx.cn

Ruby: arr.index(x)
来源：http://qo.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://lt.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://ln.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zj.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cu.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://io.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://za.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xb.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dh.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yk.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://to.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://yt.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ih.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eq.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://hm.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://hd.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yn.bookmarksfly.cn

Go:   // 手写循环
来源：http://iz.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bp.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tg.yuntaijiaju.cn

[D15] 去重
来源：http://gt.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ue.panjiajie.cn

PHP:  array_unique($arr);
来源：http://dc.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://ij.szsharing.cn

TS:   [...new Set(arr)]
来源：http://le.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gq.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qr.panjiajie.cn

Ruby: arr.uniq
来源：http://zt.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://rh.jctech888.com.cn

[D16] 求和与平均值
来源：http://tu.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uv.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sd.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oi.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iz.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oc.asd995.cn

Go:   // 手写循环累加
来源：http://kc.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yk.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://sk.hahajie.cn

[D17] 最大值与最小值
来源：http://un.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://wi.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://ds.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zq.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://dn.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wq.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ct.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://op.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://fu.asd995.cn

[D18] 扁平化嵌套数组
来源：http://dt.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://or.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://wt.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ru.haigaiapp.cn

TS:   nested.flat();
来源：http://fj.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fb.shxzukj.cn

Go:   // 手写双层循环
来源：http://vu.bookmarksfly.cn

Ruby: nested.flatten
来源：http://se.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://so.panjiajie.cn

[D19] 按字段分组
来源：http://iq.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://to.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://db.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ft.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://je.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bq.521024.cn

Go:   // 手写 map[string][]T
来源：http://bt.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xw.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zv.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://wt.hnjuh.cn

Py:   Counter(arr)
来源：http://gx.newstarts.cn

PHP:  array_count_values($arr);
来源：http://pv.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hn.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fa.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lb.nicolike.cn

Go:   // 手写 map[T]int
来源：http://ab.jianghongdianzi.cn

Ruby: arr.tally
来源：http://bh.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ot.huanxung.cn

[D21] 判断是否包含某元素
来源：http://nv.shtwfgs.cn

Py:   x in arr
来源：http://wx.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://ga.nicolike.cn

JS:   arr.includes(x)
来源：http://eq.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://bh.bookmarksfly.cn

Java: list.contains(x)
来源：http://em.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://vg.shxzukj.cn

Ruby: arr.include?(x)
来源：http://kq.chemitech.net.cn

C#:   list.Contains(x)
来源：http://kx.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://sp.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rm.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cf.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gc.bookmarksfly.cn

TS:   [...arr];
来源：http://bg.nszjky.cn

Java: new ArrayList<>(list);
来源：http://fk.chemitech.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nt.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://ur.gzmigu.cn

C#:   new List<int>(list);
来源：http://jt.colortex.cn

[D23] reduce 累积计算
来源：http://po.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jn.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qa.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mt.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ds.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jz.yuntaijiaju.cn

Go:   // 手写循环
来源：http://ot.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bv.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nf.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://if.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gk.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ic.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ut.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ro.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fb.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ya.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jg.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rk.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://sw.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oy.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jf.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pk.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sh.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xv.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gz.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bj.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gp.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://fl.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://rh.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://ij.9csxet.cn

JS:   arr.join(", ")
来源：http://wv.hahajie.cn

TS:   arr.join(", ")
来源：http://dz.bjjhwx.cn

Java: String.join(", ", list)
来源：http://rh.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://yt.panjiajie.cn

Ruby: arr.join(", ")
来源：http://dg.colortex.cn

C#:   string.Join(", ", list)
来源：http://lt.panjiajie.cn

================================================================================
来源：http://hz.shxzukj.cn

E. 字符串处理
来源：http://md.nicolike.cn

================================================================================
来源：http://xn.haigaiapp.cn

[E01] 拼接字符串
来源：http://az.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qd.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://du.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kg.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sw.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tw.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tu.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://px.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xj.asd995.cn

[E02] 重复字符串
来源：http://lx.shtwfgs.cn

Py:   "ab" * 3
来源：http://mg.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://kt.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://xl.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://qd.szxytkj.cn

Java: "ab".repeat(3)
来源：http://jn.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://qg.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://em.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sp.haigaiapp.cn

[E03] 截取子串
来源：http://ow.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mo.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yg.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yp.nszjky.cn

TS:   s.slice(1, 4)
来源：http://te.hnjuh.cn

Java: s.substring(1, 4)
来源：http://kq.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iw.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cg.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://zl.shxzskj.cn

[E04] 查找子串位置
来源：http://uz.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://ue.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://ek.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nc.jianghongdianzi.cn

TS:   s.indexOf("x")
来源：http://sd.521024.cn

Java: s.indexOf("x")
来源：http://dl.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://bp.bookmarksfly.cn

Ruby: s.index("x")
来源：http://cr.newstarts.cn

C#:   s.IndexOf("x")
来源：http://cp.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ja.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xp.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kp.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kq.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qc.yuntaijiaju.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://di.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sp.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jq.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ar.colortex.cn

[E06] 替换子串
来源：http://fp.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://do.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://qt.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ua.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://tw.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qz.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bm.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mq.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://hs.shxzskj.cn

[E07] 按分隔符拆分
来源：http://js.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ik.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aq.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cg.hahajie.cn

TS:   s.split(",")
来源：http://fc.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qo.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ff.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://ib.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ji.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://bz.szsharing.cn

Py:   ",".join(items)
来源：http://aw.hnjuh.cn

PHP:  implode(",", $items);
来源：http://lv.shtwfgs.cn

JS:   items.join(",")
来源：http://yt.muxihuayi.cn

TS:   items.join(",")
来源：http://pw.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://gr.asd995.cn

Go:   strings.Join(items, ",")
来源：http://uy.hnjuh.cn

Ruby: items.join(",")
来源：http://gt.szxytkj.cn

C#:   string.Join(",", items)
来源：http://pw.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://kj.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jl.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bk.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://da.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://mg.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://iw.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xv.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://im.huixiangedu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pl.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://ht.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hy.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bw.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://cb.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://bu.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://bp.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://py.huixiangedu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wm.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wr.shxzskj.cn

[E11] 反转字符串
来源：http://yw.gzmigu.cn

Py:   s[::-1]
来源：http://fy.muxihuayi.cn

PHP:  strrev($s);
来源：http://by.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://ud.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://xq.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tb.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dm.asd995.cn

Ruby: s.reverse
来源：http://zd.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ff.nicolike.cn

[E12] 统计某字符出现次数
来源：http://wv.gzmigu.cn

Py:   s.count("a")
来源：http://wh.panjiajie.cn

PHP:  substr_count($s, "a");
来源：http://fh.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://za.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://wg.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iy.9csxet.cn

Go:   strings.Count(s, "a")
来源：http://vu.asd995.cn

Ruby: s.count("a")
来源：http://uq.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://fv.bjjhwx.cn

[E13] 逐字符遍历
来源：http://hk.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://uf.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tn.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://to.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cg.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hq.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bk.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://va.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ba.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://jc.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hc.shxzukj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dc.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://za.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rq.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lj.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jv.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xo.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oi.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://zo.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jv.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bq.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pd.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zo.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dq.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pn.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ay.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zf.shtwfgs.cn

[E16] 数字千分位
来源：http://gd.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://nx.huanxung.cn

PHP:  number_format(1234567);
来源：http://js.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ki.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://py.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fe.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bu.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fn.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://ly.shxzukj.cn

[E17] 首字母大写
来源：http://ai.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yd.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hd.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cf.wgjwhj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vl.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uy.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://px.yuexingan06.cn

Ruby: s.capitalize
来源：http://jo.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lf.hnjuh.cn

[E18] 模板占位符替换
来源：http://kp.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uo.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hw.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ld.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ue.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ld.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tu.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qm.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ai.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://bp.huanxung.cn

Py:   s.splitlines()
来源：http://jd.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hs.huanxung.cn


<!-- 参考信息 -->