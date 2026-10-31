代发 wailian999

================================================================================
来源：http://ma.jctech888.com.cn

A. 基础语法与类型
来源：http://ej.shxzskj.cn

================================================================================
来源：http://bp.bookmarksfly.cn

[A01] Hello World
来源：http://pc.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://lv.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://dq.bjjhwx.cn

JS:   console.log("Hello, World!");
来源：http://ie.lnxyls.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yq.lnxyls.cn

Java: System.out.println("Hello, World!");
来源：http://xk.szxytkj.cn

Go:   fmt.Println("Hello, World!")
来源：http://sq.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://fs.wgjwhj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mo.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://ff.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hr.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hk.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vc.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kr.huanxung.cn

Java: String name = "Alex"; int age = 20;
来源：http://ci.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://py.hnjuh.cn

Ruby: name = "Alex"; age = 20
来源：http://wc.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vy.chemitech.net.cn

[A03] 常量定义
来源：http://vz.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wv.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://hl.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://dq.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://ml.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://dc.521024.cn

Go:   const PI = 3.14159
来源：http://eh.shxzukj.cn

Ruby: PI = 3.14159
来源：http://hk.huanxung.cn

C#:   const double PI = 3.14159;
来源：http://ee.bjjhwx.cn

[A04] 判断变量类型
来源：http://op.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xq.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mr.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bx.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://bt.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gz.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mm.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bn.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://gj.hnjuh.cn

[A05] 整数除法与取模
来源：http://cu.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gf.haigaiapp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kt.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cx.hnjuh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pc.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://gn.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://ac.bjjhwx.cn

Ruby: 7 / 2; 7 % 2
来源：http://cg.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://oy.shtwfgs.cn

[A06] 字符串转数字
来源：http://za.gzmigu.cn

Py:   int("42"); float("3.14")
来源：http://da.szsharing.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qb.huanxung.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ye.muxihuayi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tr.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sz.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://re.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wf.bookmarksfly.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://di.bjjhwx.cn

[A07] 数字转字符串
来源：http://sn.muxihuayi.cn

Py:   str(42)
来源：http://ov.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://vj.nicolike.cn

JS:   String(42); (42).toString()
来源：http://db.shtwfgs.cn

TS:   String(42)
来源：http://uh.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rj.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://ea.hahajie.cn

Ruby: 42.to_s
来源：http://mg.huanxung.cn

C#:   42.ToString()
来源：http://kd.nszjky.cn

[A08] 取整与四舍五入
来源：http://zp.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ag.asd995.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vo.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zx.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uc.huanxung.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hn.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cu.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mw.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sf.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://wz.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tt.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pl.bookmarksfly.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mq.bjjhwx.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nd.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xq.panjiajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wo.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ez.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ec.lnxyls.cn

[A10] 生成随机数
来源：http://lg.szxytkj.cn

Py:   import random; random.randint(1, 100)
来源：http://my.nicolike.cn

PHP:  random_int(1, 100);
来源：http://bz.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jg.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mq.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://ib.muxihuayi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ny.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://rj.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://re.nszjky.cn

[A11] 条件表达式（三元）
来源：http://kb.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://ru.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tm.newstarts.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ty.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mt.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://hd.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://su.lnxyls.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://at.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mp.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://bv.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cd.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gb.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://pt.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://ml.asd995.cn

Java: "Hello, %s!".formatted(name)
来源：http://bh.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pn.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://yi.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://ep.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cs.nicolike.cn

Py:   "第一行\n第二行"
来源：http://ui.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://zn.nicolike.cn

JS:   "第一行\n第二行"
来源：http://jo.hahajie.cn

TS:   "第一行\n第二行"
来源：http://wj.szxytkj.cn

Java: "第一行\n第二行"
来源：http://tq.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://kt.muxihuayi.cn

Ruby: "第一行\n第二行"
来源：http://wo.szsharing.cn

C#:   "第一行\n第二行"
来源：http://bt.chemitech.net.cn

[A14] 注释写法
来源：http://ry.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hv.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://sd.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://rq.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://iz.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://jm.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mj.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://xu.szxytkj.cn

