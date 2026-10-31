代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vv.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cd.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://se.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://tr.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ow.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ks.colortex.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vj.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ga.szxytkj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://js.panjiajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ht.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vf.yuntaijiaju.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ly.nszjky.cn

[A10] 生成随机数
来源：http://ys.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://el.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://hr.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rj.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zp.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://oi.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ar.hnjuh.cn

Ruby: rand(1..100)
来源：http://mg.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://tp.nszjky.cn

[A11] 条件表达式（三元）
来源：http://hd.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://tl.szxytkj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pd.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kh.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jp.jctech888.com.cn

Java: x > 0 ? "yes" : "no"
来源：http://oc.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ck.panjiajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qj.huixiangedu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ni.521024.cn

[A12] 字符串插值 / 格式化
来源：http://og.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://me.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zz.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://mw.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://cc.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://rf.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fg.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://rc.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://lm.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tc.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://sm.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://cv.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://le.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://uj.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://jq.nszjky.cn

Go:   "第一行\n第二行"
来源：http://bc.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://di.nicolike.cn

C#:   "第一行\n第二行"
来源：http://yp.yuntaijiaju.cn

[A14] 注释写法
来源：http://jo.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fe.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ym.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://mp.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://lp.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rl.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://dg.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ai.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://iu.nicolike.cn

[A15] 空值判断与默认值
来源：http://ul.szxytkj.cn

Py:   value = data or "默认值"
来源：http://em.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://vq.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://fm.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://kd.shxzskj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sh.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://wn.colortex.cn

Ruby: value = data || "默认值"
来源：http://hw.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://ei.asd995.cn

[A16] 真假值判断规则
来源：http://pi.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ms.wgjwhj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ex.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lo.shxzskj.cn

TS:   if (!x) {}
来源：http://xx.521024.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pq.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ls.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ox.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yt.chemitech.net.cn

[A17] 位运算
来源：http://rg.muxihuayi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://my.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://aa.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nz.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lv.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ny.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rv.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mb.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zx.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://jg.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://ex.521024.cn

PHP:  ord("A"); chr(65)
来源：http://pn.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ma.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ec.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://hi.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bs.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://pp.gzmigu.cn

C#:   (int)'A'; (char)65
来源：http://vu.shtwfgs.cn

[A19] 交换两个变量
来源：http://zb.newstarts.cn

Py:   a, b = b, a
来源：http://fl.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://se.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://mh.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://fr.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://th.huanxung.cn

Go:   a, b = b, a
来源：http://sl.muxihuayi.cn

Ruby: a, b = b, a
来源：http://yp.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://cz.521024.cn

[A20] 读取标准输入
来源：http://kp.newstarts.cn

Py:   name = input("请输入：")
来源：http://pc.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ye.wgjwhj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ts.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://uz.hnjuh.cn

Java: new Scanner(System.in).nextLine()
来源：http://rk.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dp.yuexingan06.cn

Ruby: gets.chomp
来源：http://dh.gzmigu.cn

C#:   Console.ReadLine();
来源：http://wf.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://de.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://hb.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ep.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://zy.521024.cn

TS:   (3.14159).toFixed(2)
来源：http://mq.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://nx.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yr.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://zh.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://ot.huanxung.cn

[A22] 获取字符串长度
来源：http://ee.wgjwhj.cn

Py:   len(s)
来源：http://uz.muxihuayi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://md.haigaiapp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gi.nicolike.cn

TS:   s.length
来源：http://er.huanxung.cn

Java: s.length()
来源：http://iy.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cm.jctech888.com.cn

Ruby: s.length
来源：http://im.szsharing.cn

C#:   s.Length
来源：http://br.yuntaijiaju.cn

[A23] 大小写转换
来源：http://tl.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sn.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vr.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yx.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ql.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yl.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ve.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uo.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cb.szxytkj.cn

[A24] 去除首尾空白
来源：http://zf.huanxung.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lt.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hp.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ty.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dz.bjjhwx.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zj.gzmigu.cn

Go:   strings.TrimSpace(s)
来源：http://fm.wgjwhj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ow.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zm.nszjky.cn

[A25] 字符串比较
来源：http://gz.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://gv.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ku.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kw.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nu.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://in.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ws.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jn.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mw.haigaiapp.cn

[A26] 类型转换总览
来源：http://on.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dp.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mw.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dc.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://vx.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ft.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://di.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nc.haigaiapp.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://up.shtwfgs.cn

================================================================================
来源：http://vn.nszjky.cn

B. 流程控制
来源：http://ky.9csxet.cn

================================================================================
来源：http://az.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://zl.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://at.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tz.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xd.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ic.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hb.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://im.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fj.hnjuh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ea.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://tx.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pi.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ne.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xu.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ca.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fc.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kw.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kp.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qc.chemitech.net.cn

[B03] switch / match / case
来源：http://gw.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wk.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pc.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ey.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ja.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vk.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hm.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xn.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tg.huixinmuqiang.cn

[B04] for 计数循环
来源：http://eu.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://ym.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eq.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qu.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oo.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ra.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ze.asd995.cn

Ruby: 10.times { |i| puts i }
来源：http://pg.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zv.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://lw.nszjky.cn

Py:   for item in arr: print(item)
来源：http://sx.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xc.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zc.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cy.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dx.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qr.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://pf.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fa.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://nd.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ug.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://as.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nh.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ip.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fk.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cd.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ev.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pp.bookmarksfly.cn

[B07] while 循环
来源：http://lu.newstarts.cn

Py:   while i < 10: i += 1
来源：http://fq.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ru.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://zt.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://va.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://ya.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rn.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://yf.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://fa.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://me.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://ko.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ku.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://jn.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://ju.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://iq.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sk.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://eb.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://gj.bookmarksfly.cn

[B09] break 与 continue
来源：http://wl.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pl.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vf.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dw.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uz.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cd.muxihuayi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://os.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vb.szsharing.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rz.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://jr.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ux.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zh.wgjwhj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rv.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uy.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uj.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pa.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pw.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://re.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://vs.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://yt.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://bz.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ce.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xc.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oc.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ai.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://fa.gzmigu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ok.hnjuh.cn

[B12] 跳出多层循环
来源：http://gm.nszjky.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bm.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mi.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://fq.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ys.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eu.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gy.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kh.jctech888.com.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yv.lnxyls.cn

[B13] 判断是否为数字
来源：http://dn.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://kd.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://ta.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tv.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bz.521024.cn

Java: x instanceof Number
来源：http://wq.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yf.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://ym.panjiajie.cn

C#:   x is int or double or decimal
来源：http://as.huanxung.cn

[B14] 判断值是否在集合内
来源：http://et.shxzukj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zu.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cs.jctech888.com.cn

JS:   [1, 2, 3].includes(x)
来源：http://hz.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://ga.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ji.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ma.shxzukj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ky.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://un.hnjuh.cn

[B15] 布尔运算与取反
来源：http://sg.lnxyls.cn

Py:   a and b or not c
来源：http://kj.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://mj.huanxung.cn

JS:   a && b || !c
来源：http://fa.yuntaijiaju.cn

TS:   a && b || !c
来源：http://dk.shxzukj.cn

Java: a && b || !c
来源：http://nn.shtwfgs.cn


<!-- 参考信息 -->