代发 wailian999

Py:   print("Hello, World!")
来源：http://se.shtwfgs.cn

PHP:  echo "Hello, World!";
来源：http://bi.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://ot.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mz.huixiangedu.cn

Java: System.out.println("Hello, World!");
来源：http://cp.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://me.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://jc.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bj.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://tr.yuntaijiaju.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lf.9csxet.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ee.nszjky.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ll.muxihuayi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ox.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://cs.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://dv.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://xq.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jq.szxytkj.cn

[A03] 常量定义
来源：http://be.gzmigu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ax.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://bp.asd995.cn

JS:   const PI = 3.14159;
来源：http://wm.jctech888.com.cn

TS:   const PI: number = 3.14159;
来源：http://jt.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://el.shxzukj.cn

Go:   const PI = 3.14159
来源：http://cv.hnjuh.cn

Ruby: PI = 3.14159
来源：http://fx.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://if.jctech888.com.cn

[A04] 判断变量类型
来源：http://op.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ey.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tk.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mp.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://ft.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pj.nszjky.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rw.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yf.521024.cn

C#:   x.GetType().Name; x is int
来源：http://av.shxzukj.cn

[A05] 整数除法与取模
来源：http://gp.huixiangedu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uk.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hs.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xz.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oi.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://sz.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://pc.nicolike.cn

Ruby: 7 / 2; 7 % 2
来源：http://ev.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://cu.szsharing.cn

[A06] 字符串转数字
来源：http://co.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://vr.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://iu.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hm.hahajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ei.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wp.yuntaijiaju.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://te.huixiangedu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bs.huanxung.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yh.bookmarksfly.cn

[A07] 数字转字符串
来源：http://vq.huanxung.cn

Py:   str(42)
来源：http://cc.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://en.521024.cn

JS:   String(42); (42).toString()
来源：http://le.szxytkj.cn

TS:   String(42)
来源：http://cg.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yf.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://xx.colortex.cn

Ruby: 42.to_s
来源：http://vw.chemitech.net.cn

C#:   42.ToString()
来源：http://vh.nszjky.cn

[A08] 取整与四舍五入
来源：http://iu.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tv.jianghongdianzi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xl.yuntaijiaju.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jk.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hk.hnjuh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tt.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kl.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qk.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://co.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://cb.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vp.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ae.panjiajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ty.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ax.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nf.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gf.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mi.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sj.hnjuh.cn

[A10] 生成随机数
来源：http://rq.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://je.9csxet.cn

PHP:  random_int(1, 100);
来源：http://mq.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cd.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yq.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://uq.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://te.szxytkj.cn

Ruby: rand(1..100)
来源：http://vh.muxihuayi.cn

C#:   new Random().Next(1, 101)
来源：http://jf.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://rg.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://yf.9csxet.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cw.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uq.muxihuayi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lo.asd995.cn

Java: x > 0 ? "yes" : "no"
来源：http://wo.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ut.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vq.huixiangedu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rb.muxihuayi.cn

[A12] 字符串插值 / 格式化
来源：http://vz.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://al.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bu.yuntaijiaju.cn

JS:   `Hello, ${name}!`
来源：http://sk.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://lt.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://mc.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ih.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://xh.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://qs.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dc.huixiangedu.cn

Py:   "第一行\n第二行"
来源：http://dq.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://le.nicolike.cn

JS:   "第一行\n第二行"
来源：http://sh.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://jb.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://ll.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://vy.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://gm.hahajie.cn

C#:   "第一行\n第二行"
来源：http://od.yuexingan06.cn

[A14] 注释写法
来源：http://xk.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pa.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kl.521024.cn

JS:   // 单行；/* 多行 */
来源：http://ur.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://vf.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cp.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://gs.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pd.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://tl.newstarts.cn

[A15] 空值判断与默认值
来源：http://uw.shxzskj.cn

Py:   value = data or "默认值"
来源：http://ps.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://eh.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://qe.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://ja.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ac.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://lf.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://yp.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://iu.szsharing.cn

