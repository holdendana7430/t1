代发 wailian999

================================================================================
来源：http://pz.panjiajie.cn

A. 基础语法与类型
来源：http://ih.szxytkj.cn

================================================================================
来源：http://fl.lnxyls.cn

[A01] Hello World
来源：http://ow.chemitech.net.cn

Py:   print("Hello, World!")
来源：http://bp.521024.cn

PHP:  echo "Hello, World!";
来源：http://ge.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://il.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dw.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://kj.newstarts.cn

Go:   fmt.Println("Hello, World!")
来源：http://mq.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://vx.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nx.colortex.cn

[A02] 变量声明与赋值
来源：http://vn.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://du.521024.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ub.huixiangedu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://la.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://op.bookmarksfly.cn

Java: String name = "Alex"; int age = 20;
来源：http://rw.haigaiapp.cn

Go:   name := "Alex"; age := 20
来源：http://ct.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://vt.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qh.newstarts.cn

[A03] 常量定义
来源：http://tt.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ww.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://ou.nicolike.cn

JS:   const PI = 3.14159;
来源：http://jd.jctech888.com.cn

TS:   const PI: number = 3.14159;
来源：http://te.shxzskj.cn

Java: static final double PI = 3.14159;
来源：http://qf.nicolike.cn

Go:   const PI = 3.14159
来源：http://ww.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://ex.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://kj.521024.cn

[A04] 判断变量类型
来源：http://gw.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qf.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yf.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mz.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://pj.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yt.gzmigu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nl.haigaiapp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mx.szxytkj.cn

C#:   x.GetType().Name; x is int
来源：http://vz.yuexingan06.cn

[A05] 整数除法与取模
来源：http://fe.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pg.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://na.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ed.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cj.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://lp.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://jc.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://qq.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://vo.wgjwhj.cn

[A06] 字符串转数字
来源：http://sx.panjiajie.cn

Py:   int("42"); float("3.14")
来源：http://fg.gzmigu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://en.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mg.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://do.muxihuayi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nt.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lt.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sr.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://us.bjjhwx.cn

[A07] 数字转字符串
来源：http://oq.asd995.cn

Py:   str(42)
来源：http://nr.521024.cn

PHP:  (string) 42; strval(42)
来源：http://pa.gzmigu.cn

JS:   String(42); (42).toString()
来源：http://gh.shxzukj.cn

TS:   String(42)
来源：http://zo.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fp.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://ka.shxzukj.cn

Ruby: 42.to_s
来源：http://ue.yuexingan06.cn

C#:   42.ToString()
来源：http://fk.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://pp.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wz.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yd.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yb.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://js.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gb.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.szxytkj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fu.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fn.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://oe.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rg.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://an.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://an.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bo.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ml.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nd.bookmarksfly.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://po.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rk.huixinmuqiang.cn

[A10] 生成随机数
来源：http://un.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://ns.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://vo.szxytkj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ge.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wt.521024.cn

Java: new Random().nextInt(100) + 1
来源：http://fa.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jh.shxzskj.cn

Ruby: rand(1..100)
来源：http://tq.yuexingan06.cn

C#:   new Random().Next(1, 101)
来源：http://ua.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://mr.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://lw.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mn.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dk.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wl.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://kq.shxzukj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ml.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tv.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fu.szxytkj.cn

[A12] 字符串插值 / 格式化
来源：http://bn.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lu.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gk.huixiangedu.cn

JS:   `Hello, ${name}!`
来源：http://rk.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://gf.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://ma.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mo.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://ta.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://do.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pm.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://dy.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://ha.colortex.cn

JS:   "第一行\n第二行"
来源：http://nl.gzmigu.cn

TS:   "第一行\n第二行"
来源：http://bn.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://kq.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://dn.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://ex.szsharing.cn

C#:   "第一行\n第二行"
来源：http://hr.chemitech.net.cn

[A14] 注释写法
来源：http://uv.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://uh.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.shtwfgs.cn

JS:   // 单行；/* 多行 */
来源：http://za.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://re.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nw.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://gw.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ih.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://no.shxzukj.cn

[A15] 空值判断与默认值
来源：http://ik.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://wm.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://wt.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://rr.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://yi.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jk.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://mc.asd995.cn

Ruby: value = data || "默认值"
来源：http://mn.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://lq.gzmigu.cn

