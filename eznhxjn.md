代发 wailian999

================================================================================
来源：http://iu.9csxet.cn

A. 基础语法与类型
来源：http://hr.9csxet.cn

================================================================================
来源：http://kx.bjjhwx.cn

[A01] Hello World
来源：http://ml.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://mt.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://jn.lnxyls.cn

JS:   console.log("Hello, World!");
来源：http://vf.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lo.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://ur.huanxung.cn

Go:   fmt.Println("Hello, World!")
来源：http://mu.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://yb.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lc.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://yx.yuntaijiaju.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dv.shxzukj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gx.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://za.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xr.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://lq.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://go.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://lb.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lk.nicolike.cn

[A03] 常量定义
来源：http://mu.hnjuh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ht.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://wr.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://so.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://yo.muxihuayi.cn

Java: static final double PI = 3.14159;
来源：http://bm.panjiajie.cn

Go:   const PI = 3.14159
来源：http://kr.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://lb.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://qx.9csxet.cn

[A04] 判断变量类型
来源：http://sa.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lu.wgjwhj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kl.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ss.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://rd.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ht.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://al.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ir.wgjwhj.cn

C#:   x.GetType().Name; x is int
来源：http://bk.muxihuayi.cn

[A05] 整数除法与取模
来源：http://zp.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ey.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xu.yuexingan06.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hu.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hm.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://zy.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://gs.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://qr.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://yu.jctech888.com.cn

[A06] 字符串转数字
来源：http://fz.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://lt.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ql.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jm.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qf.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://oz.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vx.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xv.asd995.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mw.hahajie.cn

[A07] 数字转字符串
来源：http://rf.huixiangedu.cn

Py:   str(42)
来源：http://ag.szsharing.cn

PHP:  (string) 42; strval(42)
来源：http://lb.huixinmuqiang.cn

JS:   String(42); (42).toString()
来源：http://zt.yuntaijiaju.cn

TS:   String(42)
来源：http://ev.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hp.nszjky.cn

Go:   strconv.Itoa(42)
来源：http://zl.bjjhwx.cn

Ruby: 42.to_s
来源：http://db.shxzukj.cn

C#:   42.ToString()
来源：http://qd.colortex.cn

[A08] 取整与四舍五入
来源：http://wu.hahajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ua.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rb.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nk.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dc.521024.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://be.shtwfgs.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zw.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ii.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://my.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://xd.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qy.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vb.nszjky.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vu.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sy.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ng.jctech888.com.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dk.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ln.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cg.newstarts.cn

[A10] 生成随机数
来源：http://mu.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://uv.szsharing.cn

PHP:  random_int(1, 100);
来源：http://hd.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rb.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gv.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://zk.shxzskj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://md.muxihuayi.cn

Ruby: rand(1..100)
来源：http://kf.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://cw.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://gq.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://vf.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ww.lnxyls.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yg.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hr.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://gk.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qd.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kp.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zw.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://ne.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cs.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vz.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://ya.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://uc.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://ug.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ps.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://mg.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://av.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bb.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://uh.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://pj.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://lr.newstarts.cn

TS:   "第一行\n第二行"
来源：http://jo.colortex.cn

Java: "第一行\n第二行"
来源：http://os.nicolike.cn

Go:   "第一行\n第二行"
来源：http://uf.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://xa.asd995.cn

C#:   "第一行\n第二行"
来源：http://td.jianghongdianzi.cn

[A14] 注释写法
来源：http://pg.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cu.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bu.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://pt.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://yv.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wd.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://os.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lv.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://zs.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://wn.nszjky.cn

Py:   value = data or "默认值"
来源：http://ft.asd995.cn

PHP:  $value = $data ?? "默认值";
来源：http://hy.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://ow.gzmigu.cn

TS:   const value = data ?? "默认值";
来源：http://on.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oq.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://lt.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://no.yuntaijiaju.cn

C#:   var value = data ?? "默认值";
来源：http://ok.jctech888.com.cn

[A16] 真假值判断规则
来源：http://jm.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://et.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eq.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lw.shtwfgs.cn

