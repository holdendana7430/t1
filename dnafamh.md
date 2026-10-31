代发 wailian999

================================================================================
来源：http://mx.newstarts.cn

A. 基础语法与类型
来源：http://jf.hahajie.cn

================================================================================
来源：http://eo.shxzukj.cn

[A01] Hello World
来源：http://tx.gzmigu.cn

Py:   print("Hello, World!")
来源：http://yz.colortex.cn

PHP:  echo "Hello, World!";
来源：http://wx.521024.cn

JS:   console.log("Hello, World!");
来源：http://ii.nszjky.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://aa.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://kn.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://en.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://wi.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qd.chemitech.net.cn

[A02] 变量声明与赋值
来源：http://zy.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xb.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hu.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gq.lnxyls.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ja.asd995.cn

Java: String name = "Alex"; int age = 20;
来源：http://gp.nszjky.cn

Go:   name := "Alex"; age := 20
来源：http://zl.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://aq.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dk.nicolike.cn

[A03] 常量定义
来源：http://bp.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ro.haigaiapp.cn

PHP:  const PI = 3.14159;
来源：http://dn.newstarts.cn

JS:   const PI = 3.14159;
来源：http://kn.huixiangedu.cn

TS:   const PI: number = 3.14159;
来源：http://hi.haigaiapp.cn

Java: static final double PI = 3.14159;
来源：http://os.shxzskj.cn

Go:   const PI = 3.14159
来源：http://du.lnxyls.cn

Ruby: PI = 3.14159
来源：http://xj.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://ro.muxihuayi.cn

[A04] 判断变量类型
来源：http://wz.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wo.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://we.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pi.hahajie.cn

TS:   typeof x; x instanceof Date
来源：http://mp.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://au.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vt.chemitech.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://or.shxzskj.cn

C#:   x.GetType().Name; x is int
来源：http://aj.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://tp.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tm.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vj.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qh.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qv.bookmarksfly.cn

Java: 7 / 2; 7 % 2
来源：http://te.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://vn.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://bo.shxzukj.cn

C#:   7 / 2; 7 % 2
来源：http://ub.gzmigu.cn

[A06] 字符串转数字
来源：http://ir.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://ht.shxzskj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pd.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ku.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bk.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mv.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://im.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ti.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qw.newstarts.cn

[A07] 数字转字符串
来源：http://hj.yuexingan06.cn

Py:   str(42)
来源：http://vs.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://uy.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://dz.jctech888.com.cn

TS:   String(42)
来源：http://ad.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://am.hahajie.cn

Go:   strconv.Itoa(42)
来源：http://uu.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://of.huixinmuqiang.cn

C#:   42.ToString()
来源：http://vz.colortex.cn

[A08] 取整与四舍五入
来源：http://ku.nicolike.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kj.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wo.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pg.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xc.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sk.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wy.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xd.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ot.huanxung.cn

[A09] 绝对值与最大最小值
来源：http://nz.hnjuh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xj.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cm.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://to.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gf.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hp.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tr.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qs.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lk.haigaiapp.cn

[A10] 生成随机数
来源：http://jb.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://db.haigaiapp.cn

PHP:  random_int(1, 100);
来源：http://yw.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sb.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rj.muxihuayi.cn

Java: new Random().nextInt(100) + 1
来源：http://ny.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://el.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://hd.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://cu.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://me.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cx.newstarts.cn

JS:   x > 0 ? "yes" : "no"
来源：http://eh.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uj.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://eq.jianghongdianzi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dk.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mk.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sb.shxzukj.cn

[A12] 字符串插值 / 格式化
来源：http://dj.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vq.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bz.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://zs.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://hk.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://ik.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mi.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://li.huixinmuqiang.cn

C#:   $"Hello, {name}!"
来源：http://wx.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://am.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://jw.shxzukj.cn

PHP:  "第一行\n第二行"
来源：http://uy.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://vs.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://rl.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://cz.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://pt.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://xn.haigaiapp.cn

C#:   "第一行\n第二行"
来源：http://dj.yuntaijiaju.cn

[A14] 注释写法
来源：http://bd.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ss.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ls.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://km.bjjhwx.cn