[A16] 真假值判断规则
来源：http://dx.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uy.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tm.szsharing.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tc.haigaiapp.cn

TS:   if (!x) {}
来源：http://vp.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://no.bookmarksfly.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ug.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bi.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qv.nszjky.cn

[A17] 位运算
来源：http://og.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tw.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dt.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rx.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xz.szxytkj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ls.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tl.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aj.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zn.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://zz.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://rb.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://zn.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://it.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nb.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://cx.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ch.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://xm.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://xs.bjjhwx.cn

[A19] 交换两个变量
来源：http://kq.haigaiapp.cn

Py:   a, b = b, a
来源：http://vc.521024.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ib.nicolike.cn

JS:   [a, b] = [b, a];
来源：http://fm.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://as.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://qp.haigaiapp.cn

Go:   a, b = b, a
来源：http://bh.huanxung.cn

Ruby: a, b = b, a
来源：http://zm.lnxyls.cn

C#:   (a, b) = (b, a);
来源：http://qp.panjiajie.cn

[A20] 读取标准输入
来源：http://vh.gzmigu.cn

Py:   name = input("请输入：")
来源：http://hw.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kr.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tt.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://ku.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://wt.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ae.jctech888.com.cn

Ruby: gets.chomp
来源：http://gf.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://fm.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://xz.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://qp.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zd.yuexingan06.cn

JS:   (3.14159).toFixed(2)
来源：http://iw.szxytkj.cn

TS:   (3.14159).toFixed(2)
来源：http://tn.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://yl.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fw.asd995.cn

Ruby: format("%.2f", 3.14159)
来源：http://sd.huixiangedu.cn

C#:   3.14159.ToString("F2")
来源：http://cl.shxzukj.cn

[A22] 获取字符串长度
来源：http://be.hnjuh.cn

Py:   len(s)
来源：http://ur.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ri.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ha.bjjhwx.cn

TS:   s.length
来源：http://qn.chemitech.net.cn

Java: s.length()
来源：http://yu.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fe.colortex.cn

Ruby: s.length
来源：http://qd.muxihuayi.cn

C#:   s.Length
来源：http://kg.bookmarksfly.cn

[A23] 大小写转换
来源：http://za.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vs.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gn.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jw.nicolike.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ea.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pb.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sh.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zx.huixiangedu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zb.bjjhwx.cn

[A24] 去除首尾空白
来源：http://ef.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ph.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ei.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://el.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rd.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fa.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://at.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://un.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://od.yuntaijiaju.cn

[A25] 字符串比较
来源：http://fm.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://tv.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kf.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xz.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://it.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eg.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eo.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lv.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jw.chemitech.net.cn

[A26] 类型转换总览
来源：http://ik.jianghongdianzi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bs.huixinmuqiang.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://go.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vv.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://lo.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fe.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zu.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kq.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wc.shxzukj.cn

================================================================================
来源：http://lh.huixinmuqiang.cn

B. 流程控制
来源：http://lu.newstarts.cn

================================================================================
来源：http://oj.hahajie.cn

[B01] 条件判断 if / else
来源：http://fn.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cs.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fl.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://va.chemitech.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://en.szxytkj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kj.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uc.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oj.jctech888.com.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vh.huanxung.cn

[B02] 多分支 else if / elif
来源：http://zu.asd995.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gy.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nk.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bq.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fh.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ch.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hd.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gl.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fl.gzmigu.cn

[B03] switch / match / case
来源：http://da.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ub.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://il.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wp.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dk.colortex.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://km.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://or.szsharing.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wj.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bu.huixiangedu.cn

[B04] for 计数循环
来源：http://xj.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://dz.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zg.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xg.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yg.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://my.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nm.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://dt.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ti.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://za.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://kt.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kp.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qp.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nj.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cj.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hy.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://mx.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wq.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://mn.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qg.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ij.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://am.yuntaijiaju.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zc.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wy.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ap.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://py.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://br.newstarts.cn

[B07] while 循环
来源：http://md.yuexingan06.cn

Py:   while i < 10: i += 1
来源：http://sb.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mn.panjiajie.cn

JS:   while (i < 10) { i++; }
来源：http://mb.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://kc.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://xi.haigaiapp.cn


<!-- 参考信息 -->