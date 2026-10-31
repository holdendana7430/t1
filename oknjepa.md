代发 wailian999

Ruby: 42.to_s
来源：http://tq.huixinmuqiang.cn

C#:   42.ToString()
来源：http://mr.hnjuh.cn

[A08] 取整与四舍五入
来源：http://qj.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://df.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jl.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sg.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fv.lnxyls.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tu.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rx.chemitech.net.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ue.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ti.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://nt.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://im.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xz.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pb.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ph.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://as.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://na.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lg.nszjky.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://iu.yuntaijiaju.cn

[A10] 生成随机数
来源：http://mr.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://ph.hahajie.cn

PHP:  random_int(1, 100);
来源：http://yy.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tt.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://je.shtwfgs.cn

Java: new Random().nextInt(100) + 1
来源：http://vz.shxzskj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://be.huixiangedu.cn

Ruby: rand(1..100)
来源：http://oe.shtwfgs.cn

C#:   new Random().Next(1, 101)
来源：http://vb.szsharing.cn

[A11] 条件表达式（三元）
来源：http://sd.hahajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://az.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rk.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://lb.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rn.asd995.cn

Java: x > 0 ? "yes" : "no"
来源：http://de.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vk.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mj.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gx.shxzukj.cn

[A12] 字符串插值 / 格式化
来源：http://ml.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zy.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gv.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://gc.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://qk.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://am.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lr.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://mu.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://wd.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ew.szsharing.cn

Py:   "第一行\n第二行"
来源：http://kb.shtwfgs.cn

PHP:  "第一行\n第二行"
来源：http://ub.521024.cn

JS:   "第一行\n第二行"
来源：http://dv.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://bj.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://ww.panjiajie.cn

Go:   "第一行\n第二行"
来源：http://ja.521024.cn

Ruby: "第一行\n第二行"
来源：http://gz.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://vs.muxihuayi.cn

[A14] 注释写法
来源：http://ud.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vx.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dl.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://ez.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://lf.szxytkj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nu.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://ak.newstarts.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ly.9csxet.cn

C#:   // 单行；/* 多行 */
来源：http://dq.gzmigu.cn

[A15] 空值判断与默认值
来源：http://vz.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://cp.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://yp.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://sh.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://hm.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dj.lnxyls.cn

Go:   if data == "" { data = "默认值" }
来源：http://ug.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://tg.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://lp.colortex.cn

[A16] 真假值判断规则
来源：http://qt.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ek.jctech888.com.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ka.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gg.huanxung.cn

TS:   if (!x) {}
来源：http://hs.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bn.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hd.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pk.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ri.wgjwhj.cn

[A17] 位运算
来源：http://uf.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xe.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://md.muxihuayi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qa.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://og.szxytkj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jg.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fm.panjiajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fx.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qx.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://bs.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://cg.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://rx.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cb.shxzukj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ep.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://nw.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vp.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://nt.colortex.cn

C#:   (int)'A'; (char)65
来源：http://ow.nszjky.cn

[A19] 交换两个变量
来源：http://wb.chemitech.net.cn

Py:   a, b = b, a
来源：http://yp.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sa.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://yk.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://fa.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://fy.haigaiapp.cn

Go:   a, b = b, a
来源：http://ti.lnxyls.cn

Ruby: a, b = b, a
来源：http://ym.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://am.huixiangedu.cn

[A20] 读取标准输入
来源：http://kd.gzmigu.cn

Py:   name = input("请输入：")
来源：http://nl.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fo.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ss.521024.cn

TS:   // Node.js：readline 模块
来源：http://kw.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://vj.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qm.9csxet.cn

Ruby: gets.chomp
来源：http://lc.nicolike.cn

C#:   Console.ReadLine();
来源：http://em.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://zi.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://kj.nszjky.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jo.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://gp.521024.cn

