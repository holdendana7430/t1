代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tl.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pp.521024.cn

JS:   arr.map(x => x * 2)
来源：http://hi.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://cm.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wc.shxzskj.cn

Go:   // 手写循环
来源：http://av.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rl.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ue.shxzukj.cn

[D15] 去重
来源：http://yq.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zx.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://ps.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://bz.nicolike.cn

TS:   [...new Set(arr)]
来源：http://rl.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jk.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bj.chemitech.net.cn

Ruby: arr.uniq
来源：http://kn.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://pt.chemitech.net.cn

[D16] 求和与平均值
来源：http://zv.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ay.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wa.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rz.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ao.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rl.yuexingan06.cn

Go:   // 手写循环累加
来源：http://ob.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lw.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://fc.huanxung.cn

[D17] 最大值与最小值
来源：http://ks.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://vz.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://ev.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ah.asd995.cn

TS:   Math.max(...arr);
来源：http://sw.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ng.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ln.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://qp.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://ve.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://zd.521024.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ul.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://ve.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pq.shxzukj.cn

TS:   nested.flat();
来源：http://qw.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lw.haigaiapp.cn

Go:   // 手写双层循环
来源：http://pe.nicolike.cn

Ruby: nested.flatten
来源：http://ne.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lp.lnxyls.cn

[D19] 按字段分组
来源：http://wo.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xy.bookmarksfly.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kl.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xz.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://la.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rh.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://ht.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nc.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zi.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://qp.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://hp.huanxung.cn

PHP:  array_count_values($arr);
来源：http://fe.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ck.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gj.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zc.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://bk.colortex.cn

Ruby: arr.tally
来源：http://jq.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ol.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://uz.bjjhwx.cn

Py:   x in arr
来源：http://ez.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://nn.panjiajie.cn

JS:   arr.includes(x)
来源：http://pr.shtwfgs.cn

TS:   arr.includes(x)
来源：http://gs.newstarts.cn

Java: list.contains(x)
来源：http://hu.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://ed.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://wt.yuexingan06.cn

C#:   list.Contains(x)
来源：http://zz.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://uv.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ng.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wj.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lk.newstarts.cn

TS:   [...arr];
来源：http://xu.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://wc.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ok.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://sr.jctech888.com.cn

C#:   new List<int>(list);
来源：http://ov.bjjhwx.cn

[D23] reduce 累积计算
来源：http://ae.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hp.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cu.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ys.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ji.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wp.shtwfgs.cn

Go:   // 手写循环
来源：http://ck.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eh.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hi.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://jm.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://me.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zs.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qn.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vq.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uf.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pz.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sh.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://og.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://kg.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://de.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pe.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nr.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dh.szxytkj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fq.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yh.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ms.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://do.yuexingan06.cn

[D26] 数组转字符串
来源：http://hj.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://qb.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://jj.shxzukj.cn

JS:   arr.join(", ")
来源：http://fq.newstarts.cn

TS:   arr.join(", ")
来源：http://mc.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://pu.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://lh.nicolike.cn

Ruby: arr.join(", ")
来源：http://qq.newstarts.cn

C#:   string.Join(", ", list)
来源：http://ef.huixinmuqiang.cn

================================================================================
来源：http://nt.jctech888.com.cn

E. 字符串处理
来源：http://xl.wgjwhj.cn

================================================================================
来源：http://go.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://ku.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://at.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ov.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sa.chemitech.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ys.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gs.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fe.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://im.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ln.huixiangedu.cn

[E02] 重复字符串
来源：http://ia.521024.cn

Py:   "ab" * 3
来源：http://hz.shxzskj.cn

PHP:  str_repeat("ab", 3);
来源：http://nq.newstarts.cn

JS:   "ab".repeat(3)
来源：http://mm.colortex.cn

TS:   "ab".repeat(3)
来源：http://ji.521024.cn

Java: "ab".repeat(3)
来源：http://vi.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://oq.szxytkj.cn

Ruby: "ab" * 3
来源：http://ig.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://na.521024.cn

[E03] 截取子串
来源：http://gl.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mw.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ph.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cq.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://qp.panjiajie.cn

