代发 wailian999

JS:   String(42); (42).toString()
来源：http://tp.lnxyls.cn

TS:   String(42)
来源：http://ob.9csxet.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dz.huixinmuqiang.cn

Go:   strconv.Itoa(42)
来源：http://gb.nszjky.cn

Ruby: 42.to_s
来源：http://tf.jctech888.com.cn

C#:   42.ToString()
来源：http://gw.gzmigu.cn

[A08] 取整与四舍五入
来源：http://oj.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yo.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dg.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jx.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dh.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://md.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mc.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fc.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gk.huanxung.cn

[A09] 绝对值与最大最小值
来源：http://ua.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://je.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lc.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zg.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eh.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lu.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ul.muxihuayi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vz.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ea.9csxet.cn

[A10] 生成随机数
来源：http://wi.huixiangedu.cn

Py:   import random; random.randint(1, 100)
来源：http://cu.asd995.cn

PHP:  random_int(1, 100);
来源：http://en.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nm.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fx.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://ls.szsharing.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dd.colortex.cn

Ruby: rand(1..100)
来源：http://lp.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://fg.lnxyls.cn

[A11] 条件表达式（三元）
来源：http://ot.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://ru.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ns.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://wh.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://iu.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://ma.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vn.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kn.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://le.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://sq.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://md.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nr.bookmarksfly.cn

JS:   `Hello, ${name}!`
来源：http://gw.521024.cn

TS:   `Hello, ${name}!`
来源：http://hv.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://qz.bookmarksfly.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jc.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://ex.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://wm.shxzukj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kp.hahajie.cn

Py:   "第一行\n第二行"
来源：http://sr.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://jk.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://ve.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://ca.hahajie.cn

Java: "第一行\n第二行"
来源：http://jm.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://zy.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://tz.haigaiapp.cn

C#:   "第一行\n第二行"
来源：http://ra.huixiangedu.cn

[A14] 注释写法
来源：http://kn.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ox.lnxyls.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lc.521024.cn

JS:   // 单行；/* 多行 */
来源：http://lp.chemitech.net.cn

TS:   // 单行；/* 多行 */
来源：http://qu.szxytkj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ac.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://st.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zw.muxihuayi.cn

C#:   // 单行；/* 多行 */
来源：http://kb.lnxyls.cn

[A15] 空值判断与默认值
来源：http://sx.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://ci.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://lk.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://ci.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://im.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xk.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://mj.asd995.cn

Ruby: value = data || "默认值"
来源：http://nx.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://mh.9csxet.cn

[A16] 真假值判断规则
来源：http://tn.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vp.9csxet.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://af.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qr.huixiangedu.cn

TS:   if (!x) {}
来源：http://ct.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lz.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zj.yuntaijiaju.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xn.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://va.shxzukj.cn

[A17] 位运算
来源：http://qj.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bc.9csxet.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sh.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vx.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ze.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sm.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ww.asd995.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yd.newstarts.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kk.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://wl.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://ho.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://zh.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hi.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eb.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://bj.lnxyls.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://eh.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://fi.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://sx.muxihuayi.cn

[A19] 交换两个变量
来源：http://vs.bjjhwx.cn

Py:   a, b = b, a
来源：http://qa.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kk.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://nb.szsharing.cn

TS:   [a, b] = [b, a];
来源：http://me.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://jf.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://ho.hahajie.cn

Ruby: a, b = b, a
来源：http://ry.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://gm.nicolike.cn

[A20] 读取标准输入
来源：http://sp.asd995.cn

Py:   name = input("请输入：")
来源：http://nb.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rd.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cn.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://zc.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://ps.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ht.newstarts.cn

Ruby: gets.chomp
来源：http://qt.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://bk.nicolike.cn

[A21] 保留指定小数位输出
来源：http://xi.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://xv.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lv.9csxet.cn

JS:   (3.14159).toFixed(2)
来源：http://ev.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://sm.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://xf.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://el.huixiangedu.cn

Ruby: format("%.2f", 3.14159)
来源：http://js.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://gg.lnxyls.cn

[A22] 获取字符串长度
来源：http://df.shxzskj.cn

Py:   len(s)
来源：http://qy.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ti.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fd.hahajie.cn

TS:   s.length
来源：http://qc.muxihuayi.cn

Java: s.length()
来源：http://ci.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rn.huanxung.cn

Ruby: s.length
来源：http://vp.huixiangedu.cn

C#:   s.Length
来源：http://jc.hahajie.cn

[A23] 大小写转换
来源：http://hv.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rd.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yi.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wu.shxzukj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yi.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dm.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rw.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xb.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xg.szxytkj.cn

[A24] 去除首尾空白
来源：http://im.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vn.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sx.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mj.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://by.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qz.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://wp.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pg.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kt.szsharing.cn

[A25] 字符串比较
来源：http://jr.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://ne.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gc.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://un.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qn.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uf.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://du.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://me.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iw.szxytkj.cn

[A26] 类型转换总览
来源：http://oj.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mc.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uh.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ol.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://cd.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zs.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jk.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jb.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jn.jianghongdianzi.cn

================================================================================
来源：http://im.shtwfgs.cn

B. 流程控制
来源：http://dd.shxzskj.cn

================================================================================
来源：http://yi.szxytkj.cn

[B01] 条件判断 if / else
来源：http://yl.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gp.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cr.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bd.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aw.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ur.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lj.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lf.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bj.nicolike.cn

[B02] 多分支 else if / elif
来源：http://yh.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dk.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mj.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ex.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jn.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hn.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kk.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ib.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vc.szsharing.cn

[B03] switch / match / case
来源：http://rt.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ux.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mi.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vm.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gu.hnjuh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qt.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cu.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qg.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wi.lnxyls.cn

[B04] for 计数循环
来源：http://wr.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://if.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gy.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qb.9csxet.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ax.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://id.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dc.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://rr.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pw.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://ll.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://vf.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://im.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fq.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yb.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mu.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rs.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://cf.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bb.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://vf.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uz.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zg.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://se.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://li.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pc.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yr.hnjuh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ob.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://si.nicolike.cn

[B07] while 循环
来源：http://zu.newstarts.cn

Py:   while i < 10: i += 1
来源：http://hf.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wd.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://km.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://uf.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://tv.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xc.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://mr.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://dv.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://od.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://ah.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://iw.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://zb.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://ha.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://up.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://it.lnxyls.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gk.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://qw.nszjky.cn

[B09] break 与 continue
来源：http://uh.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dw.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nz.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ga.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aq.shtwfgs.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dw.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jc.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nq.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ax.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://qv.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jn.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cx.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bw.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gy.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fk.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sb.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kc.chemitech.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ya.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://ld.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://gr.huanxung.cn

PHP:  range(0, 10, 2);
来源：http://qv.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qu.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zh.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ke.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qg.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://ao.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gz.muxihuayi.cn

[B12] 跳出多层循环
来源：http://nd.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ct.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://el.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cq.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vl.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hs.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ki.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qi.nszjky.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zz.gzmigu.cn

[B13] 判断是否为数字
来源：http://ca.521024.cn

Py:   isinstance(x, (int, float))
来源：http://wq.szxytkj.cn

PHP:  is_numeric($x)
来源：http://iq.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ee.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yb.bookmarksfly.cn

Java: x instanceof Number
来源：http://qo.bookmarksfly.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nu.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://ey.szsharing.cn

C#:   x is int or double or decimal
来源：http://ir.9csxet.cn

[B14] 判断值是否在集合内
来源：http://ne.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sd.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pf.colortex.cn


<!-- 参考信息 -->