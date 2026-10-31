代发 wailian999

================================================================================
来源：http://li.yuexingan06.cn

A. 基础语法与类型
来源：http://fw.asd995.cn

================================================================================
来源：http://ad.yuexingan06.cn

[A01] Hello World
来源：http://gh.panjiajie.cn

Py:   print("Hello, World!")
来源：http://yd.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://jz.gzmigu.cn

JS:   console.log("Hello, World!");
来源：http://mi.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sb.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://ov.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://gs.haigaiapp.cn

Ruby: puts "Hello, World!"
来源：http://sv.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rh.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://lk.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://di.bjjhwx.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wt.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zu.chemitech.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ew.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://id.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://rk.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://ul.bookmarksfly.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jg.wgjwhj.cn

[A03] 常量定义
来源：http://en.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vc.jianghongdianzi.cn

PHP:  const PI = 3.14159;
来源：http://mk.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://mq.colortex.cn

TS:   const PI: number = 3.14159;
来源：http://xv.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://bq.muxihuayi.cn

Go:   const PI = 3.14159
来源：http://rs.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://vz.521024.cn

C#:   const double PI = 3.14159;
来源：http://rp.szxytkj.cn

[A04] 判断变量类型
来源：http://ed.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zo.gzmigu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rl.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ok.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://yt.yuexingan06.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qc.shxzskj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ca.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vh.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://ia.haigaiapp.cn

[A05] 整数除法与取模
来源：http://ex.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://iz.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yc.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ot.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://im.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://gn.bjjhwx.cn

Go:   7 / 2; 7 % 2
来源：http://fl.yuntaijiaju.cn

Ruby: 7 / 2; 7 % 2
来源：http://sr.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://if.muxihuayi.cn

[A06] 字符串转数字
来源：http://fv.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://tk.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ad.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mk.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wf.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vz.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gi.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mt.jctech888.com.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dh.szsharing.cn

[A07] 数字转字符串
来源：http://fo.521024.cn

Py:   str(42)
来源：http://oe.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://nz.521024.cn

JS:   String(42); (42).toString()
来源：http://zi.bookmarksfly.cn

TS:   String(42)
来源：http://xv.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://uo.gzmigu.cn

Go:   strconv.Itoa(42)
来源：http://yv.bookmarksfly.cn

Ruby: 42.to_s
来源：http://td.shtwfgs.cn

C#:   42.ToString()
来源：http://ur.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://uc.bjjhwx.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bc.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ro.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ig.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qv.haigaiapp.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qf.jctech888.com.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xy.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mi.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kq.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://ck.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mg.9csxet.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sm.newstarts.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fy.colortex.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jl.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mq.jctech888.com.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://us.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pd.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nv.panjiajie.cn

[A10] 生成随机数
来源：http://mx.nszjky.cn

Py:   import random; random.randint(1, 100)
来源：http://hi.9csxet.cn

PHP:  random_int(1, 100);
来源：http://mu.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xh.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hs.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://tw.szsharing.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hf.asd995.cn

Ruby: rand(1..100)
来源：http://fm.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://cv.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://pf.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://wz.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dt.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bx.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jj.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://us.huixiangedu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gx.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wq.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://al.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://nc.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://th.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jn.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://nz.asd995.cn

TS:   `Hello, ${name}!`
来源：http://uw.asd995.cn

Java: "Hello, %s!".formatted(name)
来源：http://tk.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pz.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://sk.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://pf.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zc.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://ww.chemitech.net.cn

PHP:  "第一行\n第二行"
来源：http://fv.yuntaijiaju.cn

JS:   "第一行\n第二行"
来源：http://bk.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://ka.newstarts.cn

Java: "第一行\n第二行"
来源：http://my.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://yu.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://lp.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://zl.lnxyls.cn

[A14] 注释写法
来源：http://uk.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cz.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sj.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://yw.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://tc.gzmigu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ap.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://fr.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nu.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://zn.9csxet.cn

[A15] 空值判断与默认值
来源：http://yz.hnjuh.cn

Py:   value = data or "默认值"
来源：http://ra.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ts.haigaiapp.cn

