代发 wailian999

================================================================================
来源：http://bl.shxzukj.cn

A. 基础语法与类型
来源：http://ju.chemitech.net.cn

================================================================================
来源：http://ap.huixiangedu.cn

[A01] Hello World
来源：http://as.bjjhwx.cn

Py:   print("Hello, World!")
来源：http://nh.colortex.cn

PHP:  echo "Hello, World!";
来源：http://fn.nszjky.cn

JS:   console.log("Hello, World!");
来源：http://wo.colortex.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dv.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://hy.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://hi.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://fn.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jb.huixinmuqiang.cn

[A02] 变量声明与赋值
来源：http://nh.panjiajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mg.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ru.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://eq.nicolike.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dm.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://zy.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://th.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://uy.yuexingan06.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lr.521024.cn

[A03] 常量定义
来源：http://eo.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mq.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://dy.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://ol.panjiajie.cn

TS:   const PI: number = 3.14159;
来源：http://xe.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://ry.9csxet.cn

Go:   const PI = 3.14159
来源：http://kt.yuntaijiaju.cn

Ruby: PI = 3.14159
来源：http://zg.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://mz.521024.cn

[A04] 判断变量类型
来源：http://vf.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://uo.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fk.yuntaijiaju.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://us.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://ww.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sx.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ob.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fv.shxzukj.cn

C#:   x.GetType().Name; x is int
来源：http://pz.haigaiapp.cn

[A05] 整数除法与取模
来源：http://gd.521024.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ci.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rk.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tj.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mk.shxzukj.cn

Java: 7 / 2; 7 % 2
来源：http://nr.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://oi.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://eq.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://sc.huixiangedu.cn

[A06] 字符串转数字
来源：http://eg.hnjuh.cn

Py:   int("42"); float("3.14")
来源：http://hq.bjjhwx.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cd.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rn.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rf.9csxet.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zd.panjiajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cc.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ke.chemitech.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wb.szsharing.cn

[A07] 数字转字符串
来源：http://sm.szxytkj.cn

Py:   str(42)
来源：http://tb.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://vm.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://cd.szsharing.cn

TS:   String(42)
来源：http://zt.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ye.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://bs.wgjwhj.cn

Ruby: 42.to_s
来源：http://pv.9csxet.cn

C#:   42.ToString()
来源：http://cm.szsharing.cn

[A08] 取整与四舍五入
来源：http://ea.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ak.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vk.gzmigu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yw.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wm.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uf.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wp.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fw.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pp.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://ei.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wi.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://as.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://he.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xj.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gw.huanxung.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://du.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wr.521024.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lb.wgjwhj.cn

[A10] 生成随机数
来源：http://us.yuexingan06.cn

Py:   import random; random.randint(1, 100)
来源：http://ku.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://eb.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bd.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fs.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://fh.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vr.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://vw.szxytkj.cn

C#:   new Random().Next(1, 101)
来源：http://ge.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://bi.lnxyls.cn

Py:   "yes" if x > 0 else "no"
来源：http://gc.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vo.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bc.haigaiapp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ov.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://zy.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xn.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pz.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hu.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://qh.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ad.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iv.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://gn.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://ur.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://py.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zt.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://cf.bookmarksfly.cn

C#:   $"Hello, {name}!"
来源：http://ds.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qi.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://pc.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://sp.muxihuayi.cn

JS:   "第一行\n第二行"
来源：http://rl.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://hn.lnxyls.cn

Java: "第一行\n第二行"
来源：http://oy.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://pa.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://zs.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://ag.wgjwhj.cn

[A14] 注释写法
来源：http://su.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rx.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jt.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://pd.panjiajie.cn

TS:   // 单行；/* 多行 */
来源：http://nd.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xd.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://ra.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bk.yuntaijiaju.cn

C#:   // 单行；/* 多行 */
来源：http://lx.newstarts.cn

[A15] 空值判断与默认值
来源：http://nm.hnjuh.cn

Py:   value = data or "默认值"
来源：http://tc.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://oe.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://xu.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://xn.hnjuh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://co.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://is.szsharing.cn

Ruby: value = data || "默认值"
来源：http://qx.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://sv.hahajie.cn

