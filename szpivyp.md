代发 wailian999

[D11] 反转数组
来源：http://lm.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://df.521024.cn

PHP:  array_reverse($arr);
来源：http://gz.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rf.nszjky.cn

TS:   [...arr].reverse();
来源：http://hk.newstarts.cn

Java: Collections.reverse(list);
来源：http://yt.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://vj.gzmigu.cn

Ruby: arr.reverse
来源：http://ks.shtwfgs.cn

C#:   list.Reverse();
来源：http://om.gzmigu.cn

[D12] 查找元素下标
来源：http://jw.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://at.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ok.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jw.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bf.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ir.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://ub.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://bk.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://ar.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://rs.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rq.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bh.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://st.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://jx.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://di.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ot.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ws.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jk.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://nz.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nu.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ho.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://hc.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://jp.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://al.521024.cn

Go:   // 手写循环
来源：http://xr.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://po.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://px.szxytkj.cn

[D15] 去重
来源：http://cy.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tw.newstarts.cn

PHP:  array_unique($arr);
来源：http://cd.newstarts.cn

JS:   [...new Set(arr)]
来源：http://lh.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://na.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yk.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xl.shxzukj.cn

Ruby: arr.uniq
来源：http://yr.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://qh.szxytkj.cn

[D16] 求和与平均值
来源：http://ul.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cp.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rd.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://le.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jp.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://in.hnjuh.cn

Go:   // 手写循环累加
来源：http://uz.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zu.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://dx.szxytkj.cn

[D17] 最大值与最小值
来源：http://tv.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://il.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://sw.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ho.szxytkj.cn

TS:   Math.max(...arr);
来源：http://bg.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pj.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yd.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://in.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://qp.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://nl.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gi.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://iv.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ck.szxytkj.cn

TS:   nested.flat();
来源：http://kp.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://do.bjjhwx.cn

Go:   // 手写双层循环
来源：http://li.bjjhwx.cn

Ruby: nested.flatten
来源：http://xg.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ci.huanxung.cn

[D19] 按字段分组
来源：http://lm.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://os.wgjwhj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://md.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qo.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gi.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rx.colortex.cn

Go:   // 手写 map[string][]T
来源：http://uu.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sc.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rg.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://jf.chemitech.net.cn

Py:   Counter(arr)
来源：http://mp.colortex.cn

PHP:  array_count_values($arr);
来源：http://vy.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jz.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://th.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fl.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://ku.9csxet.cn

Ruby: arr.tally
来源：http://ma.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jc.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://wb.nszjky.cn

Py:   x in arr
来源：http://mj.bookmarksfly.cn

PHP:  in_array($x, $arr, true);
来源：http://ht.jctech888.com.cn

JS:   arr.includes(x)
来源：http://mr.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://cz.nszjky.cn

Java: list.contains(x)
来源：http://fe.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://da.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://jk.panjiajie.cn

C#:   list.Contains(x)
来源：http://de.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://sx.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fu.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rc.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ch.yuntaijiaju.cn

TS:   [...arr];
来源：http://pn.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://xx.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tf.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://vz.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://yc.yuexingan06.cn

[D23] reduce 累积计算
来源：http://im.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tr.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jb.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sx.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rw.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wd.asd995.cn

Go:   // 手写循环
来源：http://ek.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bw.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yt.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://bc.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wf.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gc.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hm.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ix.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fp.asd995.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://by.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xf.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pf.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://ak.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ou.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cc.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yp.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ko.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ee.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hx.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vy.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zg.hahajie.cn

[D26] 数组转字符串
来源：http://jd.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://fe.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://la.9csxet.cn

JS:   arr.join(", ")
来源：http://oo.newstarts.cn

TS:   arr.join(", ")
来源：http://oj.chemitech.net.cn

Java: String.join(", ", list)
来源：http://ss.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://nt.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://mb.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://ri.huanxung.cn

================================================================================
来源：http://pi.9csxet.cn

E. 字符串处理
来源：http://bz.szxytkj.cn

