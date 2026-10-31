代发 wailian999

Java: new ArrayList<>(list);
来源：http://ck.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://so.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://lv.bjjhwx.cn

C#:   new List<int>(list);
来源：http://cj.szxytkj.cn

[D23] reduce 累积计算
来源：http://xu.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pc.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dj.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ds.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zx.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vt.chemitech.net.cn

Go:   // 手写循环
来源：http://iz.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mn.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bp.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://oq.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ra.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ke.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ef.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lf.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nk.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bo.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jr.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pb.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://ne.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ls.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qz.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://db.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zw.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xm.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ip.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ep.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kp.panjiajie.cn

[D26] 数组转字符串
来源：http://pm.shtwfgs.cn

Py:   ", ".join(map(str, arr))
来源：http://lb.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://oz.chemitech.net.cn

JS:   arr.join(", ")
来源：http://gn.huixinmuqiang.cn

TS:   arr.join(", ")
来源：http://am.szsharing.cn

Java: String.join(", ", list)
来源：http://om.nicolike.cn

Go:   strings.Join(strs, ", ")
来源：http://nh.shxzskj.cn

Ruby: arr.join(", ")
来源：http://oc.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://nf.shxzukj.cn

================================================================================
来源：http://ny.huanxung.cn

E. 字符串处理
来源：http://rl.shxzskj.cn

================================================================================
来源：http://ef.szsharing.cn

[E01] 拼接字符串
来源：http://ko.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://js.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kn.colortex.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nd.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dw.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pa.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gm.shtwfgs.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mq.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ne.bjjhwx.cn

[E02] 重复字符串
来源：http://aj.shxzskj.cn

Py:   "ab" * 3
来源：http://ci.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://jw.asd995.cn

JS:   "ab".repeat(3)
来源：http://mk.panjiajie.cn

TS:   "ab".repeat(3)
来源：http://co.nicolike.cn

Java: "ab".repeat(3)
来源：http://ad.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://sf.9csxet.cn

Ruby: "ab" * 3
来源：http://yj.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uq.shtwfgs.cn

[E03] 截取子串
来源：http://ur.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rg.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vv.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wd.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://cr.hnjuh.cn

Java: s.substring(1, 4)
来源：http://nj.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nc.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cf.asd995.cn

C#:   s.Substring(1, 3)
来源：http://et.shxzskj.cn

[E04] 查找子串位置
来源：http://ia.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://ty.szsharing.cn

PHP:  strpos($s, "x");
来源：http://gu.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qh.huanxung.cn

TS:   s.indexOf("x")
来源：http://fx.hahajie.cn

Java: s.indexOf("x")
来源：http://hn.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://vw.shxzukj.cn

Ruby: s.index("x")
来源：http://jr.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://bj.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lb.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lv.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://et.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qo.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vy.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mr.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aq.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kt.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://re.szxytkj.cn

[E06] 替换子串
来源：http://pq.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pr.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://nf.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://og.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://ko.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fb.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://df.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://np.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://ei.asd995.cn

[E07] 按分隔符拆分
来源：http://gg.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xx.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xk.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bj.shtwfgs.cn

TS:   s.split(",")
来源：http://yl.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://do.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://id.bjjhwx.cn

Ruby: s.split(",");  s.split
来源：http://ar.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gf.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://jw.nszjky.cn

Py:   ",".join(items)
来源：http://sn.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://hh.shxzskj.cn

JS:   items.join(",")
来源：http://hl.panjiajie.cn

TS:   items.join(",")
来源：http://su.gzmigu.cn

Java: String.join(",", items)
来源：http://hb.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://wn.huixiangedu.cn

Ruby: items.join(",")
来源：http://if.shxzukj.cn

C#:   string.Join(",", items)
来源：http://ge.colortex.cn

[E09] 去除所有空白字符
来源：http://yx.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://st.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gc.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://je.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://xc.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://ju.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wc.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bv.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ko.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://wq.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yw.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lb.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://qw.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://gj.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://uw.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ft.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://os.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ek.lnxyls.cn

