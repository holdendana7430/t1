代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://bv.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xs.bjjhwx.cn

C#:   x.GetType().Name; x is int
来源：http://ra.asd995.cn

[A05] 整数除法与取模
来源：http://ao.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qm.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://uh.chemitech.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vh.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yi.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://xp.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://ib.jctech888.com.cn

Ruby: 7 / 2; 7 % 2
来源：http://xp.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://ev.huanxung.cn

[A06] 字符串转数字
来源：http://kr.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://tn.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://og.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qc.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://er.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kj.muxihuayi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wk.521024.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zn.9csxet.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ip.asd995.cn

[A07] 数字转字符串
来源：http://sn.chemitech.net.cn

Py:   str(42)
来源：http://li.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://qe.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://in.chemitech.net.cn

TS:   String(42)
来源：http://eg.shxzukj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ez.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://ly.nszjky.cn

Ruby: 42.to_s
来源：http://vv.asd995.cn

C#:   42.ToString()
来源：http://qh.asd995.cn

[A08] 取整与四舍五入
来源：http://cb.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pg.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zv.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gb.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ex.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://en.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xc.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ph.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bc.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://bt.lnxyls.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eu.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://al.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fs.hahajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nc.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mv.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vc.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rk.szxytkj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qk.huanxung.cn

[A10] 生成随机数
来源：http://np.newstarts.cn

Py:   import random; random.randint(1, 100)
来源：http://vf.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://xr.hnjuh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jd.hnjuh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ap.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://tu.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hk.jctech888.com.cn

Ruby: rand(1..100)
来源：http://bg.9csxet.cn

C#:   new Random().Next(1, 101)
来源：http://qp.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://dg.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://nv.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xp.jctech888.com.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kk.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ic.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://ob.huixiangedu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xo.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://uq.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zr.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://gu.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nf.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wq.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://ge.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://uz.panjiajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://ib.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lq.yuexingan06.cn

Ruby: "Hello, #{name}!"
来源：http://vx.asd995.cn

C#:   $"Hello, {name}!"
来源：http://ga.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rf.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://cs.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://ko.szxytkj.cn

JS:   "第一行\n第二行"
来源：http://yo.huixinmuqiang.cn

TS:   "第一行\n第二行"
来源：http://xt.hnjuh.cn

Java: "第一行\n第二行"
来源：http://rq.shtwfgs.cn

Go:   "第一行\n第二行"
来源：http://kb.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://yu.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://sm.shxzukj.cn

[A14] 注释写法
来源：http://yy.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vv.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vb.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://mz.newstarts.cn

TS:   // 单行；/* 多行 */
来源：http://th.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qq.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://dp.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yk.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://pe.szsharing.cn

[A15] 空值判断与默认值
来源：http://oc.lnxyls.cn

Py:   value = data or "默认值"
来源：http://so.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://pz.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://ou.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://tz.yuexingan06.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zi.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://ww.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://ex.chemitech.net.cn

C#:   var value = data ?? "默认值";
来源：http://ff.nszjky.cn

[A16] 真假值判断规则
来源：http://xs.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mf.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://un.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zf.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://kc.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yh.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tk.szxytkj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hn.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fs.nszjky.cn

[A17] 位运算
来源：http://hr.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cc.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pz.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vd.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://we.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lp.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ia.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nq.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zh.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://tg.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://af.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://hg.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ha.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ko.hnjuh.cn

Java: (int) 'A'; (char) 65
来源：http://if.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mx.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://sm.gzmigu.cn

C#:   (int)'A'; (char)65
来源：http://ea.yuexingan06.cn

[A19] 交换两个变量
来源：http://fi.haigaiapp.cn

Py:   a, b = b, a
来源：http://ew.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ze.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://la.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://jd.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://dp.szsharing.cn

Go:   a, b = b, a
来源：http://md.asd995.cn

Ruby: a, b = b, a
来源：http://gg.asd995.cn

