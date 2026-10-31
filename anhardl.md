代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://vf.huanxung.cn

Ruby: arr.include?(x)
来源：http://io.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://gx.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://wb.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ee.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fp.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sc.colortex.cn

TS:   [...arr];
来源：http://rq.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://ap.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ux.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://ie.muxihuayi.cn

C#:   new List<int>(list);
来源：http://bj.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://by.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mo.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zv.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xa.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bg.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zu.szsharing.cn

Go:   // 手写循环
来源：http://at.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sa.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wv.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://ac.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lb.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tn.newstarts.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://py.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wr.panjiajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gt.9csxet.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ts.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zr.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rq.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://rm.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qb.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tg.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fp.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yq.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zk.huanxung.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ly.muxihuayi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fx.bookmarksfly.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://co.9csxet.cn

[D26] 数组转字符串
来源：http://rp.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://aa.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://np.yuexingan06.cn

JS:   arr.join(", ")
来源：http://fw.hahajie.cn

TS:   arr.join(", ")
来源：http://iq.nszjky.cn

Java: String.join(", ", list)
来源：http://kk.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://ym.521024.cn

Ruby: arr.join(", ")
来源：http://zr.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://jw.newstarts.cn

================================================================================
来源：http://du.jianghongdianzi.cn

E. 字符串处理
来源：http://fd.huixiangedu.cn

================================================================================
来源：http://vb.shxzskj.cn

[E01] 拼接字符串
来源：http://my.bjjhwx.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qh.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tk.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://et.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xb.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fs.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uc.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fd.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nh.huixiangedu.cn

[E02] 重复字符串
来源：http://nw.chemitech.net.cn

Py:   "ab" * 3
来源：http://lx.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://bp.huanxung.cn

JS:   "ab".repeat(3)
来源：http://iw.szsharing.cn

TS:   "ab".repeat(3)
来源：http://uw.shxzskj.cn

Java: "ab".repeat(3)
来源：http://uz.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://cf.shtwfgs.cn

Ruby: "ab" * 3
来源：http://iv.colortex.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uc.jianghongdianzi.cn

[E03] 截取子串
来源：http://et.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xy.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://db.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ys.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://jw.9csxet.cn

Java: s.substring(1, 4)
来源：http://ml.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ek.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qn.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://hh.shxzukj.cn

[E04] 查找子串位置
来源：http://jn.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://vc.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://on.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://el.newstarts.cn

TS:   s.indexOf("x")
来源：http://vr.shxzskj.cn

Java: s.indexOf("x")
来源：http://li.521024.cn

Go:   strings.Index(s, "x")
来源：http://yt.nicolike.cn

Ruby: s.index("x")
来源：http://tb.nszjky.cn

C#:   s.IndexOf("x")
来源：http://ad.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vs.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sc.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qy.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ey.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zp.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cp.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://td.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hm.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ui.szsharing.cn

[E06] 替换子串
来源：http://dq.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jw.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://ue.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://on.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://dl.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qd.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://es.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zg.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://fw.nicolike.cn

[E07] 按分隔符拆分
来源：http://xq.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eq.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zx.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mo.colortex.cn

TS:   s.split(",")
来源：http://hc.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ef.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ho.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://qe.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ur.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://je.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://rg.asd995.cn

PHP:  implode(",", $items);
来源：http://oo.shtwfgs.cn

JS:   items.join(",")
来源：http://vx.shtwfgs.cn

TS:   items.join(",")
来源：http://ov.shxzukj.cn

Java: String.join(",", items)
来源：http://sw.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://yj.gzmigu.cn

Ruby: items.join(",")
来源：http://if.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://po.asd995.cn

[E09] 去除所有空白字符
来源：http://nc.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wh.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ah.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://bx.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://cu.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://zw.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zv.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pp.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://si.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://zv.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jy.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tg.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://eu.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://en.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://sa.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uy.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ja.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wa.chemitech.net.cn

[E11] 反转字符串
来源：http://aq.huixinmuqiang.cn

Py:   s[::-1]
来源：http://yl.jctech888.com.cn

PHP:  strrev($s);
来源：http://ka.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://ae.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://mr.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wj.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hg.shxzukj.cn

Ruby: s.reverse
来源：http://bp.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sb.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://mg.shtwfgs.cn

Py:   s.count("a")
来源：http://ca.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://sl.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://um.szsharing.cn

TS:   s.split("a").length - 1
来源：http://zn.bookmarksfly.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ry.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://on.szsharing.cn

Ruby: s.count("a")
来源：http://og.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://fs.nicolike.cn

[E13] 逐字符遍历
来源：http://tx.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://kn.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ml.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tj.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://my.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hc.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://du.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mr.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ha.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://ob.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ux.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://um.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kk.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tp.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://co.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ax.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hm.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://js.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://nj.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zi.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tc.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vn.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gc.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://du.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://km.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ob.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bg.shxzskj.cn

[E16] 数字千分位
来源：http://jv.szsharing.cn

Py:   f"{1234567:,}"
来源：http://zg.huanxung.cn

PHP:  number_format(1234567);
来源：http://di.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://me.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://od.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nm.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cf.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qe.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://dr.chemitech.net.cn

[E17] 首字母大写
来源：http://to.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nj.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ou.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aj.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zz.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pz.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://go.shxzukj.cn

Ruby: s.capitalize
来源：http://ye.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pc.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://xj.chemitech.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tc.colortex.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hg.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mh.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mn.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jn.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kz.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://um.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gv.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://av.colortex.cn

Py:   s.splitlines()
来源：http://xg.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pl.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://fb.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://xt.9csxet.cn

Java: s.lines().toList()
来源：http://yf.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://mq.szsharing.cn

Ruby: s.lines
来源：http://yv.nicolike.cn

C#:   s.Split('\n')
来源：http://oz.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://jv.szxytkj.cn

Py:   if not s:
来源：http://nz.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bb.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qn.9csxet.cn

TS:   if (s === "") {}
来源：http://ub.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://qq.bookmarksfly.cn

Go:   if s == "" {}
来源：http://lx.szsharing.cn

Ruby: if s.empty?
来源：http://kk.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ck.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://vx.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ro.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nz.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qq.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ls.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xm.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://rh.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cn.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dx.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://vw.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pq.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tf.shxzskj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jh.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sj.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jl.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tl.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://sd.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rx.9csxet.cn

================================================================================
来源：http://gg.huanxung.cn

F. 文件与目录
来源：http://ab.panjiajie.cn

================================================================================
来源：http://mu.nicolike.cn

[F01] 读取整个文件
来源：http://em.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nu.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://jv.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qs.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gf.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yh.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fx.newstarts.cn

Ruby: File.read("a.txt")
来源：http://pp.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://xv.asd995.cn

[F02] 逐行读取文件
来源：http://mr.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xz.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://af.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gz.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bh.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uq.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://av.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tm.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://en.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://av.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zh.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sq.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bp.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uw.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hl.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yb.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://kd.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ff.newstarts.cn

[F04] 追加写入文件
来源：http://on.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://np.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gh.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qz.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://st.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zo.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pz.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sk.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wo.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://nj.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://my.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://td.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://bu.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://xx.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lb.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vo.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://ol.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://pr.haigaiapp.cn

[F06] 删除文件
来源：http://hu.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://zn.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://sy.huixinmuqiang.cn


<!-- 参考信息 -->