TS:   if (!x) {}
来源：http://pz.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xm.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pq.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ru.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vi.hahajie.cn

[A17] 位运算
来源：http://ud.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hi.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yd.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bj.lnxyls.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ox.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ej.521024.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bx.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nb.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hm.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://lf.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://dw.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://at.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://il.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kb.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://un.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yk.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://lb.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://wb.newstarts.cn

[A19] 交换两个变量
来源：http://op.szsharing.cn

Py:   a, b = b, a
来源：http://zr.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fo.521024.cn

JS:   [a, b] = [b, a];
来源：http://xd.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://eq.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://yi.yuntaijiaju.cn

Go:   a, b = b, a
来源：http://ap.bjjhwx.cn

Ruby: a, b = b, a
来源：http://yl.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://kv.521024.cn

[A20] 读取标准输入
来源：http://dn.hahajie.cn

Py:   name = input("请输入：")
来源：http://je.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yf.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zb.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://mr.nicolike.cn

Java: new Scanner(System.in).nextLine()
来源：http://yd.chemitech.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yk.gzmigu.cn

Ruby: gets.chomp
来源：http://kw.szxytkj.cn

C#:   Console.ReadLine();
来源：http://ra.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://gq.hahajie.cn

Py:   f"{3.14159:.2f}"
来源：http://pc.jianghongdianzi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lt.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://dj.bjjhwx.cn

TS:   (3.14159).toFixed(2)
来源：http://pt.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://es.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xy.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://ae.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://xe.shtwfgs.cn

[A22] 获取字符串长度
来源：http://vf.szxytkj.cn

Py:   len(s)
来源：http://rw.shtwfgs.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hs.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aa.huanxung.cn

TS:   s.length
来源：http://ph.szsharing.cn

Java: s.length()
来源：http://vi.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://el.nszjky.cn

Ruby: s.length
来源：http://kr.chemitech.net.cn

C#:   s.Length
来源：http://lg.muxihuayi.cn

[A23] 大小写转换
来源：http://xg.jianghongdianzi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cp.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oo.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kp.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://se.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pf.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ru.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ao.shxzukj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yq.szsharing.cn

[A24] 去除首尾空白
来源：http://tg.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bi.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vz.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tc.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ps.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://qm.jctech888.com.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zg.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ay.gzmigu.cn

[A25] 字符串比较
来源：http://lu.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://bc.muxihuayi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gf.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oh.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://df.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://re.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sc.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jp.asd995.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uy.jctech888.com.cn

[A26] 类型转换总览
来源：http://we.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://es.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://os.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cg.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://sn.lnxyls.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cz.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hh.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://al.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kf.haigaiapp.cn

================================================================================
来源：http://xr.yuntaijiaju.cn

B. 流程控制
来源：http://wo.chemitech.net.cn

================================================================================
来源：http://fq.shxzukj.cn

[B01] 条件判断 if / else
来源：http://qn.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://be.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ny.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xl.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aa.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hs.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nu.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qi.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pf.521024.cn

[B02] 多分支 else if / elif
来源：http://iw.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tv.hahajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vx.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ly.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kd.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ss.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zw.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://le.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gv.huixiangedu.cn

[B03] switch / match / case
来源：http://ah.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nr.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yx.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ln.wgjwhj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wh.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wh.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ks.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gj.yuexingan06.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ge.521024.cn

[B04] for 计数循环
来源：http://yo.shtwfgs.cn

Py:   for i in range(10): print(i)
来源：http://jf.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jy.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xe.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lz.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gt.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zq.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://ed.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ma.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://uh.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://px.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nx.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nr.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://aw.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gs.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sl.bjjhwx.cn

Ruby: arr.each { |item| puts item }
来源：http://vo.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rj.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://ar.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bz.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ua.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eu.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pg.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://da.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://my.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rl.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hg.chemitech.net.cn

[B07] while 循环
来源：http://ud.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://nv.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ut.hahajie.cn

JS:   while (i < 10) { i++; }
来源：http://po.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://cp.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://gr.asd995.cn


<!-- 参考信息 -->