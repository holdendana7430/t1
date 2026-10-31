代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ok.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rg.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wj.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xc.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nm.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ve.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wh.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://yn.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://db.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fi.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ab.nszjky.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ih.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ij.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mc.bjjhwx.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rn.colortex.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gy.9csxet.cn

[A10] 生成随机数
来源：http://qr.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://fm.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://mo.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wl.hnjuh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cc.huixinmuqiang.cn

Java: new Random().nextInt(100) + 1
来源：http://nd.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bi.shtwfgs.cn

Ruby: rand(1..100)
来源：http://sb.hahajie.cn

C#:   new Random().Next(1, 101)
来源：http://yo.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://dw.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://ht.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rk.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://aw.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xu.jctech888.com.cn

Java: x > 0 ? "yes" : "no"
来源：http://rv.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ii.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wz.hnjuh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rh.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://bh.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ai.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fv.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://ps.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://oe.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://xy.shtwfgs.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mn.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://kw.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://ur.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pl.huixiangedu.cn

Py:   "第一行\n第二行"
来源：http://dl.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://sc.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://wo.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://nw.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://bm.nicolike.cn

Go:   "第一行\n第二行"
来源：http://qh.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://tt.huanxung.cn

C#:   "第一行\n第二行"
来源：http://fy.nszjky.cn

[A14] 注释写法
来源：http://no.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dm.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://eg.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://fy.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://ui.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mw.shtwfgs.cn

Go:   // 单行；/* 多行 */
来源：http://ur.huanxung.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cw.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://wg.shxzskj.cn

[A15] 空值判断与默认值
来源：http://yv.szxytkj.cn

Py:   value = data or "默认值"
来源：http://si.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://mc.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://wk.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://ew.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ju.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://tm.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://rw.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://lj.9csxet.cn

[A16] 真假值判断规则
来源：http://zs.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://by.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://il.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fk.newstarts.cn

TS:   if (!x) {}
来源：http://cn.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jy.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hy.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lf.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fs.nszjky.cn

[A17] 位运算
来源：http://br.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ch.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://if.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uk.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fd.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lg.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fw.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kn.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ua.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://gh.asd995.cn

Py:   ord("A"); chr(65)
来源：http://ue.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://ve.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bp.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lb.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://zc.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zp.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://fq.521024.cn

C#:   (int)'A'; (char)65
来源：http://nb.yuntaijiaju.cn

[A19] 交换两个变量
来源：http://gu.chemitech.net.cn

Py:   a, b = b, a
来源：http://ig.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tu.colortex.cn

JS:   [a, b] = [b, a];
来源：http://ri.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://tl.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://xj.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://al.gzmigu.cn

Ruby: a, b = b, a
来源：http://va.jctech888.com.cn

C#:   (a, b) = (b, a);
来源：http://oy.szsharing.cn

[A20] 读取标准输入
来源：http://ys.shxzukj.cn

Py:   name = input("请输入：")
来源：http://bs.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ye.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kq.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://dc.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://ju.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rs.wgjwhj.cn

Ruby: gets.chomp
来源：http://en.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://vj.asd995.cn

[A21] 保留指定小数位输出
来源：http://ay.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://tg.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ll.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://ul.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://lb.jianghongdianzi.cn

Java: String.format("%.2f", 3.14159)
来源：http://wp.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ig.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://be.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://rb.colortex.cn

[A22] 获取字符串长度
来源：http://zy.nszjky.cn

Py:   len(s)
来源：http://sa.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tl.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lr.shxzskj.cn

TS:   s.length
来源：http://ra.nicolike.cn

Java: s.length()
来源：http://ji.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://py.panjiajie.cn

Ruby: s.length
来源：http://kx.bjjhwx.cn

C#:   s.Length
来源：http://ks.bjjhwx.cn

[A23] 大小写转换
来源：http://ea.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mx.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dg.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sd.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kl.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://en.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://od.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kk.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://co.jctech888.com.cn

[A24] 去除首尾空白
来源：http://sy.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ut.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kl.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xm.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://le.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wa.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://ph.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bu.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://va.jianghongdianzi.cn

[A25] 字符串比较
来源：http://vi.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://be.bjjhwx.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ek.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ft.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qz.bjjhwx.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bk.chemitech.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cp.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wx.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nv.asd995.cn

[A26] 类型转换总览
来源：http://eb.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ki.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jv.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ep.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://dn.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rw.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iy.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ts.hnjuh.cn

================================================================================
来源：http://mb.hahajie.cn

B. 流程控制
来源：http://rp.hahajie.cn

================================================================================
来源：http://gl.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://xc.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kt.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nb.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sf.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fm.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vc.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lj.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yg.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wu.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://nu.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ij.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bv.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sd.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://na.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nj.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jh.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pb.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vy.gzmigu.cn

[B03] switch / match / case
来源：http://kd.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://js.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rx.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://us.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ge.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kq.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fa.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pr.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oy.panjiajie.cn

[B04] for 计数循环
来源：http://md.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://ra.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pm.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sd.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://je.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lr.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hf.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://sc.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yj.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://kp.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://ih.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ew.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yk.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gg.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ly.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://so.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://sh.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rl.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://cg.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ew.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://um.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nb.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ln.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jz.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xy.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tw.szsharing.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://th.lnxyls.cn

[B07] while 循环
来源：http://mx.szsharing.cn

Py:   while i < 10: i += 1
来源：http://xu.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jx.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://xn.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://xl.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://ra.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mx.yuntaijiaju.cn

Ruby: while i < 10; i += 1; end
来源：http://jz.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://jc.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://me.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://zc.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://or.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://vn.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://vh.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://so.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wu.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pm.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://wy.szsharing.cn

[B09] break 与 continue
来源：http://eh.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ry.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oq.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cr.shxzskj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bm.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iw.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vm.wgjwhj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tg.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sb.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://vb.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hp.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ur.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hh.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wj.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://no.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sw.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://no.gzmigu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tu.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://ww.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://ql.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://rg.nszjky.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fk.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dg.521024.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ok.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://iw.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bi.newstarts.cn

[B12] 跳出多层循环
来源：http://os.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wu.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vt.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ms.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qq.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rr.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://my.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ne.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iu.9csxet.cn

[B13] 判断是否为数字
来源：http://ih.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://fv.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://uf.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ac.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zh.lnxyls.cn

Java: x instanceof Number
来源：http://cr.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yk.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://ft.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://xn.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://ea.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xu.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ge.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://nc.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://jb.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nr.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vh.shtwfgs.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fu.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ti.shxzukj.cn

[B15] 布尔运算与取反
来源：http://qu.shxzskj.cn

Py:   a and b or not c
来源：http://po.bjjhwx.cn


<!-- 参考信息 -->