C#:   (a, b) = (b, a);
来源：http://cw.muxihuayi.cn

[A20] 读取标准输入
来源：http://ps.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://po.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yg.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wl.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://ks.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://po.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cu.yuexingan06.cn

Ruby: gets.chomp
来源：http://bn.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://ep.colortex.cn

[A21] 保留指定小数位输出
来源：http://et.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://jh.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://go.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://ox.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://jt.wgjwhj.cn

Java: String.format("%.2f", 3.14159)
来源：http://mo.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hu.gzmigu.cn

Ruby: format("%.2f", 3.14159)
来源：http://ez.muxihuayi.cn

C#:   3.14159.ToString("F2")
来源：http://db.nicolike.cn

[A22] 获取字符串长度
来源：http://nt.szxytkj.cn

Py:   len(s)
来源：http://vr.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rl.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cp.shxzskj.cn

TS:   s.length
来源：http://ed.hnjuh.cn

Java: s.length()
来源：http://rg.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://od.szsharing.cn

Ruby: s.length
来源：http://or.huixinmuqiang.cn

C#:   s.Length
来源：http://pv.gzmigu.cn

[A23] 大小写转换
来源：http://ki.chemitech.net.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sf.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gc.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lt.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://re.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ah.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://br.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fo.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ha.wgjwhj.cn

[A24] 去除首尾空白
来源：http://ws.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jz.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pu.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://or.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gs.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lo.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://mm.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ii.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ag.hahajie.cn

[A25] 字符串比较
来源：http://wc.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://uc.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://im.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hh.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xk.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://go.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qk.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fw.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://td.wgjwhj.cn

[A26] 类型转换总览
来源：http://hl.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sr.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ot.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qn.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://so.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ex.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sz.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sl.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ys.bookmarksfly.cn

================================================================================
来源：http://xb.panjiajie.cn

B. 流程控制
来源：http://ml.yuexingan06.cn

================================================================================
来源：http://ln.lnxyls.cn

[B01] 条件判断 if / else
来源：http://cl.szxytkj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hr.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://og.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zw.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://js.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fh.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ud.haigaiapp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uv.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ji.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://yf.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dq.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wj.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zl.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tk.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zb.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wr.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yx.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gx.gzmigu.cn

[B03] switch / match / case
来源：http://bi.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lb.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xf.asd995.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ej.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ny.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qf.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://am.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pf.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rv.521024.cn

[B04] for 计数循环
来源：http://ql.szxytkj.cn

Py:   for i in range(10): print(i)
来源：http://ij.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oh.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zo.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sj.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gk.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://go.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://da.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hn.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://go.nicolike.cn

Py:   for item in arr: print(item)
来源：http://ei.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gq.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jd.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lt.jctech888.com.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tv.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fb.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://tf.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vv.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://bm.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xa.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xa.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aj.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wu.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ai.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ge.huanxung.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ci.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iu.colortex.cn

[B07] while 循环
来源：http://pt.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://cy.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rh.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://tl.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://ye.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://kd.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sv.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://mw.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://qt.521024.cn

[B08] do-while（至少执行一次）
来源：http://gb.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://hx.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zh.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://cs.bjjhwx.cn

TS:   do { i++; } while (i < 10);
来源：http://at.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://rx.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gr.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cy.9csxet.cn

C#:   do { i++; } while (i < 10);
来源：http://er.nszjky.cn

[B09] break 与 continue
来源：http://ta.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gz.bjjhwx.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ks.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ki.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zo.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uv.shtwfgs.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eo.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fi.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cv.szsharing.cn

[B10] 遍历同时拿索引
来源：http://ja.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cd.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kc.nszjky.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://aj.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uw.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ko.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mz.hahajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://on.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://dp.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://gx.huixiangedu.cn

PHP:  range(0, 10, 2);
来源：http://mx.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tp.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zd.521024.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hr.hahajie.cn


<!-- 参考信息 -->