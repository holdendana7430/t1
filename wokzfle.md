代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ik.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pd.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ud.nicolike.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wz.huixinmuqiang.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ub.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://sp.9csxet.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gz.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://ns.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yg.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cx.jctech888.com.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tk.shtwfgs.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vi.asd995.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oe.yuntaijiaju.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://du.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ud.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kj.shxzukj.cn

[A10] 生成随机数
来源：http://dk.huixiangedu.cn

Py:   import random; random.randint(1, 100)
来源：http://dc.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://qo.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wf.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xy.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://jn.shxzskj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ta.wgjwhj.cn

Ruby: rand(1..100)
来源：http://lm.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://zo.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://ny.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://dn.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xg.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://js.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kq.jctech888.com.cn

Java: x > 0 ? "yes" : "no"
来源：http://ho.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yt.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yv.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nn.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://qu.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kz.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mj.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://jo.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://vu.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://ek.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rf.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://eu.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://on.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://iz.huixiangedu.cn

Py:   "第一行\n第二行"
来源：http://vc.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://nq.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://fe.colortex.cn

TS:   "第一行\n第二行"
来源：http://qp.colortex.cn

Java: "第一行\n第二行"
来源：http://ca.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://tz.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://cs.szxytkj.cn

C#:   "第一行\n第二行"
来源：http://tr.yuexingan06.cn

[A14] 注释写法
来源：http://qy.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ot.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://os.521024.cn

JS:   // 单行；/* 多行 */
来源：http://va.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://ia.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mg.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://mw.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lw.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://mv.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://bc.huixiangedu.cn

Py:   value = data or "默认值"
来源：http://fz.shtwfgs.cn

PHP:  $value = $data ?? "默认值";
来源：http://yi.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://tp.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://ys.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oq.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://cu.szsharing.cn

Ruby: value = data || "默认值"
来源：http://zf.chemitech.net.cn

C#:   var value = data ?? "默认值";
来源：http://cy.shxzskj.cn

[A16] 真假值判断规则
来源：http://dn.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tf.haigaiapp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jy.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://df.shxzskj.cn

TS:   if (!x) {}
来源：http://nt.nicolike.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zr.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qr.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vr.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jd.9csxet.cn

[A17] 位运算
来源：http://sd.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ux.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gi.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oh.newstarts.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ny.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bm.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fl.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ot.colortex.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://df.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://nr.wgjwhj.cn

Py:   ord("A"); chr(65)
来源：http://ug.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://na.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zx.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ex.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://jf.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ac.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://qi.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://yb.asd995.cn

[A19] 交换两个变量
来源：http://wd.hnjuh.cn

Py:   a, b = b, a
来源：http://li.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cn.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://uj.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://mt.shxzukj.cn

Java: int t = a; a = b; b = t;
来源：http://pc.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://in.lnxyls.cn

Ruby: a, b = b, a
来源：http://kh.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://cr.nicolike.cn

[A20] 读取标准输入
来源：http://ox.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://pz.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tq.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dz.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://lp.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://qh.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wx.szxytkj.cn

Ruby: gets.chomp
来源：http://vi.hahajie.cn

C#:   Console.ReadLine();
来源：http://qz.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://dn.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://bm.muxihuayi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://st.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://te.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://fy.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ka.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ca.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://zb.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://pr.yuexingan06.cn

[A22] 获取字符串长度
来源：http://as.hahajie.cn

Py:   len(s)
来源：http://vd.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ad.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cv.huixinmuqiang.cn

TS:   s.length
来源：http://qh.yuntaijiaju.cn

Java: s.length()
来源：http://kj.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ke.szsharing.cn

Ruby: s.length
来源：http://cl.hnjuh.cn

C#:   s.Length
来源：http://ov.bjjhwx.cn

[A23] 大小写转换
来源：http://ad.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jm.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pi.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nj.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ug.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://me.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qg.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://co.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mm.nicolike.cn

[A24] 去除首尾空白
来源：http://eq.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fc.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vh.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sj.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dl.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lf.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://qg.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ea.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yr.huanxung.cn

[A25] 字符串比较
来源：http://un.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://xd.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xa.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iy.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nb.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mm.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fq.9csxet.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vz.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hq.haigaiapp.cn

[A26] 类型转换总览
来源：http://pf.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://he.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ms.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xf.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://un.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://af.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vg.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qw.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cr.521024.cn

================================================================================
来源：http://hw.gzmigu.cn

B. 流程控制
来源：http://qz.hnjuh.cn

================================================================================
来源：http://af.lnxyls.cn

[B01] 条件判断 if / else
来源：http://qf.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lb.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ny.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ma.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kf.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tk.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rm.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bn.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xu.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://if.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://px.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://su.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ke.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nd.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ol.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://av.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ua.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vz.panjiajie.cn

[B03] switch / match / case
来源：http://vp.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hq.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hr.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yd.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ml.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yu.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://us.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ja.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cj.nicolike.cn

[B04] for 计数循环
来源：http://ju.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://em.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bq.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ua.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wr.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uq.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iv.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://we.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uj.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://gr.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://uv.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sh.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dw.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gs.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jo.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cc.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://xw.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fj.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://va.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://po.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ok.yuntaijiaju.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rw.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://or.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vk.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iv.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ix.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fu.shxzukj.cn

[B07] while 循环
来源：http://mt.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://ym.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yy.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://ec.szxytkj.cn

TS:   while (i < 10) { i++; }
来源：http://sr.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://ba.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vx.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://yf.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://ny.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://ot.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://cc.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zp.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://bf.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://mw.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://qn.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jv.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kq.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://ye.huanxung.cn

[B09] break 与 continue
来源：http://yv.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bi.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wm.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ee.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lh.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://we.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kn.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mj.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sr.nicolike.cn

[B10] 遍历同时拿索引
来源：http://iw.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nk.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ph.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pw.bjjhwx.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rm.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lg.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nz.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dv.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://an.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://ws.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://hj.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://ai.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://si.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lm.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cu.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ze.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://th.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cy.hahajie.cn

[B12] 跳出多层循环
来源：http://nc.wgjwhj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pp.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hb.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ng.colortex.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nm.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qn.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ed.haigaiapp.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uc.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fg.colortex.cn

[B13] 判断是否为数字
来源：http://yk.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://ny.nszjky.cn

PHP:  is_numeric($x)
来源：http://dp.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://em.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iq.shxzskj.cn

Java: x instanceof Number
来源：http://mk.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uy.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://kw.huanxung.cn

C#:   x is int or double or decimal
来源：http://hj.haigaiapp.cn

[B14] 判断值是否在集合内
来源：http://yr.yuexingan06.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zd.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sv.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://eh.hnjuh.cn

TS:   [1, 2, 3].includes(x)
来源：http://vo.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ew.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oe.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hy.panjiajie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kc.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://ee.huanxung.cn

Py:   a and b or not c
来源：http://uy.gzmigu.cn


<!-- 参考信息 -->