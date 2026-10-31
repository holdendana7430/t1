代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ym.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bv.yuexingan06.cn

TS:   typeof x; x instanceof Date
来源：http://xx.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://am.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qp.gzmigu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cj.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://vg.asd995.cn

[A05] 整数除法与取模
来源：http://gy.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://in.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qj.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sc.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ki.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://ni.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://iy.chemitech.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://sa.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://dy.lnxyls.cn

[A06] 字符串转数字
来源：http://ak.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://nw.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xw.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ce.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ou.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ig.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hq.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kv.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fo.nicolike.cn

[A07] 数字转字符串
来源：http://oq.muxihuayi.cn

Py:   str(42)
来源：http://ej.521024.cn

PHP:  (string) 42; strval(42)
来源：http://zo.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://ek.szsharing.cn

TS:   String(42)
来源：http://cd.colortex.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nw.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://mn.shxzskj.cn

Ruby: 42.to_s
来源：http://it.9csxet.cn

C#:   42.ToString()
来源：http://so.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://wp.haigaiapp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mi.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tl.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zv.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xj.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kr.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rp.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://uq.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tw.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://so.bjjhwx.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://aq.9csxet.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yj.wgjwhj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hl.shxzskj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ws.szxytkj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wz.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ck.chemitech.net.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kc.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wq.haigaiapp.cn

[A10] 生成随机数
来源：http://au.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://ua.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://zh.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kd.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sr.jianghongdianzi.cn

Java: new Random().nextInt(100) + 1
来源：http://vp.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fc.chemitech.net.cn

Ruby: rand(1..100)
来源：http://zf.shtwfgs.cn

C#:   new Random().Next(1, 101)
来源：http://xw.9csxet.cn

[A11] 条件表达式（三元）
来源：http://bf.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://fy.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ap.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zz.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xe.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://ci.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://st.panjiajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://li.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://og.panjiajie.cn

[A12] 字符串插值 / 格式化
来源：http://dt.haigaiapp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pe.lnxyls.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://al.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://fe.asd995.cn

TS:   `Hello, ${name}!`
来源：http://ok.newstarts.cn

Java: "Hello, %s!".formatted(name)
来源：http://nf.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ov.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://bw.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://ws.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pe.huanxung.cn

Py:   "第一行\n第二行"
来源：http://no.chemitech.net.cn

PHP:  "第一行\n第二行"
来源：http://vi.wgjwhj.cn

JS:   "第一行\n第二行"
来源：http://ua.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://vp.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://lb.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://cb.shxzskj.cn

Ruby: "第一行\n第二行"
来源：http://tp.szxytkj.cn

C#:   "第一行\n第二行"
来源：http://gw.hnjuh.cn

[A14] 注释写法
来源：http://nb.hnjuh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cn.bookmarksfly.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bg.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://xl.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://dt.gzmigu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bq.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://og.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lz.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://uz.colortex.cn

[A15] 空值判断与默认值
来源：http://ug.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://aq.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://ci.haigaiapp.cn

JS:   const value = data ?? "默认值";
来源：http://ro.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://iq.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vr.szxytkj.cn

Go:   if data == "" { data = "默认值" }
来源：http://tv.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://dx.huixinmuqiang.cn

C#:   var value = data ?? "默认值";
来源：http://wo.szsharing.cn

[A16] 真假值判断规则
来源：http://ac.huixinmuqiang.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ed.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mz.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tv.jianghongdianzi.cn

TS:   if (!x) {}
来源：http://md.521024.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fm.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wk.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nc.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fv.hnjuh.cn

[A17] 位运算
来源：http://fr.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vc.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vq.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kr.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yu.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gt.lnxyls.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://le.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oa.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ho.jctech888.com.cn

[A18] 字符与 ASCII 码互转
来源：http://cy.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://hz.hahajie.cn

PHP:  ord("A"); chr(65)
来源：http://fp.bjjhwx.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qj.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bb.521024.cn

Java: (int) 'A'; (char) 65
来源：http://xu.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tb.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://do.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://we.shxzukj.cn

[A19] 交换两个变量
来源：http://yf.szxytkj.cn

