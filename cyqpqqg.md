代发 wailian999

================================================================================
来源：http://jy.huixinmuqiang.cn

A. 基础语法与类型
来源：http://rg.jianghongdianzi.cn

================================================================================
来源：http://tw.colortex.cn

[A01] Hello World
来源：http://ez.gzmigu.cn

Py:   print("Hello, World!")
来源：http://wy.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://cb.colortex.cn

JS:   console.log("Hello, World!");
来源：http://uh.szxytkj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sm.9csxet.cn

Java: System.out.println("Hello, World!");
来源：http://ot.hnjuh.cn

Go:   fmt.Println("Hello, World!")
来源：http://mi.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://yf.lnxyls.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kr.gzmigu.cn

[A02] 变量声明与赋值
来源：http://ow.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cy.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gp.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://oe.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kx.newstarts.cn

Java: String name = "Alex"; int age = 20;
来源：http://gj.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://tw.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://ro.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sz.9csxet.cn

[A03] 常量定义
来源：http://vo.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nu.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://md.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://jr.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://ol.muxihuayi.cn

Java: static final double PI = 3.14159;
来源：http://iy.szsharing.cn

Go:   const PI = 3.14159
来源：http://cu.szsharing.cn

Ruby: PI = 3.14159
来源：http://lg.9csxet.cn

C#:   const double PI = 3.14159;
来源：http://mw.gzmigu.cn

[A04] 判断变量类型
来源：http://pw.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fr.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://di.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ze.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://pa.lnxyls.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qh.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rx.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lb.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://us.shxzskj.cn

[A05] 整数除法与取模
来源：http://vs.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rc.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nd.chemitech.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rj.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mu.gzmigu.cn

Java: 7 / 2; 7 % 2
来源：http://qe.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://el.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://nr.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://oa.huanxung.cn

[A06] 字符串转数字
来源：http://rx.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://ww.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hm.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qf.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lj.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yg.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oj.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yr.yuexingan06.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://by.shxzukj.cn

[A07] 数字转字符串
来源：http://gv.szxytkj.cn

Py:   str(42)
来源：http://ey.bookmarksfly.cn

PHP:  (string) 42; strval(42)
来源：http://yw.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://vv.hnjuh.cn

TS:   String(42)
来源：http://jz.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://px.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://lh.szsharing.cn

Ruby: 42.to_s
来源：http://nh.szxytkj.cn

C#:   42.ToString()
来源：http://iu.huixiangedu.cn

[A08] 取整与四舍五入
来源：http://dn.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yp.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lk.muxihuayi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://aa.9csxet.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bt.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://aa.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lb.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xh.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qg.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://ez.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lh.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kz.yuexingan06.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dm.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nl.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gr.yuntaijiaju.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tu.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://eq.szxytkj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lu.hahajie.cn

[A10] 生成随机数
来源：http://cr.shxzukj.cn

Py:   import random; random.randint(1, 100)
来源：http://dd.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://xz.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rn.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uv.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://gs.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://li.chemitech.net.cn

Ruby: rand(1..100)
来源：http://vf.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://kt.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://df.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://mr.panjiajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hu.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pb.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zx.huanxung.cn

Java: x > 0 ? "yes" : "no"
来源：http://ko.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jf.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lu.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ru.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://pv.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yf.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bx.bookmarksfly.cn

JS:   `Hello, ${name}!`
来源：http://up.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://kw.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://xl.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jw.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://pd.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://uj.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xq.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://ag.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://gr.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://nx.nszjky.cn

TS:   "第一行\n第二行"
来源：http://jy.nszjky.cn

Java: "第一行\n第二行"
来源：http://zi.shtwfgs.cn

Go:   "第一行\n第二行"
来源：http://ad.521024.cn

Ruby: "第一行\n第二行"
来源：http://lm.huanxung.cn

C#:   "第一行\n第二行"
来源：http://ta.bjjhwx.cn

[A14] 注释写法
来源：http://pf.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xv.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gy.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://ff.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://lm.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pn.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://wk.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://em.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://kn.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://jq.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://zv.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://lz.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://zk.hahajie.cn

TS:   const value = data ?? "默认值";
来源：http://zq.colortex.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ce.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://nm.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://vh.nszjky.cn

C#:   var value = data ?? "默认值";
来源：http://zn.panjiajie.cn