TS:   // 单行；/* 多行 */
来源：http://hf.gzmigu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://eb.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://ud.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://au.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://pp.asd995.cn

[A15] 空值判断与默认值
来源：http://qg.panjiajie.cn

Py:   value = data or "默认值"
来源：http://wl.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://sy.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://ub.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://nh.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yf.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://qa.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://ja.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://zv.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://gw.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lw.9csxet.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xd.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lg.huanxung.cn

TS:   if (!x) {}
来源：http://ec.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qb.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vb.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mc.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nw.huixiangedu.cn

[A17] 位运算
来源：http://ja.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jg.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ub.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dw.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xj.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sr.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://va.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ec.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://up.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://uz.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://mx.521024.cn

PHP:  ord("A"); chr(65)
来源：http://nb.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qb.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lm.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://kf.lnxyls.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://em.521024.cn

Ruby: "A".ord; 65.chr
来源：http://or.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://ai.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://bo.muxihuayi.cn

Py:   a, b = b, a
来源：http://vt.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zp.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://gw.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://bk.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://ay.hahajie.cn

Go:   a, b = b, a
来源：http://dy.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://nh.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://gp.bookmarksfly.cn

[A20] 读取标准输入
来源：http://yw.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://kv.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://va.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gg.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://ht.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://he.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://na.nicolike.cn

Ruby: gets.chomp
来源：http://ks.nicolike.cn

C#:   Console.ReadLine();
来源：http://ak.hahajie.cn

[A21] 保留指定小数位输出
来源：http://wf.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://hw.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qn.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://gz.521024.cn

TS:   (3.14159).toFixed(2)
来源：http://wy.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://ks.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nf.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://of.yuexingan06.cn

C#:   3.14159.ToString("F2")
来源：http://fl.nszjky.cn

[A22] 获取字符串长度
来源：http://up.wgjwhj.cn

Py:   len(s)
来源：http://mz.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ny.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ug.huixinmuqiang.cn

TS:   s.length
来源：http://fy.jianghongdianzi.cn

Java: s.length()
来源：http://ex.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ed.yuexingan06.cn

Ruby: s.length
来源：http://ll.szsharing.cn

C#:   s.Length
来源：http://wq.jctech888.com.cn

[A23] 大小写转换
来源：http://ms.huanxung.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://go.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ph.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yc.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mn.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vt.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ii.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pq.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yq.huixiangedu.cn

[A24] 去除首尾空白
来源：http://sf.lnxyls.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ka.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nl.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bz.gzmigu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gn.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ql.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://nj.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fn.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uw.521024.cn

[A25] 字符串比较
来源：http://nh.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://xu.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ex.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uv.szxytkj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pn.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dm.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pr.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://eg.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nv.lnxyls.cn

[A26] 类型转换总览
来源：http://at.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lt.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rz.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wt.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://bm.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lr.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fb.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fm.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pv.jctech888.com.cn

================================================================================
来源：http://is.hnjuh.cn

B. 流程控制
来源：http://yd.shxzukj.cn

================================================================================
来源：http://on.nszjky.cn

[B01] 条件判断 if / else
来源：http://oc.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mn.jianghongdianzi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uw.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yv.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gr.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sh.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oq.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bb.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ov.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://wg.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wn.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uf.9csxet.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tl.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xf.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ni.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zn.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gl.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tu.panjiajie.cn

[B03] switch / match / case
来源：http://rq.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zt.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://my.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sp.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vd.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mq.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://in.bookmarksfly.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dh.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fr.9csxet.cn

[B04] for 计数循环
来源：http://xv.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://xz.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lp.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lm.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qa.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ri.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hs.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://pp.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bv.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://ym.huixinmuqiang.cn

Py:   for item in arr: print(item)
来源：http://fi.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zq.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qi.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zb.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://es.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pb.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://da.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tq.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://xd.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cy.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fw.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vz.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lh.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kk.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cr.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yj.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jm.nszjky.cn

[B07] while 循环
来源：http://vo.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://xv.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jp.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://ea.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://nv.9csxet.cn

Java: while (i < 10) { i++; }
来源：http://yk.shtwfgs.cn


<!-- 参考信息 -->