Py:   a, b = b, a
来源：http://pl.shtwfgs.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vw.colortex.cn

JS:   [a, b] = [b, a];
来源：http://jr.asd995.cn

TS:   [a, b] = [b, a];
来源：http://sf.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://hc.yuexingan06.cn

Go:   a, b = b, a
来源：http://gb.9csxet.cn

Ruby: a, b = b, a
来源：http://nv.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://ta.shtwfgs.cn

[A20] 读取标准输入
来源：http://ts.szsharing.cn

Py:   name = input("请输入：")
来源：http://qb.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jk.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gp.521024.cn

TS:   // Node.js：readline 模块
来源：http://lp.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://ls.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ed.huixiangedu.cn

Ruby: gets.chomp
来源：http://dv.gzmigu.cn

C#:   Console.ReadLine();
来源：http://mt.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://xs.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://pe.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://or.9csxet.cn

JS:   (3.14159).toFixed(2)
来源：http://zo.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://eg.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://th.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ru.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://vc.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://no.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://jo.newstarts.cn

Py:   len(s)
来源：http://wd.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ik.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ux.hahajie.cn

TS:   s.length
来源：http://yv.huanxung.cn

Java: s.length()
来源：http://df.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qt.lnxyls.cn

Ruby: s.length
来源：http://ea.newstarts.cn

C#:   s.Length
来源：http://sb.szxytkj.cn

[A23] 大小写转换
来源：http://sp.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vo.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sj.lnxyls.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://it.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hf.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cy.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lt.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mm.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rb.bjjhwx.cn

[A24] 去除首尾空白
来源：http://el.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xg.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vf.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yb.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fa.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gv.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://mm.shxzskj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ym.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fl.muxihuayi.cn

[A25] 字符串比较
来源：http://pm.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://mj.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nn.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jl.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ot.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eh.asd995.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ef.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tp.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xp.colortex.cn

[A26] 类型转换总览
来源：http://rm.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cd.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gm.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ve.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://sp.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bm.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wt.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ns.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tq.shtwfgs.cn

================================================================================
来源：http://cb.chemitech.net.cn

B. 流程控制
来源：http://va.huixinmuqiang.cn

================================================================================
来源：http://ya.shxzskj.cn

[B01] 条件判断 if / else
来源：http://yc.shxzskj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tj.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ez.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fh.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fb.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hh.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pm.huanxung.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jh.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yo.521024.cn

[B02] 多分支 else if / elif
来源：http://al.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://if.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xb.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vs.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xu.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tk.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wk.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uz.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jm.muxihuayi.cn

[B03] switch / match / case
来源：http://ot.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gs.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bq.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mq.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mt.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qw.shxzskj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yu.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pc.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nb.lnxyls.cn

[B04] for 计数循环
来源：http://mu.colortex.cn

Py:   for i in range(10): print(i)
来源：http://zr.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tb.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gh.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gp.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://me.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zl.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://ty.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zi.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://tu.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://ls.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kx.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ty.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zz.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ts.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yz.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://lu.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kj.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://xa.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rt.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fk.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dw.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ky.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bm.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hg.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sa.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eu.yuexingan06.cn

[B07] while 循环
来源：http://sr.hahajie.cn

Py:   while i < 10: i += 1
来源：http://wt.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jg.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://la.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://cp.bookmarksfly.cn

Java: while (i < 10) { i++; }
来源：http://wh.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ug.szxytkj.cn

Ruby: while i < 10; i += 1; end
来源：http://ng.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://hp.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://eq.hahajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://jq.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ge.chemitech.net.cn

JS:   do { i++; } while (i < 10);
来源：http://wp.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://kx.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://xf.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jz.panjiajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dh.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://df.bjjhwx.cn

[B09] break 与 continue
来源：http://or.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hn.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xw.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sy.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dh.bookmarksfly.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hr.szsharing.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cy.yuexingan06.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ul.yuexingan06.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tt.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://kh.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iv.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nk.szxytkj.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rt.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sn.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://of.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://li.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fg.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wr.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://px.bjjhwx.cn

Py:   list(range(0, 10, 2))
来源：http://ca.gzmigu.cn


<!-- 参考信息 -->