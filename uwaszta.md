代发 wailian999

Py:   print("Hello, World!")
来源：http://xt.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://uw.gzmigu.cn

JS:   console.log("Hello, World!");
来源：http://my.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xv.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://jp.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://ya.bookmarksfly.cn

Ruby: puts "Hello, World!"
来源：http://rz.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ch.asd995.cn

[A02] 变量声明与赋值
来源：http://ef.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ae.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gq.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mg.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pw.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://um.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://fv.bjjhwx.cn

Ruby: name = "Alex"; age = 20
来源：http://fm.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yo.colortex.cn

[A03] 常量定义
来源：http://fy.hnjuh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://eh.jctech888.com.cn

PHP:  const PI = 3.14159;
来源：http://vq.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://rm.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://sl.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://cf.huanxung.cn

Go:   const PI = 3.14159
来源：http://zf.nszjky.cn

Ruby: PI = 3.14159
来源：http://ww.nicolike.cn

C#:   const double PI = 3.14159;
来源：http://nk.chemitech.net.cn

[A04] 判断变量类型
来源：http://iy.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cp.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mv.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gq.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://ti.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wr.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gt.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vf.haigaiapp.cn

C#:   x.GetType().Name; x is int
来源：http://xm.hnjuh.cn

[A05] 整数除法与取模
来源：http://wx.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lr.yuntaijiaju.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ww.bookmarksfly.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xx.bookmarksfly.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ze.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://bf.gzmigu.cn

Go:   7 / 2; 7 % 2
来源：http://hc.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://qb.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://cq.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://fq.nszjky.cn

Py:   int("42"); float("3.14")
来源：http://ec.hahajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://re.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hi.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zw.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cy.yuntaijiaju.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tc.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://iv.hahajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://us.9csxet.cn

[A07] 数字转字符串
来源：http://rm.wgjwhj.cn

Py:   str(42)
来源：http://jg.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://us.asd995.cn

JS:   String(42); (42).toString()
来源：http://as.haigaiapp.cn

TS:   String(42)
来源：http://vp.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wj.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://qs.muxihuayi.cn

Ruby: 42.to_s
来源：http://cl.haigaiapp.cn

C#:   42.ToString()
来源：http://el.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://kw.haigaiapp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ht.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nd.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ie.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://br.shtwfgs.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zs.gzmigu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ku.nszjky.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ge.wgjwhj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tg.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://kq.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hh.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lo.lnxyls.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xo.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dt.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jv.szsharing.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iw.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yd.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wd.newstarts.cn

[A10] 生成随机数
来源：http://rf.bookmarksfly.cn

Py:   import random; random.randint(1, 100)
来源：http://ku.huixinmuqiang.cn

PHP:  random_int(1, 100);
来源：http://ec.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ce.chemitech.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dd.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://ap.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xc.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://lt.hnjuh.cn

C#:   new Random().Next(1, 101)
来源：http://un.gzmigu.cn

[A11] 条件表达式（三元）
来源：http://rb.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://lh.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gj.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mh.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hp.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://wv.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://la.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gv.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qo.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://th.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ys.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jr.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://xs.lnxyls.cn

TS:   `Hello, ${name}!`
来源：http://dg.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://bs.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xm.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://gg.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://vf.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ru.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://mr.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://zq.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://sl.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://cy.521024.cn

Java: "第一行\n第二行"
来源：http://uj.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://ob.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://ww.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://rr.bjjhwx.cn

[A14] 注释写法
来源：http://dk.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ze.bookmarksfly.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://an.jianghongdianzi.cn

JS:   // 单行；/* 多行 */
来源：http://rh.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://aq.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dj.gzmigu.cn

Go:   // 单行；/* 多行 */
来源：http://gm.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ep.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://dz.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://fw.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://rr.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://zw.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://bs.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://fl.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rd.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://zu.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://qo.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://vv.hahajie.cn