[A15] 空值判断与默认值
来源：http://bb.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://tc.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://qn.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://os.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://gu.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uo.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://uw.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://bu.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://ae.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://xr.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kk.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ix.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rm.wgjwhj.cn

TS:   if (!x) {}
来源：http://vb.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ld.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rm.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cr.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jt.521024.cn

[A17] 位运算
来源：http://ho.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kg.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nr.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xf.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ty.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ef.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pv.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dv.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://un.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://tw.521024.cn

Py:   ord("A"); chr(65)
来源：http://pg.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://ug.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mh.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zm.hnjuh.cn

Java: (int) 'A'; (char) 65
来源：http://hc.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mi.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://wo.colortex.cn

C#:   (int)'A'; (char)65
来源：http://aa.9csxet.cn

[A19] 交换两个变量
来源：http://bn.shtwfgs.cn

Py:   a, b = b, a
来源：http://ae.jianghongdianzi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ff.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://eb.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://pj.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://in.lnxyls.cn

Go:   a, b = b, a
来源：http://ya.panjiajie.cn

Ruby: a, b = b, a
来源：http://al.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://iw.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://zm.nicolike.cn

Py:   name = input("请输入：")
来源：http://tf.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ph.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qm.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://cp.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://ig.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ud.jctech888.com.cn

Ruby: gets.chomp
来源：http://ut.nicolike.cn

C#:   Console.ReadLine();
来源：http://yn.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://ia.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://mv.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dk.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://ge.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://zf.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://ni.bjjhwx.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pg.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://gt.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://me.nicolike.cn

[A22] 获取字符串长度
来源：http://up.nicolike.cn

Py:   len(s)
来源：http://ye.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ch.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rj.chemitech.net.cn

TS:   s.length
来源：http://cb.gzmigu.cn

Java: s.length()
来源：http://ij.nicolike.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uo.huixinmuqiang.cn

Ruby: s.length
来源：http://hc.yuntaijiaju.cn

C#:   s.Length
来源：http://nc.yuntaijiaju.cn

[A23] 大小写转换
来源：http://vp.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dd.bookmarksfly.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yr.wgjwhj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ol.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nv.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wt.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xf.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gt.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pl.jctech888.com.cn

[A24] 去除首尾空白
来源：http://ob.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://id.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fc.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sc.newstarts.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vs.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vv.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://rv.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cu.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ed.wgjwhj.cn

[A25] 字符串比较
来源：http://nm.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://ji.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://um.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ge.nicolike.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tl.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vz.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tr.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rb.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://um.yuexingan06.cn

[A26] 类型转换总览
来源：http://pi.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://aj.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ii.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://re.huanxung.cn

TS:   Number() String() Boolean() x as number
来源：http://pm.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ga.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ow.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://id.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uf.nicolike.cn

================================================================================
来源：http://hx.huixiangedu.cn

B. 流程控制
来源：http://gb.shxzukj.cn

================================================================================
来源：http://js.hnjuh.cn

[B01] 条件判断 if / else
来源：http://wy.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://if.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bz.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wq.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vs.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xa.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bv.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zm.9csxet.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tt.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://vu.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bj.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://km.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wb.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mb.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aw.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://de.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cb.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cv.bookmarksfly.cn

[B03] switch / match / case
来源：http://da.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ft.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jz.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sv.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nr.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tv.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pv.muxihuayi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yj.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vu.nicolike.cn

[B04] for 计数循环
来源：http://qw.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://hp.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bq.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vq.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cw.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://um.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cw.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://xz.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fx.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://ys.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://pr.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ju.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ok.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wy.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yq.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tq.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://pj.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ce.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://kk.9csxet.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lq.jctech888.com.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mh.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vn.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://df.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://af.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nn.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wu.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bs.shxzukj.cn

[B07] while 循环
来源：http://af.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://bn.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eh.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://ri.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://jw.asd995.cn

Java: while (i < 10) { i++; }
来源：http://rh.9csxet.cn


<!-- 参考信息 -->