[A16] 真假值判断规则
来源：http://li.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://va.yuntaijiaju.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://aq.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bd.asd995.cn

TS:   if (!x) {}
来源：http://qn.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qk.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ly.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gy.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gw.wgjwhj.cn

[A17] 位运算
来源：http://vp.yuexingan06.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kp.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nw.hahajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fo.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ag.yuexingan06.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ka.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://po.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cd.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uw.jctech888.com.cn

[A18] 字符与 ASCII 码互转
来源：http://fl.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://mf.haigaiapp.cn

PHP:  ord("A"); chr(65)
来源：http://oj.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ay.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fu.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://hp.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jc.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://iy.9csxet.cn

C#:   (int)'A'; (char)65
来源：http://dd.asd995.cn

[A19] 交换两个变量
来源：http://ki.nszjky.cn

Py:   a, b = b, a
来源：http://je.huixiangedu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://xa.muxihuayi.cn

JS:   [a, b] = [b, a];
来源：http://jf.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://cp.wgjwhj.cn

Java: int t = a; a = b; b = t;
来源：http://mg.asd995.cn

Go:   a, b = b, a
来源：http://nq.huixiangedu.cn

Ruby: a, b = b, a
来源：http://ds.colortex.cn

C#:   (a, b) = (b, a);
来源：http://vd.hahajie.cn

[A20] 读取标准输入
来源：http://sq.bookmarksfly.cn

Py:   name = input("请输入：")
来源：http://ip.asd995.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://aq.jianghongdianzi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sv.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://ss.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://sl.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ui.jctech888.com.cn

Ruby: gets.chomp
来源：http://lz.gzmigu.cn

C#:   Console.ReadLine();
来源：http://bk.nszjky.cn

[A21] 保留指定小数位输出
来源：http://qh.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://ig.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jh.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://uz.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://tz.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://yb.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qv.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://zc.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://rm.muxihuayi.cn

[A22] 获取字符串长度
来源：http://gs.muxihuayi.cn

Py:   len(s)
来源：http://cl.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qt.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cx.nicolike.cn

TS:   s.length
来源：http://rk.asd995.cn

Java: s.length()
来源：http://hc.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fm.shtwfgs.cn

Ruby: s.length
来源：http://sm.huanxung.cn

C#:   s.Length
来源：http://am.huanxung.cn

[A23] 大小写转换
来源：http://he.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jr.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tk.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ks.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hl.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vg.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cq.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gz.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hx.haigaiapp.cn

[A24] 去除首尾空白
来源：http://tv.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gy.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://if.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ox.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lc.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ya.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://pg.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vd.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nw.szxytkj.cn

[A25] 字符串比较
来源：http://ed.huixiangedu.cn

Py:   s1 == s2; s1 != s2
来源：http://un.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rl.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fe.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://al.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ft.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ng.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uf.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dn.huixiangedu.cn

[A26] 类型转换总览
来源：http://vd.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xt.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zd.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bw.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://bd.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zn.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qc.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zy.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zk.haigaiapp.cn

================================================================================
来源：http://uq.9csxet.cn

B. 流程控制
来源：http://sd.lnxyls.cn

================================================================================
来源：http://uw.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://en.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ne.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nu.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zj.shxzukj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ul.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yf.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fx.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zc.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jn.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://vt.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cw.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kf.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yk.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wy.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ut.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mk.jianghongdianzi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kt.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fi.shtwfgs.cn

[B03] switch / match / case
来源：http://tr.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pv.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ks.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ad.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://is.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://md.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wo.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kb.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://za.panjiajie.cn

[B04] for 计数循环
来源：http://ms.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://ue.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uh.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bp.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kf.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fs.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fg.shxzskj.cn

Ruby: 10.times { |i| puts i }
来源：http://ti.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rm.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://dv.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://fw.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vj.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wt.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sr.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kw.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mp.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://sv.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yy.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://sm.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lo.szsharing.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ib.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fp.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nw.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wa.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hb.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://av.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ge.521024.cn

[B07] while 循环
来源：http://iv.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://cy.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ct.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://jb.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://wp.shtwfgs.cn

Java: while (i < 10) { i++; }
来源：http://bi.szxytkj.cn


<!-- 参考信息 -->