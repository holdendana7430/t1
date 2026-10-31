代发 wailian999

Py:   print("Hello, World!")
来源：http://zn.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://wo.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://yq.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vg.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://zl.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://mx.521024.cn

Ruby: puts "Hello, World!"
来源：http://tt.panjiajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://te.gzmigu.cn

[A02] 变量声明与赋值
来源：http://sv.yuntaijiaju.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ae.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ov.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dz.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ep.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://vh.yuntaijiaju.cn

Go:   name := "Alex"; age := 20
来源：http://zx.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://sl.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ey.yuexingan06.cn

[A03] 常量定义
来源：http://dw.chemitech.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dy.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://af.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://ce.bjjhwx.cn

TS:   const PI: number = 3.14159;
来源：http://em.muxihuayi.cn

Java: static final double PI = 3.14159;
来源：http://as.newstarts.cn

Go:   const PI = 3.14159
来源：http://yj.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://pc.521024.cn

C#:   const double PI = 3.14159;
来源：http://pr.muxihuayi.cn

[A04] 判断变量类型
来源：http://go.lnxyls.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ef.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tn.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bw.shxzukj.cn

TS:   typeof x; x instanceof Date
来源：http://my.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hs.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uy.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ms.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://dc.panjiajie.cn

[A05] 整数除法与取模
来源：http://dv.chemitech.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zg.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xu.hnjuh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ut.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pa.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://py.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://nf.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://cu.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://ir.hahajie.cn

[A06] 字符串转数字
来源：http://xe.yuntaijiaju.cn

Py:   int("42"); float("3.14")
来源：http://uc.hahajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gm.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ir.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://es.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ad.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gm.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jr.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://th.521024.cn

[A07] 数字转字符串
来源：http://fy.yuntaijiaju.cn

Py:   str(42)
来源：http://je.panjiajie.cn

PHP:  (string) 42; strval(42)
来源：http://ez.nszjky.cn

JS:   String(42); (42).toString()
来源：http://sw.haigaiapp.cn

TS:   String(42)
来源：http://mi.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ib.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://zo.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://lq.szxytkj.cn

C#:   42.ToString()
来源：http://wt.haigaiapp.cn

[A08] 取整与四舍五入
来源：http://bn.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ek.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sv.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zr.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lj.szxytkj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mq.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ti.hahajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://eq.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://el.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://db.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cl.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ro.newstarts.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hv.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bt.9csxet.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sh.szxytkj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://em.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sn.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://at.jianghongdianzi.cn

[A10] 生成随机数
来源：http://lz.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://gg.nicolike.cn

PHP:  random_int(1, 100);
来源：http://yv.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ih.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ee.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://vk.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yh.shxzukj.cn

Ruby: rand(1..100)
来源：http://gm.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://ok.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://ke.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://oi.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://at.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ch.521024.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hm.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://zm.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qg.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kz.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ln.shxzukj.cn

[A12] 字符串插值 / 格式化
来源：http://ad.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sv.hahajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tw.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://lx.nszjky.cn

TS:   `Hello, ${name}!`
来源：http://lp.panjiajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://ih.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rl.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://mt.asd995.cn

C#:   $"Hello, {name}!"
来源：http://pv.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qx.yuexingan06.cn

Py:   "第一行\n第二行"
来源：http://lc.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://bj.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://ae.huanxung.cn

TS:   "第一行\n第二行"
来源：http://yz.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://ki.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://in.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://bf.huanxung.cn

C#:   "第一行\n第二行"
来源：http://ts.yuexingan06.cn

[A14] 注释写法
来源：http://qa.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cc.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cb.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://ro.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://iq.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wm.hahajie.cn

Go:   // 单行；/* 多行 */
来源：http://uk.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dv.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://jw.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://vt.panjiajie.cn

Py:   value = data or "默认值"
来源：http://fg.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://ie.huixinmuqiang.cn

JS:   const value = data ?? "默认值";
来源：http://gs.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://mf.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bu.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://av.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://ax.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://un.huanxung.cn

