代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jm.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://po.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://cb.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://jh.colortex.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hx.lnxyls.cn

[A03] 常量定义
来源：http://hf.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zm.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://nh.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://cn.colortex.cn

TS:   const PI: number = 3.14159;
来源：http://fj.shxzskj.cn

Java: static final double PI = 3.14159;
来源：http://ou.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://qu.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://qm.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://vs.hnjuh.cn

[A04] 判断变量类型
来源：http://vy.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://kv.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fm.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fr.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://vq.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ex.chemitech.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://or.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sv.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://kk.9csxet.cn

[A05] 整数除法与取模
来源：http://ow.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sj.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ki.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ib.szsharing.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cg.jctech888.com.cn

Java: 7 / 2; 7 % 2
来源：http://vy.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://jm.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://yb.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://uk.9csxet.cn

[A06] 字符串转数字
来源：http://cq.panjiajie.cn

Py:   int("42"); float("3.14")
来源：http://ek.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zs.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ta.gzmigu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bw.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ma.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ii.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wx.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xh.hnjuh.cn

[A07] 数字转字符串
来源：http://xh.szsharing.cn

Py:   str(42)
来源：http://va.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://cr.hahajie.cn

JS:   String(42); (42).toString()
来源：http://au.hnjuh.cn

TS:   String(42)
来源：http://ss.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fk.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://rj.colortex.cn

Ruby: 42.to_s
来源：http://qr.panjiajie.cn

C#:   42.ToString()
来源：http://jg.lnxyls.cn

[A08] 取整与四舍五入
来源：http://zj.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zu.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ds.bjjhwx.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bf.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vg.huixiangedu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mu.colortex.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qi.shxzskj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xl.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://oy.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://ys.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hu.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dw.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pm.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sz.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ju.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tp.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ht.bjjhwx.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kn.nicolike.cn

[A10] 生成随机数
来源：http://aq.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://ny.bookmarksfly.cn

PHP:  random_int(1, 100);
来源：http://nq.shxzskj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jb.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ki.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://tx.shxzukj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://oj.szsharing.cn

Ruby: rand(1..100)
来源：http://dj.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://um.hahajie.cn

[A11] 条件表达式（三元）
来源：http://ps.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://ti.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gm.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jv.lnxyls.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sp.szsharing.cn

Java: x > 0 ? "yes" : "no"
来源：http://rk.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ee.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tw.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://yq.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ow.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dl.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://ms.gzmigu.cn

TS:   `Hello, ${name}!`
来源：http://ww.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://mu.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qh.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://cc.bjjhwx.cn

C#:   $"Hello, {name}!"
来源：http://an.bjjhwx.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oh.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://lx.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://be.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://mm.521024.cn

TS:   "第一行\n第二行"
来源：http://lt.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://mr.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://yk.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://cg.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://ae.shtwfgs.cn

[A14] 注释写法
来源：http://hm.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ws.hahajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lu.yuexingan06.cn

JS:   // 单行；/* 多行 */
来源：http://ce.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://qs.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oh.huixiangedu.cn

Go:   // 单行；/* 多行 */
来源：http://us.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rt.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://lk.szsharing.cn

[A15] 空值判断与默认值
来源：http://ar.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://tp.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://df.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://ym.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://ha.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mb.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://zy.9csxet.cn

Ruby: value = data || "默认值"
来源：http://yq.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://xs.huixiangedu.cn

[A16] 真假值判断规则
来源：http://wk.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wl.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ik.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tb.521024.cn

TS:   if (!x) {}
来源：http://wr.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jg.shxzskj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://li.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oh.hahajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ml.szsharing.cn

[A17] 位运算
来源：http://ri.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ng.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sz.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zj.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ml.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hf.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ir.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gy.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ew.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://nv.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://rk.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://va.gzmigu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bp.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yh.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://ep.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ty.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://wb.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://ea.nszjky.cn

[A19] 交换两个变量
来源：http://fs.jctech888.com.cn

Py:   a, b = b, a
来源：http://lq.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kk.521024.cn

JS:   [a, b] = [b, a];
来源：http://dj.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://jb.521024.cn

Java: int t = a; a = b; b = t;
来源：http://ko.szxytkj.cn

Go:   a, b = b, a
来源：http://sx.nicolike.cn

Ruby: a, b = b, a
来源：http://tg.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://bv.shtwfgs.cn

[A20] 读取标准输入
来源：http://hi.hahajie.cn

Py:   name = input("请输入：")
来源：http://xv.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kz.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rk.colortex.cn

TS:   // Node.js：readline 模块
来源：http://uv.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://yx.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xa.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://kq.asd995.cn

C#:   Console.ReadLine();
来源：http://jh.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://lb.huixiangedu.cn

Py:   f"{3.14159:.2f}"
来源：http://yd.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pq.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://hu.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://wp.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://pg.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ka.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://ar.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://by.colortex.cn

[A22] 获取字符串长度
来源：http://ts.colortex.cn

Py:   len(s)
来源：http://el.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ev.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bz.chemitech.net.cn

TS:   s.length
来源：http://go.hnjuh.cn

Java: s.length()
来源：http://rr.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kq.bjjhwx.cn

Ruby: s.length
来源：http://hn.bookmarksfly.cn

C#:   s.Length
来源：http://zg.colortex.cn

[A23] 大小写转换
来源：http://kp.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fw.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pl.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xe.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://li.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ma.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dn.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bw.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://am.colortex.cn

[A24] 去除首尾空白
来源：http://pl.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://su.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nw.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://to.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iv.yuntaijiaju.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pb.521024.cn

Go:   strings.TrimSpace(s)
来源：http://ld.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ds.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://im.gzmigu.cn

[A25] 字符串比较
来源：http://ax.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://vz.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hf.yuntaijiaju.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ls.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xa.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://br.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fk.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cl.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ld.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://oa.newstarts.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mo.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gm.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qo.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://oa.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lb.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kq.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://an.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ou.lnxyls.cn

================================================================================
来源：http://cg.lnxyls.cn

B. 流程控制
来源：http://zr.haigaiapp.cn

================================================================================
来源：http://fj.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://kt.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kd.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vb.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ok.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qr.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vo.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kt.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qu.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hr.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://rd.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gx.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fc.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qf.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zh.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ps.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dv.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xr.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gj.huixinmuqiang.cn

[B03] switch / match / case
来源：http://ig.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kd.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eb.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://je.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ui.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gw.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hl.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mf.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://av.gzmigu.cn

[B04] for 计数循环
来源：http://sg.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://wg.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vj.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ss.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ju.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tu.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zo.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://mi.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pq.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://wc.521024.cn

Py:   for item in arr: print(item)
来源：http://om.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ly.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://en.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pi.wgjwhj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bc.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kj.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://rg.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ms.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://we.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gl.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tt.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cf.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://za.bookmarksfly.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hk.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uu.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wp.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xw.bjjhwx.cn

[B07] while 循环
来源：http://in.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://zi.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dk.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://kl.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://ai.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://sa.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lv.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://en.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://fm.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://gu.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://yp.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xh.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://ev.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://xp.huanxung.cn

Java: do { i++; } while (i < 10);
来源：http://mv.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ti.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cd.shxzskj.cn

C#:   do { i++; } while (i < 10);
来源：http://af.shxzukj.cn

[B09] break 与 continue
来源：http://ut.jianghongdianzi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rn.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kw.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://el.bookmarksfly.cn


<!-- 参考信息 -->