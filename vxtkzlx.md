代发 wailian999

Py:   print("Hello, World!")
来源：http://pj.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://sl.shtwfgs.cn

JS:   console.log("Hello, World!");
来源：http://nd.colortex.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xl.szxytkj.cn

Java: System.out.println("Hello, World!");
来源：http://ro.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://ct.colortex.cn

Ruby: puts "Hello, World!"
来源：http://fr.jianghongdianzi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cm.hahajie.cn

[A02] 变量声明与赋值
来源：http://va.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dk.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xu.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://re.muxihuayi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ru.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://po.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://wl.newstarts.cn

Ruby: name = "Alex"; age = 20
来源：http://qv.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zo.hahajie.cn

[A03] 常量定义
来源：http://on.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ir.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://we.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://of.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://jv.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://eq.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://sd.hnjuh.cn

Ruby: PI = 3.14159
来源：http://wu.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://co.jctech888.com.cn

[A04] 判断变量类型
来源：http://wl.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vo.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://df.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hk.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://tg.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ou.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ft.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://go.asd995.cn

C#:   x.GetType().Name; x is int
来源：http://st.muxihuayi.cn

[A05] 整数除法与取模
来源：http://iw.521024.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ri.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jj.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tb.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ii.shxzukj.cn

Java: 7 / 2; 7 % 2
来源：http://wa.gzmigu.cn

Go:   7 / 2; 7 % 2
来源：http://yo.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://jf.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://ff.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://mt.jianghongdianzi.cn

Py:   int("42"); float("3.14")
来源：http://qy.shxzskj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jj.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ft.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wl.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sv.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hs.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://te.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://le.huanxung.cn

[A07] 数字转字符串
来源：http://jx.hahajie.cn

Py:   str(42)
来源：http://ve.nicolike.cn

PHP:  (string) 42; strval(42)
来源：http://ne.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://ev.shtwfgs.cn

TS:   String(42)
来源：http://mz.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bj.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://cq.huanxung.cn

Ruby: 42.to_s
来源：http://cn.yuexingan06.cn

C#:   42.ToString()
来源：http://ud.asd995.cn

[A08] 取整与四舍五入
来源：http://cs.haigaiapp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rj.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://id.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://at.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wf.jctech888.com.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wy.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yj.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cg.yuexingan06.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rc.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://ee.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eg.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gs.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mc.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vz.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fo.haigaiapp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iu.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gs.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kz.lnxyls.cn

[A10] 生成随机数
来源：http://pt.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://ao.nicolike.cn

PHP:  random_int(1, 100);
来源：http://xg.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://se.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nk.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://ru.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jx.asd995.cn

Ruby: rand(1..100)
来源：http://sm.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://ld.9csxet.cn

[A11] 条件表达式（三元）
来源：http://zp.nicolike.cn

Py:   "yes" if x > 0 else "no"
来源：http://mt.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yh.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xn.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ng.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://ol.huixinmuqiang.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tp.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ye.shxzukj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://dq.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://wu.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://iv.shxzukj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sd.hnjuh.cn

JS:   `Hello, ${name}!`
来源：http://ay.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://qi.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://qc.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eb.gzmigu.cn

Ruby: "Hello, #{name}!"
来源：http://xh.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://vq.muxihuayi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ig.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://di.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://bp.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://ff.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://my.colortex.cn

Java: "第一行\n第二行"
来源：http://ev.colortex.cn

Go:   "第一行\n第二行"
来源：http://ep.shxzskj.cn

Ruby: "第一行\n第二行"
来源：http://tr.9csxet.cn

C#:   "第一行\n第二行"
来源：http://jc.huanxung.cn

[A14] 注释写法
来源：http://ct.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ke.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ho.huanxung.cn

JS:   // 单行；/* 多行 */
来源：http://oo.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://xp.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cw.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://tb.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mk.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://mt.shtwfgs.cn

[A15] 空值判断与默认值
来源：http://cx.shxzukj.cn

Py:   value = data or "默认值"
来源：http://fx.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://lm.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://ro.521024.cn

