代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://nq.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qh.shtwfgs.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pi.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://te.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kj.chemitech.net.cn

[A07] 数字转字符串
来源：http://mt.szxytkj.cn

Py:   str(42)
来源：http://uq.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://lb.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://tm.haigaiapp.cn

TS:   String(42)
来源：http://ry.nicolike.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ke.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://rt.shxzskj.cn

Ruby: 42.to_s
来源：http://oq.yuexingan06.cn

C#:   42.ToString()
来源：http://tv.panjiajie.cn

[A08] 取整与四舍五入
来源：http://uc.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jp.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rb.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://at.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hj.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pe.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qg.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ms.huanxung.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bd.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://ys.szxytkj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fc.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kd.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kd.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oz.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yn.jctech888.com.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://np.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bj.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qa.muxihuayi.cn

[A10] 生成随机数
来源：http://bq.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://yi.nicolike.cn

PHP:  random_int(1, 100);
来源：http://ma.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bk.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tr.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://em.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gv.panjiajie.cn

Ruby: rand(1..100)
来源：http://rl.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://tk.newstarts.cn

[A11] 条件表达式（三元）
来源：http://lc.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://cc.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://iw.yuntaijiaju.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ez.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qq.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://vt.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://de.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ew.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zv.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://jw.huanxung.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ed.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zn.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://do.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://pe.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://ob.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xg.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://dc.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://wq.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tc.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://sl.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://yf.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://yk.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://uu.huanxung.cn

Java: "第一行\n第二行"
来源：http://pf.jianghongdianzi.cn

Go:   "第一行\n第二行"
来源：http://sd.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://ek.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://gu.haigaiapp.cn

[A14] 注释写法
来源：http://kv.hahajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zs.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mq.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://ht.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://uh.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ko.huanxung.cn

Go:   // 单行；/* 多行 */
来源：http://jg.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qe.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://tp.shtwfgs.cn

[A15] 空值判断与默认值
来源：http://tk.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://qy.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://me.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://mo.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://rp.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ib.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://jw.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://bz.lnxyls.cn

C#:   var value = data ?? "默认值";
来源：http://gl.yuexingan06.cn

[A16] 真假值判断规则
来源：http://zw.jianghongdianzi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fw.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xn.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vd.colortex.cn

TS:   if (!x) {}
来源：http://cb.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fe.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ga.panjiajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sq.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://er.bjjhwx.cn

[A17] 位运算
来源：http://yk.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vp.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sy.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hx.lnxyls.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qi.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://as.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pf.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pl.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yy.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://bj.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://nz.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://wn.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vi.szsharing.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xo.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://do.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://eu.nicolike.cn

Ruby: "A".ord; 65.chr
来源：http://xy.colortex.cn

C#:   (int)'A'; (char)65
来源：http://ka.huixiangedu.cn

[A19] 交换两个变量
来源：http://ha.bookmarksfly.cn

Py:   a, b = b, a
来源：http://xd.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yf.huixiangedu.cn

JS:   [a, b] = [b, a];
来源：http://nj.szsharing.cn

TS:   [a, b] = [b, a];
来源：http://al.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://zj.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://yn.shtwfgs.cn

Ruby: a, b = b, a
来源：http://mz.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://zr.shtwfgs.cn

[A20] 读取标准输入
来源：http://wr.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://np.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fm.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lv.521024.cn

TS:   // Node.js：readline 模块
来源：http://zr.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://gz.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ck.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://eb.lnxyls.cn

C#:   Console.ReadLine();
来源：http://lc.nszjky.cn

[A21] 保留指定小数位输出
来源：http://ns.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://wl.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nz.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://zf.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://zn.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://xs.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lj.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://pi.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://bo.huanxung.cn

[A22] 获取字符串长度
来源：http://ks.huixiangedu.cn

Py:   len(s)
来源：http://le.newstarts.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qx.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mf.szsharing.cn

TS:   s.length
来源：http://ly.wgjwhj.cn

Java: s.length()
来源：http://qv.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://aq.nszjky.cn

Ruby: s.length
来源：http://rz.bjjhwx.cn

C#:   s.Length
来源：http://da.521024.cn

[A23] 大小写转换
来源：http://hm.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xb.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nc.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://im.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jx.shxzskj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nv.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pr.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ev.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tj.nicolike.cn

[A24] 去除首尾空白
来源：http://ks.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eb.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pk.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yc.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eo.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mf.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://it.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sn.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gq.jctech888.com.cn

[A25] 字符串比较
来源：http://xo.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://tl.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ot.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://re.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dc.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zz.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pf.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://po.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xc.muxihuayi.cn

[A26] 类型转换总览
来源：http://em.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sg.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ai.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gl.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://aw.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vn.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dj.hnjuh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bq.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://co.yuexingan06.cn

================================================================================
来源：http://va.shxzskj.cn

B. 流程控制
来源：http://zl.asd995.cn

================================================================================
来源：http://mk.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://uj.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gi.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iy.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gh.huanxung.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ez.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mm.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qy.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ml.shtwfgs.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aw.nicolike.cn

[B02] 多分支 else if / elif
来源：http://gp.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ds.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pe.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lz.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rk.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yp.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nt.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rn.jctech888.com.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jm.chemitech.net.cn

[B03] switch / match / case
来源：http://qu.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nf.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xg.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jp.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gy.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://im.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://va.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qd.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nm.bookmarksfly.cn

[B04] for 计数循环
来源：http://ex.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://ux.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jo.wgjwhj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mh.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qp.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tc.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://af.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://rs.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ww.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://rb.newstarts.cn

Py:   for item in arr: print(item)
来源：http://yr.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ak.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lk.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oa.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://uf.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://un.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://uk.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://li.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://vo.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sj.shxzskj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dq.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qf.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://np.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yg.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xu.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fk.chemitech.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yt.hnjuh.cn

[B07] while 循环
来源：http://os.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://pc.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qp.bjjhwx.cn

JS:   while (i < 10) { i++; }
来源：http://xq.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://by.521024.cn

Java: while (i < 10) { i++; }
来源：http://gt.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gm.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://ml.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://df.jctech888.com.cn

[B08] do-while（至少执行一次）
来源：http://np.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://fm.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rs.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://zk.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://op.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://cj.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://tf.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vz.yuntaijiaju.cn

C#:   do { i++; } while (i < 10);
来源：http://gh.shtwfgs.cn

[B09] break 与 continue
来源：http://os.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qq.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mu.nszjky.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ou.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yp.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wd.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vi.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ex.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xn.asd995.cn

[B10] 遍历同时拿索引
来源：http://kc.bjjhwx.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iu.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ac.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mh.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sk.shxzukj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ge.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bi.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://co.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vb.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://eh.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://fr.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://hn.nicolike.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zn.hnjuh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jv.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ic.colortex.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kb.colortex.cn

Ruby: (0...10).step(2).to_a
来源：http://um.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nc.9csxet.cn

[B12] 跳出多层循环
来源：http://fp.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uc.9csxet.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bd.asd995.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jz.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wh.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wc.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ot.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hg.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fy.hahajie.cn

[B13] 判断是否为数字
来源：http://fm.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://ac.bjjhwx.cn

PHP:  is_numeric($x)
来源：http://yy.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://co.yuntaijiaju.cn


<!-- 参考信息 -->