[A16] 真假值判断规则
来源：http://sn.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sj.lnxyls.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mb.asd995.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sq.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://vq.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ts.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ow.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vl.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uw.hnjuh.cn

[A17] 位运算
来源：http://et.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gk.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dp.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bc.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kf.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zg.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ig.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://al.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jx.shxzukj.cn

[A18] 字符与 ASCII 码互转
来源：http://su.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://nh.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://ze.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rd.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yy.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://vz.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pn.muxihuayi.cn

Ruby: "A".ord; 65.chr
来源：http://pi.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://hy.shxzskj.cn

[A19] 交换两个变量
来源：http://fk.huixiangedu.cn

Py:   a, b = b, a
来源：http://rf.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ys.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://gu.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://os.muxihuayi.cn

Java: int t = a; a = b; b = t;
来源：http://nl.shxzskj.cn

Go:   a, b = b, a
来源：http://ws.shxzskj.cn

Ruby: a, b = b, a
来源：http://xj.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://yp.shxzukj.cn

[A20] 读取标准输入
来源：http://gv.gzmigu.cn

Py:   name = input("请输入：")
来源：http://zj.shxzskj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://st.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xe.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://wq.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://it.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bi.yuexingan06.cn

Ruby: gets.chomp
来源：http://dn.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://ci.newstarts.cn

[A21] 保留指定小数位输出
来源：http://fe.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://su.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vn.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://tg.yuntaijiaju.cn

TS:   (3.14159).toFixed(2)
来源：http://ww.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://bl.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ok.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://mn.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://vi.haigaiapp.cn

[A22] 获取字符串长度
来源：http://an.asd995.cn

Py:   len(s)
来源：http://jz.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yt.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ki.bookmarksfly.cn

TS:   s.length
来源：http://mp.nicolike.cn

Java: s.length()
来源：http://ns.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dk.szxytkj.cn

Ruby: s.length
来源：http://gd.bookmarksfly.cn

C#:   s.Length
来源：http://wk.shxzskj.cn

[A23] 大小写转换
来源：http://wm.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kj.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bs.lnxyls.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://da.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cq.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zy.hahajie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://em.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qy.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yh.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://kf.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hi.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mh.colortex.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fn.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gt.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dj.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://jj.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dw.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rv.hnjuh.cn

[A25] 字符串比较
来源：http://tx.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://hw.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ys.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zp.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rn.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ud.hnjuh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pj.nicolike.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jf.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rd.huanxung.cn

[A26] 类型转换总览
来源：http://gk.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gf.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ow.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uo.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://bp.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ud.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oc.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hc.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tn.nszjky.cn

================================================================================
来源：http://gm.huixinmuqiang.cn

B. 流程控制
来源：http://mk.nicolike.cn

================================================================================
来源：http://xu.nicolike.cn

[B01] 条件判断 if / else
来源：http://zm.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bu.gzmigu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dn.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yw.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vl.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://es.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gk.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://up.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wb.nszjky.cn

[B02] 多分支 else if / elif
来源：http://uu.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ht.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iu.colortex.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://px.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jr.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ek.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nf.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gs.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dg.asd995.cn

[B03] switch / match / case
来源：http://tc.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cx.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jj.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yh.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hx.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://os.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ka.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ir.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ia.asd995.cn

[B04] for 计数循环
来源：http://ne.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://bb.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ta.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://et.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zp.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://as.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qv.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://yr.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bt.shxzskj.cn

[B05] 遍历数组 / 列表
来源：http://ld.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://dc.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cg.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ma.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://re.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ay.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ui.yuexingan06.cn

Ruby: arr.each { |item| puts item }
来源：http://gr.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dc.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://ok.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://we.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ez.szsharing.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ij.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pc.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gq.panjiajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zu.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sl.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wb.hahajie.cn

[B07] while 循环
来源：http://tj.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://vp.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qy.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://ko.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://ed.colortex.cn

Java: while (i < 10) { i++; }
来源：http://bd.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ed.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://if.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://lz.shtwfgs.cn

[B08] do-while（至少执行一次）
来源：http://ir.nicolike.cn


<!-- 参考信息 -->