Java: s.substring(1, 4)
来源：http://dl.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zy.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tx.asd995.cn

C#:   s.Substring(1, 3)
来源：http://hc.szxytkj.cn

[E04] 查找子串位置
来源：http://ln.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://cq.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://tp.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jg.hnjuh.cn

TS:   s.indexOf("x")
来源：http://kv.hahajie.cn

Java: s.indexOf("x")
来源：http://nh.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://zv.hahajie.cn

Ruby: s.index("x")
来源：http://gy.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://bt.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ip.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kc.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rh.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tt.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://it.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sv.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ry.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sx.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ir.bjjhwx.cn

[E06] 替换子串
来源：http://kv.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rz.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://dy.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qy.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://es.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tq.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wi.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sf.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://wz.hnjuh.cn

[E07] 按分隔符拆分
来源：http://vf.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rm.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oo.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qn.gzmigu.cn

TS:   s.split(",")
来源：http://vt.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vf.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ez.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://ia.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yn.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://ax.gzmigu.cn

Py:   ",".join(items)
来源：http://xm.szxytkj.cn

PHP:  implode(",", $items);
来源：http://ry.wgjwhj.cn

JS:   items.join(",")
来源：http://yw.lnxyls.cn

TS:   items.join(",")
来源：http://oj.shtwfgs.cn

Java: String.join(",", items)
来源：http://rk.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://gi.bookmarksfly.cn

Ruby: items.join(",")
来源：http://vx.shxzukj.cn

C#:   string.Join(",", items)
来源：http://sq.521024.cn

[E09] 去除所有空白字符
来源：http://cw.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tc.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nx.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://be.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://jy.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://kw.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fo.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mx.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mm.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://ys.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yx.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pi.huixinmuqiang.cn

JS:   "7".padStart(3, "0")
来源：http://ok.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://sx.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://vj.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sm.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lb.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ft.nicolike.cn

[E11] 反转字符串
来源：http://cj.gzmigu.cn

Py:   s[::-1]
来源：http://zq.muxihuayi.cn

PHP:  strrev($s);
来源：http://rg.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://ro.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://bf.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ij.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cy.gzmigu.cn

Ruby: s.reverse
来源：http://le.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ae.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://vf.bookmarksfly.cn

Py:   s.count("a")
来源：http://oh.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://xd.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://qd.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://ay.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kr.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://sl.nicolike.cn

Ruby: s.count("a")
来源：http://xu.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://pa.shxzskj.cn

[E13] 逐字符遍历
来源：http://ni.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://mx.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yc.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tm.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yn.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tz.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ic.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oo.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kh.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://zn.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pk.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wy.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zq.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vy.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://iu.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yc.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ik.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sw.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://ww.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ck.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ge.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ew.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://un.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xh.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lz.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nd.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zf.yuexingan06.cn

[E16] 数字千分位
来源：http://fb.newstarts.cn

Py:   f"{1234567:,}"
来源：http://ha.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://vb.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ef.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sq.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ks.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zu.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mx.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://ay.lnxyls.cn

[E17] 首字母大写
来源：http://ua.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://si.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ey.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mj.yuntaijiaju.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sc.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xa.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dk.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://ad.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vd.yuexingan06.cn

[E18] 模板占位符替换
来源：http://hn.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dp.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ay.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://if.9csxet.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gg.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nw.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ix.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qu.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qn.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://ho.shxzukj.cn

Py:   s.splitlines()
来源：http://fa.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://al.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://sy.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://me.huanxung.cn

Java: s.lines().toList()
来源：http://os.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://qy.jianghongdianzi.cn

Ruby: s.lines
来源：http://ze.shxzukj.cn

C#:   s.Split('\n')
来源：http://no.nszjky.cn

[E20] 判断字符串是否为空
来源：http://or.nszjky.cn

Py:   if not s:
来源：http://pf.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wn.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bn.newstarts.cn

TS:   if (s === "") {}
来源：http://vj.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://yr.bjjhwx.cn

Go:   if s == "" {}
来源：http://nk.521024.cn

Ruby: if s.empty?
来源：http://pa.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hy.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://xj.jctech888.com.cn


<!-- 参考信息 -->