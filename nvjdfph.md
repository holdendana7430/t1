代发 wailian999

Ruby: arr.index(x)
来源：http://rl.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://pa.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://ae.panjiajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gu.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pj.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://em.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://zb.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vc.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gj.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ph.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://it.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://wu.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cu.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fe.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://bs.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://bt.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oa.panjiajie.cn

Go:   // 手写循环
来源：http://ym.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qg.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ku.nszjky.cn

[D15] 去重
来源：http://uo.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ir.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://wz.nicolike.cn

JS:   [...new Set(arr)]
来源：http://qo.nszjky.cn

TS:   [...new Set(arr)]
来源：http://mz.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fu.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ay.nicolike.cn

Ruby: arr.uniq
来源：http://gk.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://cr.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://xu.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vn.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dh.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fm.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ef.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zp.huixiangedu.cn

Go:   // 手写循环累加
来源：http://lx.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://au.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://lr.chemitech.net.cn

[D17] 最大值与最小值
来源：http://wq.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://ks.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://gz.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fl.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://ac.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yq.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kh.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://dm.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://lh.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://sw.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gv.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://yy.shxzukj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cm.szsharing.cn

TS:   nested.flat();
来源：http://qg.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bl.shxzskj.cn

Go:   // 手写双层循环
来源：http://hs.hnjuh.cn

Ruby: nested.flatten
来源：http://rq.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vu.jianghongdianzi.cn

[D19] 按字段分组
来源：http://wc.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mf.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ko.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dm.wgjwhj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://aj.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://db.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://kz.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gk.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gv.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://pr.shtwfgs.cn

Py:   Counter(arr)
来源：http://tl.szsharing.cn

PHP:  array_count_values($arr);
来源：http://pk.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pd.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://up.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iz.nicolike.cn

Go:   // 手写 map[T]int
来源：http://ss.huanxung.cn

Ruby: arr.tally
来源：http://zy.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://au.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://ww.521024.cn

Py:   x in arr
来源：http://au.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://cm.huixiangedu.cn

JS:   arr.includes(x)
来源：http://ar.shxzskj.cn

TS:   arr.includes(x)
来源：http://rp.chemitech.net.cn

Java: list.contains(x)
来源：http://em.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://iu.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://xo.shxzukj.cn

C#:   list.Contains(x)
来源：http://cb.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://ue.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ui.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zq.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jc.nicolike.cn

TS:   [...arr];
来源：http://xo.newstarts.cn

Java: new ArrayList<>(list);
来源：http://qc.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ti.huixiangedu.cn

Ruby: arr.dup;  arr.clone
来源：http://ud.muxihuayi.cn

C#:   new List<int>(list);
来源：http://bu.bjjhwx.cn

[D23] reduce 累积计算
来源：http://zx.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qt.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ts.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ff.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hj.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ul.hahajie.cn

Go:   // 手写循环
来源：http://fc.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ki.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qu.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://zn.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ja.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zk.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cf.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hl.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oz.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qx.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tm.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yf.huanxung.cn

[D25] Set 集合去重与交并差
来源：http://fc.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ij.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mf.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wz.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mq.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sn.yuexingan06.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xd.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oz.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ys.gzmigu.cn

[D26] 数组转字符串
来源：http://if.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://mq.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://tz.nszjky.cn

JS:   arr.join(", ")
来源：http://to.muxihuayi.cn

TS:   arr.join(", ")
来源：http://pz.hahajie.cn

Java: String.join(", ", list)
来源：http://ig.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://hj.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://zr.9csxet.cn

C#:   string.Join(", ", list)
来源：http://xb.yuexingan06.cn

================================================================================
来源：http://wh.panjiajie.cn

E. 字符串处理
来源：http://hy.colortex.cn

================================================================================
来源：http://lf.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://va.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ex.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kf.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pa.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uz.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ky.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fp.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vq.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zp.shxzukj.cn

[E02] 重复字符串
来源：http://xu.szsharing.cn

