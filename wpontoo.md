代发 wailian999

JS:   String(42); (42).toString()
来源：http://wy.9csxet.cn

TS:   String(42)
来源：http://uf.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yi.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://dz.shxzukj.cn

Ruby: 42.to_s
来源：http://pa.lnxyls.cn

C#:   42.ToString()
来源：http://du.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://pl.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fe.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ai.szxytkj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kv.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://px.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nc.nszjky.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ez.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fr.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rx.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://wl.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ev.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mq.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sv.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://by.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://va.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://la.lnxyls.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hr.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xs.lnxyls.cn

[A10] 生成随机数
来源：http://is.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://eh.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://kq.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ii.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xw.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://ay.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zl.panjiajie.cn

Ruby: rand(1..100)
来源：http://vo.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://ta.huanxung.cn

[A11] 条件表达式（三元）
来源：http://pc.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://ii.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://zs.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gp.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yk.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://sx.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tc.hnjuh.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vm.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qk.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://wf.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qr.shxzukj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nd.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://fn.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://al.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://ql.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jm.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://jm.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://sw.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ai.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://xk.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://zg.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://tq.colortex.cn

TS:   "第一行\n第二行"
来源：http://od.chemitech.net.cn

Java: "第一行\n第二行"
来源：http://dz.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://oi.521024.cn

Ruby: "第一行\n第二行"
来源：http://gb.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://qk.asd995.cn

[A14] 注释写法
来源：http://wg.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zy.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kz.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://ko.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://vv.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ey.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://eq.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fa.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://my.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://oj.lnxyls.cn

Py:   value = data or "默认值"
来源：http://ct.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://ge.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://bz.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://vi.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://th.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://lj.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://uu.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://cg.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://pb.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yp.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fp.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://np.shtwfgs.cn

TS:   if (!x) {}
来源：http://bz.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bo.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://af.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hc.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fj.newstarts.cn

[A17] 位运算
来源：http://ca.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yz.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xo.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vh.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ev.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mm.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kn.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://at.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tt.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://uc.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://cr.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://yu.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ew.szsharing.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lt.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://zu.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pk.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://mp.colortex.cn

C#:   (int)'A'; (char)65
来源：http://yt.nszjky.cn

[A19] 交换两个变量
来源：http://jo.chemitech.net.cn

Py:   a, b = b, a
来源：http://kj.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fa.lnxyls.cn

JS:   [a, b] = [b, a];
来源：http://fv.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://eg.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://rp.521024.cn

Go:   a, b = b, a
来源：http://gs.lnxyls.cn

Ruby: a, b = b, a
来源：http://yj.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://wd.hahajie.cn

[A20] 读取标准输入
来源：http://js.9csxet.cn

Py:   name = input("请输入：")
来源：http://hw.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sn.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hy.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://dx.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://th.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ii.gzmigu.cn

Ruby: gets.chomp
来源：http://ph.lnxyls.cn

C#:   Console.ReadLine();
来源：http://hu.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://wk.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://ur.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gl.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://nd.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://ht.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://ja.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kc.wgjwhj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ns.wgjwhj.cn

C#:   3.14159.ToString("F2")
来源：http://fw.nszjky.cn

[A22] 获取字符串长度
来源：http://nb.wgjwhj.cn

Py:   len(s)
来源：http://ly.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ha.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aq.yuntaijiaju.cn

TS:   s.length
来源：http://vt.newstarts.cn

Java: s.length()
来源：http://at.nicolike.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ly.shxzukj.cn

Ruby: s.length
来源：http://el.shxzukj.cn

C#:   s.Length
来源：http://sm.newstarts.cn

[A23] 大小写转换
来源：http://qj.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jm.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://we.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fj.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://to.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rm.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kt.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oe.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hf.shxzskj.cn

[A24] 去除首尾空白
来源：http://pg.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pm.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ic.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lo.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kb.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://da.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://pk.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nj.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xb.nszjky.cn

[A25] 字符串比较
来源：http://uh.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://kd.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nf.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eu.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://od.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nd.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nb.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sn.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yx.chemitech.net.cn

[A26] 类型转换总览
来源：http://pc.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uc.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ty.yuntaijiaju.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://be.szxytkj.cn

TS:   Number() String() Boolean() x as number
来源：http://gy.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xr.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yz.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cd.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ym.huixiangedu.cn

================================================================================
来源：http://dr.gzmigu.cn

B. 流程控制
来源：http://wt.hahajie.cn

================================================================================
来源：http://sr.colortex.cn

[B01] 条件判断 if / else
来源：http://ns.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wk.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ph.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uk.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bk.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vc.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ve.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sa.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gk.521024.cn

[B02] 多分支 else if / elif
来源：http://ry.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zq.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mc.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jm.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://si.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ue.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lv.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zc.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oz.panjiajie.cn

[B03] switch / match / case
来源：http://ob.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dc.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://al.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ui.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pa.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ph.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bl.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fu.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://in.hahajie.cn

[B04] for 计数循环
来源：http://bj.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://uh.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zx.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kc.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yp.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eg.shxzukj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lx.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://tk.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ro.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://bk.newstarts.cn

Py:   for item in arr: print(item)
来源：http://ei.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qq.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ix.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vb.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://of.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rs.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://wm.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kf.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://xc.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ng.wgjwhj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tf.shxzskj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bj.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://to.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://na.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vo.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://td.panjiajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cg.huanxung.cn

[B07] while 循环
来源：http://ob.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://vq.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ze.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://ru.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://pr.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://wa.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://of.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://jp.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://sr.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://ht.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://gs.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mk.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://jb.nicolike.cn

TS:   do { i++; } while (i < 10);
来源：http://nv.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://mr.hahajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://im.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bt.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://us.hahajie.cn

[B09] break 与 continue
来源：http://il.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pl.shxzskj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iy.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yg.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ck.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mu.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nf.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dx.9csxet.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://it.nicolike.cn

[B10] 遍历同时拿索引
来源：http://bn.haigaiapp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ll.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dr.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ar.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lp.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pk.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iy.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bb.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dz.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://kd.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://fm.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://mf.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tm.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ys.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sr.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://am.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://jp.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tf.nszjky.cn

[B12] 跳出多层循环
来源：http://qc.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hk.jctech888.com.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nh.panjiajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zj.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xq.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nq.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gd.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tn.yuntaijiaju.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qr.shtwfgs.cn

[B13] 判断是否为数字
来源：http://ss.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://cc.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://ai.jctech888.com.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cg.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://df.shxzskj.cn

Java: x instanceof Number
来源：http://qb.nszjky.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ww.jctech888.com.cn

Ruby: x.is_a?(Numeric)
来源：http://nf.newstarts.cn

C#:   x is int or double or decimal
来源：http://rs.huixiangedu.cn

[B14] 判断值是否在集合内
来源：http://lh.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zm.szsharing.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xo.huixinmuqiang.cn


<!-- 参考信息 -->