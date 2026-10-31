代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://by.szxytkj.cn

Ruby: arr.include?(x)
来源：http://gc.chemitech.net.cn

C#:   list.Contains(x)
来源：http://qh.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://ds.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eu.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jb.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zt.shxzukj.cn

TS:   [...arr];
来源：http://uw.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://ml.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tm.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://rw.muxihuayi.cn

C#:   new List<int>(list);
来源：http://iw.shtwfgs.cn

[D23] reduce 累积计算
来源：http://te.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ar.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cc.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://so.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ra.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fd.haigaiapp.cn

Go:   // 手写循环
来源：http://gq.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ht.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gt.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://vh.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ua.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ue.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nz.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qb.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yq.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nz.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ns.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bw.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://kr.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oq.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vd.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ys.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://by.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://db.521024.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tz.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rp.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://li.szxytkj.cn

[D26] 数组转字符串
来源：http://mx.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://sf.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://vv.newstarts.cn

JS:   arr.join(", ")
来源：http://nu.yuexingan06.cn

TS:   arr.join(", ")
来源：http://eg.asd995.cn

Java: String.join(", ", list)
来源：http://nw.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://yd.newstarts.cn

Ruby: arr.join(", ")
来源：http://tn.szsharing.cn

C#:   string.Join(", ", list)
来源：http://fe.nicolike.cn

================================================================================
来源：http://ur.yuntaijiaju.cn

E. 字符串处理
来源：http://hj.shxzukj.cn

================================================================================
来源：http://vx.bookmarksfly.cn

[E01] 拼接字符串
来源：http://nb.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yp.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wq.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ul.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mr.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://op.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pu.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yi.9csxet.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pm.hahajie.cn

[E02] 重复字符串
来源：http://hs.shxzukj.cn

Py:   "ab" * 3
来源：http://zi.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://va.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://sc.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://pr.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://lg.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://na.huanxung.cn

Ruby: "ab" * 3
来源：http://lx.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gd.9csxet.cn

[E03] 截取子串
来源：http://nu.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bk.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zt.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ne.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://gq.panjiajie.cn

Java: s.substring(1, 4)
来源：http://je.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hj.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wm.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://cu.wgjwhj.cn

[E04] 查找子串位置
来源：http://yn.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://eb.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://oa.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pe.panjiajie.cn

TS:   s.indexOf("x")
来源：http://sf.muxihuayi.cn

Java: s.indexOf("x")
来源：http://dw.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://qw.shxzskj.cn

Ruby: s.index("x")
来源：http://zd.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://ru.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wi.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hb.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cc.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://al.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kg.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sy.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zl.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rf.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cv.shxzskj.cn

[E06] 替换子串
来源：http://dt.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hd.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://xv.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ue.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://sz.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xp.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oy.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fb.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://oo.gzmigu.cn

[E07] 按分隔符拆分
来源：http://vm.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tg.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ph.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ba.bookmarksfly.cn

TS:   s.split(",")
来源：http://wu.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lr.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xg.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://jk.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ir.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://ud.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://sb.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://zm.bookmarksfly.cn

JS:   items.join(",")
来源：http://qw.nicolike.cn

TS:   items.join(",")
来源：http://jq.szsharing.cn

Java: String.join(",", items)
来源：http://wm.521024.cn

Go:   strings.Join(items, ",")
来源：http://hm.jctech888.com.cn

Ruby: items.join(",")
来源：http://rn.shxzukj.cn

C#:   string.Join(",", items)
来源：http://tp.hnjuh.cn

[E09] 去除所有空白字符
来源：http://qi.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yq.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://em.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://yd.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://th.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://yt.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sv.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zr.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ki.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://rc.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ib.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kd.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://qp.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://ii.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://en.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gt.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tn.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wz.szsharing.cn

[E11] 反转字符串
来源：http://kr.jctech888.com.cn

Py:   s[::-1]
来源：http://nt.szsharing.cn

PHP:  strrev($s);
来源：http://va.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://mp.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://qa.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tt.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vt.haigaiapp.cn

Ruby: s.reverse
来源：http://cq.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jj.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://rp.shxzskj.cn

Py:   s.count("a")
来源：http://xj.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://vl.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://bp.nszjky.cn

TS:   s.split("a").length - 1
来源：http://nu.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zj.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://sb.nicolike.cn

Ruby: s.count("a")
来源：http://we.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://le.nszjky.cn

[E13] 逐字符遍历
来源：http://re.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://kl.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uq.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ox.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vs.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xo.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://me.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uj.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bd.newstarts.cn

[E14] URL 编码与 Base64
来源：http://lj.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uc.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cu.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mt.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xn.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kg.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yv.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ql.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jl.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://tx.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vk.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://of.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zj.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rz.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ln.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kb.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nx.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fq.9csxet.cn

[E16] 数字千分位
来源：http://fw.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://ky.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://nm.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dr.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ls.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gm.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xs.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://we.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://ec.9csxet.cn

[E17] 首字母大写
来源：http://gy.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://go.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sa.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ei.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vu.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hp.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fu.wgjwhj.cn

Ruby: s.capitalize
来源：http://xj.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pr.bjjhwx.cn

[E18] 模板占位符替换
来源：http://gs.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oy.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xi.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lf.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ez.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kg.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ge.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gy.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qh.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://jp.shxzskj.cn

Py:   s.splitlines()
来源：http://qu.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bi.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://ap.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://fj.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://xn.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://wk.shxzukj.cn

Ruby: s.lines
来源：http://qu.asd995.cn

C#:   s.Split('\n')
来源：http://cs.huanxung.cn

[E20] 判断字符串是否为空
来源：http://ht.wgjwhj.cn

Py:   if not s:
来源：http://gg.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ch.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ig.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://mv.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://td.9csxet.cn

Go:   if s == "" {}
来源：http://pf.huanxung.cn

Ruby: if s.empty?
来源：http://vp.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.colortex.cn

[E21] 超长截断加省略号
来源：http://np.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uy.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hy.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ac.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pp.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cg.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://ip.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cx.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ow.hahajie.cn

[E22] 字节长度与字符长度
来源：http://mg.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fm.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://di.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://px.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sr.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fu.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xn.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://kj.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://no.colortex.cn

================================================================================
来源：http://zr.jctech888.com.cn

F. 文件与目录
来源：http://zl.nszjky.cn

================================================================================
来源：http://eq.nicolike.cn

[F01] 读取整个文件
来源：http://wv.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://by.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://qb.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sh.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ez.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bs.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pi.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://st.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://hk.szxytkj.cn

[F02] 逐行读取文件
来源：http://nl.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eb.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ma.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kz.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ls.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yb.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hc.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://om.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lh.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://cf.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://te.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pd.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wf.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vn.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yw.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rl.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://xw.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yn.newstarts.cn

[F04] 追加写入文件
来源：http://rj.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ex.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gc.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rb.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uw.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://py.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gq.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nj.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fh.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://tg.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ek.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://ug.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://sl.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://ig.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ev.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zd.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://gm.colortex.cn

C#:   File.Exists("a.txt")
来源：http://nz.asd995.cn

[F06] 删除文件
来源：http://fn.newstarts.cn

Py:   os.remove("a.txt")
来源：http://lt.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://gg.521024.cn


<!-- 参考信息 -->