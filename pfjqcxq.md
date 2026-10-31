代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://kv.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rz.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://nz.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qa.shxzskj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ze.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://bq.shxzskj.cn

Py:   Counter(arr)
来源：http://uu.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://ed.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ue.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cd.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dx.hahajie.cn

Go:   // 手写 map[T]int
来源：http://vo.yuntaijiaju.cn

Ruby: arr.tally
来源：http://ub.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jr.huanxung.cn

[D21] 判断是否包含某元素
来源：http://pt.asd995.cn

Py:   x in arr
来源：http://yj.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://wh.bjjhwx.cn

JS:   arr.includes(x)
来源：http://oo.521024.cn

TS:   arr.includes(x)
来源：http://uj.shxzukj.cn

Java: list.contains(x)
来源：http://rr.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://ii.9csxet.cn

Ruby: arr.include?(x)
来源：http://wn.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://bc.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://ot.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://er.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rd.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xc.huanxung.cn

TS:   [...arr];
来源：http://pw.haigaiapp.cn

Java: new ArrayList<>(list);
来源：http://cc.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://co.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://ep.huanxung.cn

C#:   new List<int>(list);
来源：http://jj.yuexingan06.cn

[D23] reduce 累积计算
来源：http://kg.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jb.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ex.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://co.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://du.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ik.asd995.cn

Go:   // 手写循环
来源：http://ka.hnjuh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kx.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ar.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://ql.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iz.asd995.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oa.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sg.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ya.shxzukj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uy.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ut.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zr.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kg.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://jq.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gs.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://io.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zs.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ke.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ww.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kl.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rq.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://by.bjjhwx.cn

[D26] 数组转字符串
来源：http://ux.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://pt.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://ja.newstarts.cn

JS:   arr.join(", ")
来源：http://se.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://vi.szsharing.cn

Java: String.join(", ", list)
来源：http://af.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://cz.nicolike.cn

Ruby: arr.join(", ")
来源：http://dq.shtwfgs.cn

C#:   string.Join(", ", list)
来源：http://sv.haigaiapp.cn

================================================================================
来源：http://ak.nicolike.cn

E. 字符串处理
来源：http://bh.huixinmuqiang.cn

================================================================================
来源：http://bx.haigaiapp.cn

[E01] 拼接字符串
来源：http://ga.wgjwhj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ms.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hx.shxzukj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bv.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bi.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uu.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cs.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nc.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lz.nszjky.cn

[E02] 重复字符串
来源：http://kw.lnxyls.cn

Py:   "ab" * 3
来源：http://qp.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://xv.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://gc.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://pw.huanxung.cn

Java: "ab".repeat(3)
来源：http://fm.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://mb.huanxung.cn

Ruby: "ab" * 3
来源：http://vg.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eu.huanxung.cn

[E03] 截取子串
来源：http://ga.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lb.gzmigu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://og.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lv.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://kp.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://nh.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mw.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ly.panjiajie.cn

C#:   s.Substring(1, 3)
来源：http://bn.shtwfgs.cn

[E04] 查找子串位置
来源：http://zs.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://oe.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://rl.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ry.huanxung.cn

TS:   s.indexOf("x")
来源：http://ii.colortex.cn

Java: s.indexOf("x")
来源：http://ek.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://xf.lnxyls.cn

Ruby: s.index("x")
来源：http://vi.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://ef.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yc.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ic.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qi.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pc.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wu.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lk.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hj.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xg.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fq.panjiajie.cn

[E06] 替换子串
来源：http://sd.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qs.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://ue.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tn.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://vs.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://og.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fw.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wa.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://ur.shxzukj.cn

[E07] 按分隔符拆分
来源：http://fg.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dv.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://da.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hq.haigaiapp.cn

TS:   s.split(",")
来源：http://ko.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vf.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fe.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://pr.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sb.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://py.9csxet.cn

Py:   ",".join(items)
来源：http://rf.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://nt.shxzukj.cn

JS:   items.join(",")
来源：http://aa.huixinmuqiang.cn