TS:   (3.14159).toFixed(2)
来源：http://vc.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://iy.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lb.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://ut.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://nq.bjjhwx.cn

[A22] 获取字符串长度
来源：http://ho.huixinmuqiang.cn

Py:   len(s)
来源：http://ee.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yc.szxytkj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xk.shxzskj.cn

TS:   s.length
来源：http://kh.asd995.cn

Java: s.length()
来源：http://fy.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://er.huanxung.cn

Ruby: s.length
来源：http://jf.muxihuayi.cn

C#:   s.Length
来源：http://ev.muxihuayi.cn

[A23] 大小写转换
来源：http://ah.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vt.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qc.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qt.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gw.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://da.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ex.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kp.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://li.shxzskj.cn

[A24] 去除首尾空白
来源：http://ft.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mv.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qe.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nr.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wo.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fw.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://yu.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bm.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jr.9csxet.cn

[A25] 字符串比较
来源：http://yj.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://re.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jg.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lb.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hd.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jm.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bh.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://se.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pz.lnxyls.cn

[A26] 类型转换总览
来源：http://wb.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dn.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jn.yuexingan06.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://es.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://by.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cg.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rv.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://td.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vq.panjiajie.cn

================================================================================
来源：http://by.haigaiapp.cn

B. 流程控制
来源：http://zg.haigaiapp.cn

================================================================================
来源：http://jr.panjiajie.cn

[B01] 条件判断 if / else
来源：http://vb.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ma.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qu.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gz.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xq.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yg.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wh.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://op.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hi.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://mh.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nt.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wc.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jw.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eg.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rw.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dc.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vm.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eh.shxzukj.cn

[B03] switch / match / case
来源：http://mj.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zg.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://of.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sq.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uy.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qm.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ke.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://db.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://md.shtwfgs.cn

[B04] for 计数循环
来源：http://gd.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://kw.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ib.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jo.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ds.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ab.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mi.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://oh.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://th.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://qq.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://if.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dh.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gx.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bk.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fu.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yf.haigaiapp.cn

Ruby: arr.each { |item| puts item }
来源：http://bj.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ff.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://kc.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ef.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xb.hahajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ie.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fq.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ua.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vi.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wb.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vc.bjjhwx.cn

[B07] while 循环
来源：http://uy.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://oo.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tc.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://ns.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://iv.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://qz.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sq.shtwfgs.cn

Ruby: while i < 10; i += 1; end
来源：http://zv.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://gf.521024.cn

[B08] do-while（至少执行一次）
来源：http://zc.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://yg.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xv.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://bq.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://bu.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://ge.nicolike.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vo.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ea.asd995.cn

C#:   do { i++; } while (i < 10);
来源：http://qn.nicolike.cn

[B09] break 与 continue
来源：http://xq.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xj.muxihuayi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cz.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pa.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kw.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kx.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lf.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jz.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xh.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://dx.shxzskj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rr.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ji.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ha.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gn.shtwfgs.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ux.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gn.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pt.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qi.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://sa.jianghongdianzi.cn

Py:   list(range(0, 10, 2))
来源：http://tk.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://gt.9csxet.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bs.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qg.colortex.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zs.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://de.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://pu.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iu.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://jj.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ua.newstarts.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lz.hnjuh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xr.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ok.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://si.asd995.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tw.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nr.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qo.newstarts.cn

[B13] 判断是否为数字
来源：http://kk.huixinmuqiang.cn

Py:   isinstance(x, (int, float))
来源：http://vk.newstarts.cn

PHP:  is_numeric($x)
来源：http://iz.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aa.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ed.shtwfgs.cn

Java: x instanceof Number
来源：http://np.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mc.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://ck.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://hh.newstarts.cn

[B14] 判断值是否在集合内
来源：http://jw.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ni.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vo.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://vk.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://eu.lnxyls.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qg.shtwfgs.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yd.yuntaijiaju.cn


<!-- 参考信息 -->