TS:   const value = data ?? "默认值";
来源：http://js.wgjwhj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gl.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://xm.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://vc.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://fu.nicolike.cn

[A16] 真假值判断规则
来源：http://es.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wf.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://px.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hc.hahajie.cn

TS:   if (!x) {}
来源：http://kt.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uq.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xn.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cg.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ol.jctech888.com.cn

[A17] 位运算
来源：http://ce.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hq.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bk.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yz.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mb.jctech888.com.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ww.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jm.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ml.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gr.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://py.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://ts.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://lr.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jm.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://os.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://fm.huixiangedu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://eg.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://ug.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://xj.shxzskj.cn

[A19] 交换两个变量
来源：http://by.wgjwhj.cn

Py:   a, b = b, a
来源：http://wu.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fu.hahajie.cn

JS:   [a, b] = [b, a];
来源：http://mr.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://cb.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://du.nicolike.cn

Go:   a, b = b, a
来源：http://gw.yuexingan06.cn

Ruby: a, b = b, a
来源：http://cp.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://zl.lnxyls.cn

[A20] 读取标准输入
来源：http://ec.panjiajie.cn

Py:   name = input("请输入：")
来源：http://pt.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sg.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mc.shxzukj.cn

TS:   // Node.js：readline 模块
来源：http://cx.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://lv.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bu.szxytkj.cn

Ruby: gets.chomp
来源：http://ye.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://of.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://wd.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://pj.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rn.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://zq.szsharing.cn

TS:   (3.14159).toFixed(2)
来源：http://rk.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://mp.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://md.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://ni.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://yy.shxzskj.cn

[A22] 获取字符串长度
来源：http://of.gzmigu.cn

Py:   len(s)
来源：http://gj.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tk.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gh.jianghongdianzi.cn

TS:   s.length
来源：http://ab.shxzukj.cn

Java: s.length()
来源：http://wm.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ot.muxihuayi.cn

Ruby: s.length
来源：http://fz.haigaiapp.cn

C#:   s.Length
来源：http://zv.nicolike.cn

[A23] 大小写转换
来源：http://ji.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ah.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pj.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ro.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ww.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fx.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hl.panjiajie.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gl.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jz.chemitech.net.cn

[A24] 去除首尾空白
来源：http://ch.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tb.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qu.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zo.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kz.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tu.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://go.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wt.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cx.asd995.cn

[A25] 字符串比较
来源：http://xa.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://sd.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uq.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zw.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dk.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nf.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iq.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fz.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vx.shtwfgs.cn

[A26] 类型转换总览
来源：http://md.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eb.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oz.haigaiapp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://do.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://wx.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vw.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tu.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tn.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://av.huanxung.cn

================================================================================
来源：http://uh.jianghongdianzi.cn

B. 流程控制
来源：http://hk.newstarts.cn

================================================================================
来源：http://ss.gzmigu.cn

[B01] 条件判断 if / else
来源：http://fw.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mu.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fl.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hs.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vr.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ib.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jk.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ex.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hg.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://cb.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ab.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://al.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ay.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pg.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://di.hahajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pp.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vv.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jp.newstarts.cn

[B03] switch / match / case
来源：http://ir.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yi.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cg.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wt.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://im.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pu.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dn.chemitech.net.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://js.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bu.nszjky.cn

[B04] for 计数循环
来源：http://im.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://jt.bjjhwx.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ie.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nb.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jc.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://di.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ro.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://ly.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ta.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://zj.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://ye.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gb.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://it.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rb.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xh.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ef.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://zb.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tf.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://lr.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ow.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jw.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hc.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gp.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jw.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vc.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mm.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fi.nicolike.cn

[B07] while 循环
来源：http://lp.haigaiapp.cn

Py:   while i < 10: i += 1
来源：http://gy.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://og.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://cu.chemitech.net.cn

TS:   while (i < 10) { i++; }
来源：http://kl.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://as.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ub.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://fm.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://ss.colortex.cn

[B08] do-while（至少执行一次）
来源：http://kn.hahajie.cn


<!-- 参考信息 -->