================================================================================
来源：http://tt.yuexingan06.cn

[E01] 拼接字符串
来源：http://tj.521024.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yp.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sq.hahajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pw.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://un.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lh.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sp.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jz.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uh.nicolike.cn

[E02] 重复字符串
来源：http://um.hnjuh.cn

Py:   "ab" * 3
来源：http://pp.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://ol.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://bi.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://kz.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://sg.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://yc.lnxyls.cn

Ruby: "ab" * 3
来源：http://lt.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ox.huixiangedu.cn

[E03] 截取子串
来源：http://zm.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://my.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dh.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ud.521024.cn

TS:   s.slice(1, 4)
来源：http://xw.gzmigu.cn

Java: s.substring(1, 4)
来源：http://fe.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ma.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nr.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://oy.9csxet.cn

[E04] 查找子串位置
来源：http://mv.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://tj.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://ga.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zl.521024.cn

TS:   s.indexOf("x")
来源：http://rh.hahajie.cn

Java: s.indexOf("x")
来源：http://uf.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://lv.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://ji.9csxet.cn

C#:   s.IndexOf("x")
来源：http://pk.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://if.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jr.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nz.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://es.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bq.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lt.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://id.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xw.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zo.521024.cn

[E06] 替换子串
来源：http://vy.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gp.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://bl.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bd.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://nq.huixiangedu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://co.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vi.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ps.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://kc.shxzskj.cn

[E07] 按分隔符拆分
来源：http://nd.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ce.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yx.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tj.yuexingan06.cn

TS:   s.split(",")
来源：http://pn.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ia.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bp.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://di.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wv.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://lh.jctech888.com.cn

Py:   ",".join(items)
来源：http://et.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://dl.bjjhwx.cn

JS:   items.join(",")
来源：http://eh.szxytkj.cn

TS:   items.join(",")
来源：http://ys.nicolike.cn

Java: String.join(",", items)
来源：http://mm.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://dx.521024.cn

Ruby: items.join(",")
来源：http://eb.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://ns.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://fq.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xh.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://be.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://bq.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://ng.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://ky.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zq.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pl.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fd.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://rx.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zd.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nt.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://gq.lnxyls.cn

TS:   "7".padStart(3, "0")
来源：http://uj.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://zj.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jj.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zk.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oy.shxzukj.cn

[E11] 反转字符串
来源：http://ge.bookmarksfly.cn

Py:   s[::-1]
来源：http://uj.haigaiapp.cn

PHP:  strrev($s);
来源：http://ro.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://ps.colortex.cn

TS:   [...s].reverse().join("")
来源：http://dp.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uy.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gr.chemitech.net.cn

Ruby: s.reverse
来源：http://la.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://aq.huanxung.cn

[E12] 统计某字符出现次数
来源：http://ni.bookmarksfly.cn

Py:   s.count("a")
来源：http://rw.asd995.cn

PHP:  substr_count($s, "a");
来源：http://tw.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://xr.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://je.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vc.521024.cn

Go:   strings.Count(s, "a")
来源：http://js.jctech888.com.cn

Ruby: s.count("a")
来源：http://av.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://on.9csxet.cn

[E13] 逐字符遍历
来源：http://qd.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://bp.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xa.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vx.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nt.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nk.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rm.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ot.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xm.hahajie.cn

[E14] URL 编码与 Base64
来源：http://of.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jc.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uq.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lo.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://da.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qz.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zi.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hl.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ca.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://ac.colortex.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oi.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://su.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qj.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://iq.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ji.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://by.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ni.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fx.nicolike.cn

[E16] 数字千分位
来源：http://do.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://wn.hnjuh.cn

PHP:  number_format(1234567);
来源：http://xa.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://om.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zf.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://es.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eg.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jv.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://uu.bookmarksfly.cn

[E17] 首字母大写
来源：http://ja.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hb.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zf.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mn.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sv.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://si.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rf.lnxyls.cn

Ruby: s.capitalize
来源：http://iz.colortex.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jw.muxihuayi.cn


<!-- 参考信息 -->