[A16] 真假值判断规则
来源：http://yk.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wl.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nt.huixiangedu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ge.lnxyls.cn

TS:   if (!x) {}
来源：http://ft.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yy.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ia.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xf.hahajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xi.hahajie.cn

[A17] 位运算
来源：http://hz.szxytkj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tr.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://je.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rw.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gt.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kf.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yc.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jh.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fl.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://ju.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://cf.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://ku.gzmigu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lx.jctech888.com.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ij.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://gc.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lk.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://ce.szxytkj.cn

C#:   (int)'A'; (char)65
来源：http://ps.nicolike.cn

[A19] 交换两个变量
来源：http://mz.jctech888.com.cn

Py:   a, b = b, a
来源：http://vw.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tg.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://bn.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://xk.521024.cn

Java: int t = a; a = b; b = t;
来源：http://ql.huixiangedu.cn

Go:   a, b = b, a
来源：http://co.muxihuayi.cn

Ruby: a, b = b, a
来源：http://ve.shtwfgs.cn

C#:   (a, b) = (b, a);
来源：http://rb.huixiangedu.cn

[A20] 读取标准输入
来源：http://lk.lnxyls.cn

Py:   name = input("请输入：")
来源：http://ci.huixinmuqiang.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bz.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://to.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://bd.gzmigu.cn

Java: new Scanner(System.in).nextLine()
来源：http://qh.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ev.huanxung.cn

Ruby: gets.chomp
来源：http://mr.hnjuh.cn

C#:   Console.ReadLine();
来源：http://jy.521024.cn

[A21] 保留指定小数位输出
来源：http://cz.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://yv.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ar.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://ax.szsharing.cn

TS:   (3.14159).toFixed(2)
来源：http://gv.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://xg.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jk.yuntaijiaju.cn

Ruby: format("%.2f", 3.14159)
来源：http://al.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://ao.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://qo.newstarts.cn

Py:   len(s)
来源：http://qd.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jc.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wy.huanxung.cn

TS:   s.length
来源：http://uq.huanxung.cn

Java: s.length()
来源：http://ss.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sd.yuntaijiaju.cn

Ruby: s.length
来源：http://je.yuntaijiaju.cn

C#:   s.Length
来源：http://xb.szsharing.cn

[A23] 大小写转换
来源：http://yn.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sn.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://py.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gm.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://aw.chemitech.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ii.muxihuayi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tv.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jh.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rk.yuexingan06.cn

[A24] 去除首尾空白
来源：http://em.jctech888.com.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qx.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xb.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gm.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wc.huixiangedu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ia.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://oy.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ff.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qw.asd995.cn

[A25] 字符串比较
来源：http://jh.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://xj.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fm.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hi.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gu.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vs.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bl.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sk.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cf.asd995.cn

[A26] 类型转换总览
来源：http://ph.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iu.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cr.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bw.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://ub.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xp.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uh.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://va.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://aw.huixiangedu.cn

================================================================================
来源：http://fr.jianghongdianzi.cn

B. 流程控制
来源：http://ew.9csxet.cn

================================================================================
来源：http://cr.lnxyls.cn

[B01] 条件判断 if / else
来源：http://au.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cs.huixiangedu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oh.szsharing.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dr.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aj.wgjwhj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cd.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://do.muxihuayi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://md.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ma.shxzskj.cn

[B02] 多分支 else if / elif
来源：http://lo.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cu.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xr.huixinmuqiang.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cy.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gy.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oi.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jj.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pd.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vx.521024.cn

[B03] switch / match / case
来源：http://nv.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mv.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mo.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sf.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pr.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tu.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://td.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sx.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://aq.hnjuh.cn

[B04] for 计数循环
来源：http://sz.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://da.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xa.szsharing.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mx.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ws.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gs.9csxet.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ue.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://zm.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ym.9csxet.cn

[B05] 遍历数组 / 列表
来源：http://va.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://ir.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ut.hnjuh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lv.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yq.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bx.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ul.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://dh.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hn.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://xa.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jj.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pq.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hj.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jw.shtwfgs.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gk.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sl.shxzukj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ml.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vs.haigaiapp.cn

[B07] while 循环
来源：http://li.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://tm.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ss.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://bu.521024.cn

TS:   while (i < 10) { i++; }
来源：http://qa.jctech888.com.cn

Java: while (i < 10) { i++; }
来源：http://kg.shtwfgs.cn


<!-- 参考信息 -->