Py:   "ab" * 3
来源：http://ux.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://ut.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://qa.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://gn.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://dh.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://ay.huanxung.cn

Ruby: "ab" * 3
来源：http://rb.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oj.lnxyls.cn

[E03] 截取子串
来源：http://vc.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kr.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://we.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qu.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://is.shxzskj.cn

Java: s.substring(1, 4)
来源：http://ma.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jr.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mh.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://po.bjjhwx.cn

[E04] 查找子串位置
来源：http://fp.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://wk.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://mh.colortex.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mv.huanxung.cn

TS:   s.indexOf("x")
来源：http://gp.bjjhwx.cn

Java: s.indexOf("x")
来源：http://ec.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://lr.bjjhwx.cn

Ruby: s.index("x")
来源：http://dw.huanxung.cn

C#:   s.IndexOf("x")
来源：http://cm.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ow.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xp.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wj.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yu.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ev.colortex.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lk.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ge.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lc.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qv.bjjhwx.cn

[E06] 替换子串
来源：http://yh.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qy.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://bk.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vg.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://qs.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uh.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://et.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cz.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://id.shxzskj.cn

[E07] 按分隔符拆分
来源：http://hd.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bz.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kg.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ap.panjiajie.cn

TS:   s.split(",")
来源：http://go.szsharing.cn

Java: s.split(",");  s.split("\\s+")
来源：http://be.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fd.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://mr.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mp.colortex.cn

[E08] 数组按分隔符合并
来源：http://ce.9csxet.cn

Py:   ",".join(items)
来源：http://cm.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://qo.hahajie.cn

JS:   items.join(",")
来源：http://xf.nszjky.cn

TS:   items.join(",")
来源：http://uj.nicolike.cn

Java: String.join(",", items)
来源：http://hu.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://ks.haigaiapp.cn

Ruby: items.join(",")
来源：http://wb.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://zq.521024.cn

[E09] 去除所有空白字符
来源：http://mk.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fi.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dj.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://ow.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://fm.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://fs.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jp.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rh.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ha.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://yo.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lz.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xl.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://yu.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://ny.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://ic.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mw.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ca.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ln.asd995.cn

[E11] 反转字符串
来源：http://nz.shtwfgs.cn

Py:   s[::-1]
来源：http://fz.bjjhwx.cn

PHP:  strrev($s);
来源：http://fz.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://qf.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://kr.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xq.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wu.hahajie.cn

Ruby: s.reverse
来源：http://ub.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ss.szsharing.cn

[E12] 统计某字符出现次数
来源：http://zv.bjjhwx.cn

Py:   s.count("a")
来源：http://ly.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://nx.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://vk.yuexingan06.cn

TS:   s.split("a").length - 1
来源：http://ey.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kc.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://mv.521024.cn

Ruby: s.count("a")
来源：http://tn.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://kb.szxytkj.cn

[E13] 逐字符遍历
来源：http://gv.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://vk.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gx.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uf.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fp.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yh.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vu.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ib.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qf.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://cn.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ql.huixinmuqiang.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ae.asd995.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ly.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ee.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lz.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ft.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yo.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mb.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://ty.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://id.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://so.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uk.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ax.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mi.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lr.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nm.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ne.shtwfgs.cn

[E16] 数字千分位
来源：http://cf.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://xq.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://bq.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kf.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vu.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ll.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vj.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gb.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://ul.szsharing.cn

[E17] 首字母大写
来源：http://dx.nszjky.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ye.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yr.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ts.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ag.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ff.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dd.panjiajie.cn

Ruby: s.capitalize
来源：http://gv.colortex.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ec.newstarts.cn

[E18] 模板占位符替换
来源：http://wt.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wb.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yq.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yg.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wz.shxzukj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tz.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qd.newstarts.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pl.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ty.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://ab.panjiajie.cn

Py:   s.splitlines()
来源：http://eh.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bl.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://ix.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://tj.shxzskj.cn

Java: s.lines().toList()
来源：http://id.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://tq.shxzskj.cn


<!-- 参考信息 -->