[E11] 反转字符串
来源：http://ky.yuexingan06.cn

Py:   s[::-1]
来源：http://be.wgjwhj.cn

PHP:  strrev($s);
来源：http://fe.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://jz.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://pg.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wh.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jl.lnxyls.cn

Ruby: s.reverse
来源：http://pp.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://oh.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://dp.chemitech.net.cn

Py:   s.count("a")
来源：http://mo.shxzskj.cn

PHP:  substr_count($s, "a");
来源：http://yz.asd995.cn

JS:   s.split("a").length - 1
来源：http://vn.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://js.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jg.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://he.muxihuayi.cn

Ruby: s.count("a")
来源：http://rj.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://py.hahajie.cn

[E13] 逐字符遍历
来源：http://vy.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://bg.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kl.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wp.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kz.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qa.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wk.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ud.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nb.newstarts.cn

[E14] URL 编码与 Base64
来源：http://vs.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ms.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xt.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pm.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fc.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mu.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sn.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gi.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zt.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://yn.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kc.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dv.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fv.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gr.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dq.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fh.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cn.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jx.colortex.cn

[E16] 数字千分位
来源：http://pv.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://rc.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://zz.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pk.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vo.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://co.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nj.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eu.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://ga.shxzukj.cn

[E17] 首字母大写
来源：http://ky.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bv.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kp.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oo.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kv.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://po.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://km.huixiangedu.cn

Ruby: s.capitalize
来源：http://oq.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ut.huixiangedu.cn

[E18] 模板占位符替换
来源：http://xq.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mp.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iz.bjjhwx.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qs.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yf.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tx.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qm.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ok.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://fl.shxzskj.cn

Py:   s.splitlines()
来源：http://qe.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://el.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://cz.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://ob.bjjhwx.cn

Java: s.lines().toList()
来源：http://kw.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://xf.szxytkj.cn

Ruby: s.lines
来源：http://lc.hahajie.cn

C#:   s.Split('\n')
来源：http://pz.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://sx.hnjuh.cn

Py:   if not s:
来源：http://qn.huixinmuqiang.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wi.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sd.szxytkj.cn

TS:   if (s === "") {}
来源：http://dw.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://gd.lnxyls.cn

Go:   if s == "" {}
来源：http://gp.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://ud.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ap.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://na.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ml.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wv.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gl.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oo.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kh.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://ho.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ib.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xx.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://zj.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sw.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sm.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bi.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jg.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uj.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xt.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://nv.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yh.jctech888.com.cn

================================================================================
来源：http://pc.shtwfgs.cn

F. 文件与目录
来源：http://dy.bjjhwx.cn

================================================================================
来源：http://zy.asd995.cn

[F01] 读取整个文件
来源：http://fb.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://na.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://mz.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qb.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vf.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vc.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ay.szsharing.cn

Ruby: File.read("a.txt")
来源：http://vv.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://zy.shtwfgs.cn

[F02] 逐行读取文件
来源：http://fv.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bk.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pk.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gl.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qa.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zu.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ns.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://db.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dz.asd995.cn

[F03] 写入文件（覆盖）
来源：http://yg.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tx.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mx.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nq.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mx.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mm.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zo.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://ck.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oj.bjjhwx.cn

[F04] 追加写入文件
来源：http://iz.hnjuh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mm.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fd.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oj.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nw.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wu.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rs.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nb.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hv.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://si.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wo.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://fd.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://dw.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://br.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ok.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vt.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://tq.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://up.haigaiapp.cn

[F06] 删除文件
来源：http://jx.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://ff.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://gw.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fy.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gj.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yi.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://yn.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://le.521024.cn

C#:   File.Delete("a.txt");
来源：http://ay.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://nv.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bm.chemitech.net.cn


<!-- 参考信息 -->