[A16] 真假值判断规则
来源：http://mj.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jf.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kx.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qp.nszjky.cn

TS:   if (!x) {}
来源：http://si.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://by.shxzskj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mm.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fq.hnjuh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pi.bookmarksfly.cn

[A17] 位运算
来源：http://ci.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kp.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cx.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://th.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qo.szxytkj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yq.huixinmuqiang.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bq.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cn.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gx.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://hf.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://cp.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://ck.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cx.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ae.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://sm.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fn.huanxung.cn

Ruby: "A".ord; 65.chr
来源：http://vi.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://vq.shxzukj.cn

[A19] 交换两个变量
来源：http://cs.shxzukj.cn

Py:   a, b = b, a
来源：http://lu.yuexingan06.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mg.9csxet.cn

JS:   [a, b] = [b, a];
来源：http://vv.521024.cn

TS:   [a, b] = [b, a];
来源：http://sn.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://kz.hnjuh.cn

Go:   a, b = b, a
来源：http://pe.bjjhwx.cn

Ruby: a, b = b, a
来源：http://um.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://ud.521024.cn

[A20] 读取标准输入
来源：http://zj.colortex.cn

Py:   name = input("请输入：")
来源：http://jh.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://up.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jd.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://la.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://hh.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://px.haigaiapp.cn

Ruby: gets.chomp
来源：http://dp.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://pq.newstarts.cn

[A21] 保留指定小数位输出
来源：http://ev.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://kk.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tu.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://dm.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://ee.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://mn.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ud.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://dl.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://nz.9csxet.cn

[A22] 获取字符串长度
来源：http://mw.huixinmuqiang.cn

Py:   len(s)
来源：http://vd.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dz.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uj.wgjwhj.cn

TS:   s.length
来源：http://fq.hahajie.cn

Java: s.length()
来源：http://wm.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gn.yuntaijiaju.cn

Ruby: s.length
来源：http://st.colortex.cn

C#:   s.Length
来源：http://ow.bookmarksfly.cn

[A23] 大小写转换
来源：http://lv.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ii.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rj.shtwfgs.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xg.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bi.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ez.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ut.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lt.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hh.9csxet.cn

[A24] 去除首尾空白
来源：http://xn.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vb.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dd.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ey.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ja.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ua.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://ov.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zt.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jp.chemitech.net.cn

[A25] 字符串比较
来源：http://mp.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://vo.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qs.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pg.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bv.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iy.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vf.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lh.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hg.shxzskj.cn

[A26] 类型转换总览
来源：http://gn.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lo.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ll.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nc.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://ov.huixinmuqiang.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://re.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yu.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ge.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ax.szsharing.cn

================================================================================
来源：http://tm.huixiangedu.cn

B. 流程控制
来源：http://at.colortex.cn

================================================================================
来源：http://su.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://se.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://re.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cz.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nh.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iw.huixinmuqiang.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qs.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wx.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cn.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qj.asd995.cn

[B02] 多分支 else if / elif
来源：http://qw.szsharing.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dk.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xp.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ux.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gc.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kb.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yb.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zn.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ze.shxzukj.cn

[B03] switch / match / case
来源：http://xq.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://to.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://he.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nr.bjjhwx.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aj.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fo.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nf.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uo.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tz.yuexingan06.cn

[B04] for 计数循环
来源：http://bg.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://ol.hnjuh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://no.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tt.haigaiapp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sg.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wj.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ux.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://jd.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vo.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://sb.nicolike.cn

Py:   for item in arr: print(item)
来源：http://xv.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jy.muxihuayi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ai.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lj.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mk.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kf.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://zj.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sk.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://ti.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zu.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hj.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sq.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bx.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vk.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vh.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sc.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ec.9csxet.cn

[B07] while 循环
来源：http://yn.hahajie.cn

Py:   while i < 10: i += 1
来源：http://cc.jianghongdianzi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xx.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://tg.521024.cn

TS:   while (i < 10) { i++; }
来源：http://zm.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://yt.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rg.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://re.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://zk.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://fz.gzmigu.cn


<!-- 参考信息 -->