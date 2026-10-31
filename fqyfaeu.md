代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://zm.nicolike.cn

Go:   fmt.Println("Hello, World!")
来源：http://tj.asd995.cn

Ruby: puts "Hello, World!"
来源：http://xt.huixiangedu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://tq.lnxyls.cn

[A02] 变量声明与赋值
来源：http://ji.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ww.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://na.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qd.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kz.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://ma.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://uv.huixiangedu.cn

Ruby: name = "Alex"; age = 20
来源：http://xw.wgjwhj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nw.nicolike.cn

[A03] 常量定义
来源：http://xi.panjiajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jt.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://lh.521024.cn

JS:   const PI = 3.14159;
来源：http://bg.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://yx.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://oq.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://xd.nicolike.cn

Ruby: PI = 3.14159
来源：http://zb.521024.cn

C#:   const double PI = 3.14159;
来源：http://ow.hahajie.cn

[A04] 判断变量类型
来源：http://sv.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dk.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mc.colortex.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zq.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://is.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ql.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ap.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pb.yuexingan06.cn

C#:   x.GetType().Name; x is int
来源：http://bq.521024.cn

[A05] 整数除法与取模
来源：http://sq.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zk.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://au.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://um.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gf.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://ez.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://cw.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://me.shxzskj.cn

C#:   7 / 2; 7 % 2
来源：http://we.szxytkj.cn

[A06] 字符串转数字
来源：http://px.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://cs.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://iu.shxzukj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wd.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mt.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://na.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tq.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://cv.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yu.shxzukj.cn

[A07] 数字转字符串
来源：http://sq.shtwfgs.cn

Py:   str(42)
来源：http://hc.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://ya.panjiajie.cn

JS:   String(42); (42).toString()
来源：http://ee.lnxyls.cn

TS:   String(42)
来源：http://bw.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://td.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://cg.nicolike.cn

Ruby: 42.to_s
来源：http://dw.bjjhwx.cn

C#:   42.ToString()
来源：http://di.asd995.cn

[A08] 取整与四舍五入
来源：http://go.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wm.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ip.bjjhwx.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sp.muxihuayi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gl.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tx.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ol.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hl.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uh.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://sj.hahajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://aq.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hf.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mz.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cj.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mh.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kn.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lm.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xk.haigaiapp.cn

[A10] 生成随机数
来源：http://qh.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://if.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://jn.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pk.bookmarksfly.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://og.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://we.nszjky.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dx.nicolike.cn

Ruby: rand(1..100)
来源：http://lb.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://ef.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://cu.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://wb.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gl.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vj.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lq.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://hx.shxzskj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vs.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rx.huixiangedu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yy.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://hg.bjjhwx.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cg.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hd.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://hi.521024.cn

TS:   `Hello, ${name}!`
来源：http://nt.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://ah.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mj.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://bm.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://gl.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gn.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://nd.521024.cn

PHP:  "第一行\n第二行"
来源：http://ff.hahajie.cn

JS:   "第一行\n第二行"
来源：http://vz.colortex.cn

TS:   "第一行\n第二行"
来源：http://sp.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://wo.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://zz.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://qt.nicolike.cn

C#:   "第一行\n第二行"
来源：http://ni.yuexingan06.cn

[A14] 注释写法
来源：http://yb.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pw.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tw.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://zw.chemitech.net.cn

TS:   // 单行；/* 多行 */
来源：http://of.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sw.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://nu.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dn.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://fy.nicolike.cn

[A15] 空值判断与默认值
来源：http://rx.huixiangedu.cn

Py:   value = data or "默认值"
来源：http://rx.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://bu.bookmarksfly.cn

JS:   const value = data ?? "默认值";
来源：http://lx.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://ao.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yt.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://bi.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://og.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://bm.hahajie.cn

[A16] 真假值判断规则
来源：http://lh.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zd.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ov.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://do.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://wp.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mt.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ch.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://io.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ol.huixinmuqiang.cn

[A17] 位运算
来源：http://wd.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pb.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gn.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sa.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dn.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xc.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pv.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bj.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://by.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://jc.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://kc.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://pm.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://il.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tk.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://qs.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tr.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://ag.521024.cn

C#:   (int)'A'; (char)65
来源：http://mu.hnjuh.cn

[A19] 交换两个变量
来源：http://bn.nszjky.cn

Py:   a, b = b, a
来源：http://re.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ae.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://px.bookmarksfly.cn

TS:   [a, b] = [b, a];
来源：http://bq.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://cc.nszjky.cn

Go:   a, b = b, a
来源：http://it.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://bn.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://xf.szsharing.cn

[A20] 读取标准输入
来源：http://el.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://uf.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bl.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fn.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://rb.shtwfgs.cn

Java: new Scanner(System.in).nextLine()
来源：http://ca.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vd.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://ae.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://bl.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://dq.szsharing.cn

Py:   f"{3.14159:.2f}"
来源：http://an.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nz.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://ba.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://ss.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://re.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vp.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://cp.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://mc.chemitech.net.cn

[A22] 获取字符串长度
来源：http://od.shxzskj.cn

Py:   len(s)
来源：http://po.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gz.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gk.bookmarksfly.cn

TS:   s.length
来源：http://pd.huixinmuqiang.cn

Java: s.length()
来源：http://co.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mt.lnxyls.cn

Ruby: s.length
来源：http://io.nszjky.cn

C#:   s.Length
来源：http://gj.huanxung.cn

[A23] 大小写转换
来源：http://dd.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ny.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iv.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kl.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ut.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jf.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bt.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://aa.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rt.shtwfgs.cn

[A24] 去除首尾空白
来源：http://rh.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cm.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rp.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ef.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rm.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ny.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://bg.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jg.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cn.huanxung.cn

[A25] 字符串比较
来源：http://wx.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://nn.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ia.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pc.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fy.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ko.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ek.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zn.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://az.shxzukj.cn

[A26] 类型转换总览
来源：http://ez.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dq.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ge.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://qm.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jb.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hf.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ui.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ga.yuntaijiaju.cn

================================================================================
来源：http://zi.muxihuayi.cn

B. 流程控制
来源：http://uy.nszjky.cn

================================================================================
来源：http://hu.panjiajie.cn

[B01] 条件判断 if / else
来源：http://td.gzmigu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xe.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yv.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kc.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wh.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wu.bookmarksfly.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://no.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vw.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ng.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://sn.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ki.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tu.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ln.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bw.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gv.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ly.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kn.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wi.newstarts.cn

[B03] switch / match / case
来源：http://hv.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sy.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kh.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oi.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uv.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://je.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sq.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cv.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zz.asd995.cn

[B04] for 计数循环
来源：http://ok.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://dz.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ut.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ek.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://br.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ss.yuntaijiaju.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ky.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://zb.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sc.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://kz.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://gl.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ut.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xn.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jo.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ic.yuexingan06.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://um.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://tj.szxytkj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hu.9csxet.cn

[B06] 遍历字典 / 对象
来源：http://oz.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vf.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zh.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ek.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yk.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qe.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zv.haigaiapp.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rb.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ra.yuntaijiaju.cn

[B07] while 循环
来源：http://ki.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://ti.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nj.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://iz.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://fa.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://nu.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ck.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://yv.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://lj.asd995.cn

[B08] do-while（至少执行一次）
来源：http://ri.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://vq.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ax.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://ym.bookmarksfly.cn

TS:   do { i++; } while (i < 10);
来源：http://ck.shxzskj.cn


<!-- 参考信息 -->