代发 wailian999

[A06] 字符串转数字
来源：http://xv.colortex.cn

Py:   int("42"); float("3.14")
来源：http://ic.szsharing.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lg.shxzukj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yq.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cw.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kt.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ti.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bl.chemitech.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pc.yuntaijiaju.cn

[A07] 数字转字符串
来源：http://xk.bjjhwx.cn

Py:   str(42)
来源：http://rr.nicolike.cn

PHP:  (string) 42; strval(42)
来源：http://fd.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://dw.yuexingan06.cn

TS:   String(42)
来源：http://cd.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bs.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://pd.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://ex.haigaiapp.cn

C#:   42.ToString()
来源：http://dd.szxytkj.cn

[A08] 取整与四舍五入
来源：http://qj.szxytkj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ms.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vi.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uh.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bf.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yq.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rs.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ht.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pn.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://ns.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cl.huixiangedu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ao.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gd.jctech888.com.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://go.gzmigu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vu.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://af.jianghongdianzi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tg.huixinmuqiang.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://aq.haigaiapp.cn

[A10] 生成随机数
来源：http://wp.shxzukj.cn

Py:   import random; random.randint(1, 100)
来源：http://cy.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://gu.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kb.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dn.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://oe.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ov.muxihuayi.cn

Ruby: rand(1..100)
来源：http://bi.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://cv.newstarts.cn

[A11] 条件表达式（三元）
来源：http://xt.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://hq.gzmigu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hi.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://oi.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wa.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://lh.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://le.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ke.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lo.521024.cn

[A12] 字符串插值 / 格式化
来源：http://ry.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://is.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hb.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://yw.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://au.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://yj.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jd.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://gh.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://is.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qk.jianghongdianzi.cn

Py:   "第一行\n第二行"
来源：http://rv.shtwfgs.cn

PHP:  "第一行\n第二行"
来源：http://ew.nszjky.cn

JS:   "第一行\n第二行"
来源：http://vo.521024.cn

TS:   "第一行\n第二行"
来源：http://ny.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://ql.hahajie.cn

Go:   "第一行\n第二行"
来源：http://qh.shxzukj.cn

Ruby: "第一行\n第二行"
来源：http://jk.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://yl.9csxet.cn

[A14] 注释写法
来源：http://aj.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xm.nszjky.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bf.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://bg.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://tk.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mr.gzmigu.cn

Go:   // 单行；/* 多行 */
来源：http://st.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qo.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://jl.szsharing.cn

[A15] 空值判断与默认值
来源：http://wy.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://mh.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://wa.521024.cn

JS:   const value = data ?? "默认值";
来源：http://wp.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://ry.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zy.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://ri.521024.cn

Ruby: value = data || "默认值"
来源：http://yn.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://qv.muxihuayi.cn

[A16] 真假值判断规则
来源：http://rs.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uc.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ul.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rn.huanxung.cn

TS:   if (!x) {}
来源：http://gd.gzmigu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jy.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kh.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xa.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ho.newstarts.cn

[A17] 位运算
来源：http://op.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yp.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ah.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ur.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jn.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ds.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mp.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ov.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ff.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://jr.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://hx.asd995.cn

PHP:  ord("A"); chr(65)
来源：http://ni.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vk.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jf.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://zu.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://es.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://rg.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://xm.asd995.cn

[A19] 交换两个变量
来源：http://iu.nicolike.cn

Py:   a, b = b, a
来源：http://xy.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vd.jianghongdianzi.cn

JS:   [a, b] = [b, a];
来源：http://xz.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://rx.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://kq.gzmigu.cn

Go:   a, b = b, a
来源：http://pe.9csxet.cn

Ruby: a, b = b, a
来源：http://xv.colortex.cn

C#:   (a, b) = (b, a);
来源：http://hh.szsharing.cn

[A20] 读取标准输入
来源：http://vq.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://zq.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ss.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oi.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://at.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://xe.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lp.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://yh.hahajie.cn

C#:   Console.ReadLine();
来源：http://ry.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://tx.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://zq.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ia.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://cz.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://ny.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://es.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fe.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://hn.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://tm.shtwfgs.cn

[A22] 获取字符串长度
来源：http://aq.nicolike.cn

Py:   len(s)
来源：http://uk.lnxyls.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://le.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jr.yuntaijiaju.cn

TS:   s.length
来源：http://oa.jctech888.com.cn

Java: s.length()
来源：http://fi.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fm.muxihuayi.cn

Ruby: s.length
来源：http://wo.hnjuh.cn

C#:   s.Length
来源：http://ag.hahajie.cn

[A23] 大小写转换
来源：http://qs.bjjhwx.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xi.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hm.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ri.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zd.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nh.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rj.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zk.hahajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mq.newstarts.cn

[A24] 去除首尾空白
来源：http://ji.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fg.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vn.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lc.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pr.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ij.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://vq.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bd.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vq.wgjwhj.cn

[A25] 字符串比较
来源：http://tr.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://br.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lz.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://os.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ou.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://og.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://st.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pd.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://su.shxzskj.cn

[A26] 类型转换总览
来源：http://fr.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kz.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gf.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hh.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://qq.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uc.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dn.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jt.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lh.shxzskj.cn

================================================================================
来源：http://co.huixinmuqiang.cn

B. 流程控制
来源：http://mr.bjjhwx.cn

================================================================================
来源：http://kg.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://en.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ow.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ys.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lj.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jp.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://em.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tf.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xf.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ke.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://ed.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hl.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tv.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rn.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ul.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://id.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bm.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pe.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wo.lnxyls.cn

[B03] switch / match / case
来源：http://ff.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rg.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kl.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wb.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fh.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sr.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ia.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cy.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zn.huixiangedu.cn

[B04] for 计数循环
来源：http://pq.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://tb.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nu.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gl.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ut.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ut.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ph.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://yf.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iy.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://kb.wgjwhj.cn

Py:   for item in arr: print(item)
来源：http://yi.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kj.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hg.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://db.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ad.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jw.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://yt.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ls.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://qn.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lq.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sf.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fa.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tz.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yf.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lr.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fi.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qa.bookmarksfly.cn

[B07] while 循环
来源：http://yf.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://jh.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yf.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://se.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://xc.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://sw.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kb.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://wr.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://zw.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://to.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://pt.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vx.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://mb.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://gu.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://ah.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qi.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qa.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://ui.bookmarksfly.cn

[B09] break 与 continue
来源：http://ya.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ky.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://li.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eg.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wm.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hm.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ev.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://am.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xw.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://wp.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ci.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hs.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wn.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ae.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ua.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://me.shxzskj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uo.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fd.521024.cn

[B11] 生成数字序列 / 区间
来源：http://ra.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://om.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://wm.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://br.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rj.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ms.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nv.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://wz.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lj.colortex.cn

[B12] 跳出多层循环
来源：http://ub.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nm.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ex.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hw.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cf.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qk.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bs.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xz.shxzukj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://to.newstarts.cn


<!-- 参考信息 -->