[A16] 真假值判断规则
来源：http://dx.yuexingan06.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bf.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ow.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kw.shtwfgs.cn

TS:   if (!x) {}
来源：http://yv.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jl.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nq.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kz.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lq.521024.cn

[A17] 位运算
来源：http://at.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wc.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kv.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nf.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dr.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pi.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gq.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cu.colortex.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bm.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://av.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://or.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://gy.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fa.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hu.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://ey.bookmarksfly.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ho.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://ap.colortex.cn

C#:   (int)'A'; (char)65
来源：http://ak.shxzskj.cn

[A19] 交换两个变量
来源：http://yg.hnjuh.cn

Py:   a, b = b, a
来源：http://sm.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kn.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://kk.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://cx.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://lj.shxzukj.cn

Go:   a, b = b, a
来源：http://nb.gzmigu.cn

Ruby: a, b = b, a
来源：http://hu.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://xi.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://ju.panjiajie.cn

Py:   name = input("请输入：")
来源：http://lb.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://af.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sm.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://lq.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://ft.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ri.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://fw.colortex.cn

C#:   Console.ReadLine();
来源：http://hg.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://lv.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://nv.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://od.shxzskj.cn

JS:   (3.14159).toFixed(2)
来源：http://of.szsharing.cn

TS:   (3.14159).toFixed(2)
来源：http://ts.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://fv.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mx.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://ev.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://iq.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://ma.haigaiapp.cn

Py:   len(s)
来源：http://co.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tw.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bq.9csxet.cn

TS:   s.length
来源：http://pk.huixinmuqiang.cn

Java: s.length()
来源：http://sz.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oa.shxzskj.cn

Ruby: s.length
来源：http://th.haigaiapp.cn

C#:   s.Length
来源：http://ew.panjiajie.cn

[A23] 大小写转换
来源：http://nc.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bd.bjjhwx.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mq.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sn.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tm.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jr.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ti.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jh.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://md.shxzskj.cn

[A24] 去除首尾空白
来源：http://jl.yuntaijiaju.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qb.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fn.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oa.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nj.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ih.521024.cn

Go:   strings.TrimSpace(s)
来源：http://js.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://if.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ay.wgjwhj.cn

[A25] 字符串比较
来源：http://ae.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://tu.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gz.panjiajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xy.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eq.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://om.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oh.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oh.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nc.hahajie.cn

[A26] 类型转换总览
来源：http://ne.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fw.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lf.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hs.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://qv.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jl.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cm.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yo.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zb.9csxet.cn

================================================================================
来源：http://hg.chemitech.net.cn

B. 流程控制
来源：http://ba.panjiajie.cn

================================================================================
来源：http://eu.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://kw.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qq.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bj.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jj.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yq.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bl.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rh.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://he.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yl.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://bb.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xz.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dk.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lo.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qj.gzmigu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vb.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bi.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jh.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yv.szxytkj.cn

[B03] switch / match / case
来源：http://fu.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fr.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rt.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://on.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bs.asd995.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://we.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://og.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://de.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zt.gzmigu.cn

[B04] for 计数循环
来源：http://es.lnxyls.cn

Py:   for i in range(10): print(i)
来源：http://iz.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hj.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ar.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lb.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ft.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vy.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://sj.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ft.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://hl.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://op.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ec.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yp.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ol.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jp.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sd.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://wc.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qg.shxzukj.cn

[B06] 遍历字典 / 对象
来源：http://op.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://eb.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mo.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bj.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nk.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lz.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fi.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://el.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ar.newstarts.cn

[B07] while 循环
来源：http://dh.szsharing.cn

Py:   while i < 10: i += 1
来源：http://gp.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ve.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://fb.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://cv.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://ek.yuntaijiaju.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://le.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://fl.szsharing.cn

C#:   while (i < 10) { i++; }
来源：http://qx.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://qc.panjiajie.cn


<!-- 参考信息 -->