TS:   items.join(",")
来源：http://dc.521024.cn

Java: String.join(",", items)
来源：http://wl.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://be.yuexingan06.cn

Ruby: items.join(",")
来源：http://to.asd995.cn

C#:   string.Join(",", items)
来源：http://md.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://sv.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nn.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bu.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://dj.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://oh.szsharing.cn

Java: s.replaceAll("\\s+", "")
来源：http://lx.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ky.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tj.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kq.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://to.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zj.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kg.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://aa.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://vq.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://oa.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jk.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zy.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kh.haigaiapp.cn

[E11] 反转字符串
来源：http://uw.hahajie.cn

Py:   s[::-1]
来源：http://ez.shxzukj.cn

PHP:  strrev($s);
来源：http://cx.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://st.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://yi.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xh.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bn.asd995.cn

Ruby: s.reverse
来源：http://qa.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tm.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://wt.jianghongdianzi.cn

Py:   s.count("a")
来源：http://ns.wgjwhj.cn

PHP:  substr_count($s, "a");
来源：http://hi.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://nk.huanxung.cn

TS:   s.split("a").length - 1
来源：http://ng.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ke.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://du.hnjuh.cn

Ruby: s.count("a")
来源：http://pe.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://uq.yuexingan06.cn

[E13] 逐字符遍历
来源：http://nv.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://ht.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ek.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iv.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wq.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rc.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uu.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xp.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ot.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://kx.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ty.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ku.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bw.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bl.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xm.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lw.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fn.haigaiapp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tm.521024.cn

[E15] HTML 转义 / 反转义
来源：http://cg.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pv.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ps.newstarts.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fn.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://oj.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ft.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xy.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mg.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gw.muxihuayi.cn

[E16] 数字千分位
来源：http://wc.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://ib.9csxet.cn

PHP:  number_format(1234567);
来源：http://wq.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ay.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lp.panjiajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cy.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xa.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hw.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://dt.asd995.cn

[E17] 首字母大写
来源：http://sb.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rf.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qt.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ws.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mj.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vw.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yu.9csxet.cn

Ruby: s.capitalize
来源：http://ld.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://be.shtwfgs.cn

[E18] 模板占位符替换
来源：http://jv.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ud.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nm.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cw.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rd.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ix.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mm.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xl.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eo.asd995.cn

[E19] 多行文本按行拆分
来源：http://qh.521024.cn

Py:   s.splitlines()
来源：http://rw.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qm.gzmigu.cn

JS:   s.split(/\r?\n/)
来源：http://qj.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://xy.chemitech.net.cn

Java: s.lines().toList()
来源：http://pm.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://ln.huixiangedu.cn

Ruby: s.lines
来源：http://pc.colortex.cn

C#:   s.Split('\n')
来源：http://xk.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://vp.huixinmuqiang.cn

Py:   if not s:
来源：http://bq.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kp.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vc.muxihuayi.cn

TS:   if (s === "") {}
来源：http://ut.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://jr.nszjky.cn

Go:   if s == "" {}
来源：http://sl.newstarts.cn

Ruby: if s.empty?
来源：http://je.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wm.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://cn.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rc.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lk.shtwfgs.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iy.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ow.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dh.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://gh.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bu.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iq.colortex.cn

[E22] 字节长度与字符长度
来源：http://lg.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vj.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://br.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fs.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bh.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ay.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jc.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://kv.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lt.gzmigu.cn

================================================================================
来源：http://ds.huixinmuqiang.cn

F. 文件与目录
来源：http://af.szsharing.cn

================================================================================
来源：http://bf.yuexingan06.cn

[F01] 读取整个文件
来源：http://ex.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://is.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://os.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sg.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wg.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://py.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zb.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://ft.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://wi.muxihuayi.cn

[F02] 逐行读取文件
来源：http://gv.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tf.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ag.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vo.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rl.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zy.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gx.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pg.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bb.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://hd.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iu.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ok.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uo.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ym.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fg.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ss.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://ad.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fq.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://xr.9csxet.cn


<!-- 参考信息 -->