JS:   const value = data ?? "默认值";
来源：http://jt.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://po.wgjwhj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dr.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://lz.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://py.521024.cn

C#:   var value = data ?? "默认值";
来源：http://xq.lnxyls.cn

[A16] 真假值判断规则
来源：http://xa.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pz.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tr.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bf.szsharing.cn

TS:   if (!x) {}
来源：http://ks.nicolike.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uw.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dd.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://id.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tr.hnjuh.cn

[A17] 位运算
来源：http://wl.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ft.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mw.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ys.shtwfgs.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ot.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ng.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xv.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hp.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bb.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://uj.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://ee.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://ke.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ne.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://un.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://cu.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sc.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://qa.asd995.cn

C#:   (int)'A'; (char)65
来源：http://dc.nszjky.cn

[A19] 交换两个变量
来源：http://xp.nszjky.cn

Py:   a, b = b, a
来源：http://vf.bookmarksfly.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tj.colortex.cn

JS:   [a, b] = [b, a];
来源：http://nj.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://sx.bookmarksfly.cn

Java: int t = a; a = b; b = t;
来源：http://gg.haigaiapp.cn

Go:   a, b = b, a
来源：http://dx.jctech888.com.cn

Ruby: a, b = b, a
来源：http://ff.huixinmuqiang.cn

C#:   (a, b) = (b, a);
来源：http://mv.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://ss.colortex.cn

Py:   name = input("请输入：")
来源：http://hh.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gp.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://do.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://lq.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://vu.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lq.huanxung.cn

Ruby: gets.chomp
来源：http://dg.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://ln.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://lc.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://rw.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bq.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://gs.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://td.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://sn.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cx.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://sr.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://tk.asd995.cn

[A22] 获取字符串长度
来源：http://ne.jianghongdianzi.cn

Py:   len(s)
来源：http://ed.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://km.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pi.haigaiapp.cn

TS:   s.length
来源：http://sh.gzmigu.cn

Java: s.length()
来源：http://in.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zl.nszjky.cn

Ruby: s.length
来源：http://ql.huixiangedu.cn

C#:   s.Length
来源：http://mo.asd995.cn

[A23] 大小写转换
来源：http://ot.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nn.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hy.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xr.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xl.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://to.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tg.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yw.jctech888.com.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sn.gzmigu.cn

[A24] 去除首尾空白
来源：http://kt.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sx.lnxyls.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kp.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jz.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jm.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://og.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://qd.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ze.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yq.huanxung.cn

[A25] 字符串比较
来源：http://re.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://am.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kg.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hr.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fm.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://du.shxzskj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nu.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://np.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cs.gzmigu.cn

[A26] 类型转换总览
来源：http://gs.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pj.yuexingan06.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oz.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xu.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://pe.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hk.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tk.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ux.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wr.newstarts.cn

================================================================================
来源：http://wx.lnxyls.cn

B. 流程控制
来源：http://jt.colortex.cn

================================================================================
来源：http://cz.shtwfgs.cn

[B01] 条件判断 if / else
来源：http://nl.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://om.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wd.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yz.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ex.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nl.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dn.huixinmuqiang.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wo.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wc.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://xk.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wg.yuexingan06.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sp.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jd.521024.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ox.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bd.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fp.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ns.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gp.huanxung.cn

[B03] switch / match / case
来源：http://fo.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yd.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nm.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rm.shxzukj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yp.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://be.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://us.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wt.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ve.hnjuh.cn

[B04] for 计数循环
来源：http://mo.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://wy.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qg.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zy.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xn.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wv.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yz.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://yg.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://er.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://ih.hahajie.cn

Py:   for item in arr: print(item)
来源：http://tp.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pm.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sr.huixiangedu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fk.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://at.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wm.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://ph.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vq.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://nf.newstarts.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fq.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ak.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lb.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zo.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fe.shxzskj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wl.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ak.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yj.yuntaijiaju.cn

[B07] while 循环
来源：http://hn.hahajie.cn

Py:   while i < 10: i += 1
来源：http://aq.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uy.bookmarksfly.cn

JS:   while (i < 10) { i++; }
来源：http://dk.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://xh.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://bo.jianghongdianzi.cn


<!-- 参考信息 -->