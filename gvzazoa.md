代发 wailian999

Py:   print("Hello, World!")
来源：http://tw.hahajie.cn

PHP:  echo "Hello, World!";
来源：http://hy.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://ou.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fd.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://gp.jianghongdianzi.cn

Go:   fmt.Println("Hello, World!")
来源：http://hh.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://ja.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://co.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://mi.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://aq.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gs.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mj.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oa.bookmarksfly.cn

Java: String name = "Alex"; int age = 20;
来源：http://jf.yuntaijiaju.cn

Go:   name := "Alex"; age := 20
来源：http://vw.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://va.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jx.shtwfgs.cn

[A03] 常量定义
来源：http://cy.nszjky.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xo.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://jt.huanxung.cn

JS:   const PI = 3.14159;
来源：http://mc.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://kh.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://aq.yuexingan06.cn

Go:   const PI = 3.14159
来源：http://bf.huixiangedu.cn

Ruby: PI = 3.14159
来源：http://if.bjjhwx.cn

C#:   const double PI = 3.14159;
来源：http://ji.shxzukj.cn

[A04] 判断变量类型
来源：http://fm.huixinmuqiang.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ii.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hq.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gn.muxihuayi.cn

TS:   typeof x; x instanceof Date
来源：http://qz.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xl.asd995.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pt.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vg.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://dc.9csxet.cn

[A05] 整数除法与取模
来源：http://ma.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bz.haigaiapp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ku.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ur.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ew.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://tn.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://yq.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://iy.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://kx.nicolike.cn

[A06] 字符串转数字
来源：http://yz.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://wo.hnjuh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pr.muxihuayi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hk.gzmigu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yr.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ws.jianghongdianzi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uj.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nc.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://el.nszjky.cn

[A07] 数字转字符串
来源：http://ov.panjiajie.cn

Py:   str(42)
来源：http://tb.shxzukj.cn

PHP:  (string) 42; strval(42)
来源：http://wc.szxytkj.cn

JS:   String(42); (42).toString()
来源：http://oa.yuexingan06.cn

TS:   String(42)
来源：http://dl.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jn.nszjky.cn

Go:   strconv.Itoa(42)
来源：http://ce.muxihuayi.cn

Ruby: 42.to_s
来源：http://fs.shxzskj.cn

C#:   42.ToString()
来源：http://dz.panjiajie.cn

[A08] 取整与四舍五入
来源：http://pp.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://um.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ui.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://de.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://di.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qp.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wb.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xj.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ma.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://wo.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xv.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qd.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sy.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://no.yuntaijiaju.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lp.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://on.lnxyls.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sd.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qy.szsharing.cn

[A10] 生成随机数
来源：http://wz.bookmarksfly.cn

Py:   import random; random.randint(1, 100)
来源：http://pj.521024.cn

PHP:  random_int(1, 100);
来源：http://ui.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ar.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vo.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://io.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yl.colortex.cn

Ruby: rand(1..100)
来源：http://qm.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://lg.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://hc.yuexingan06.cn

Py:   "yes" if x > 0 else "no"
来源：http://zp.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wb.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zy.haigaiapp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lc.yuexingan06.cn

Java: x > 0 ? "yes" : "no"
来源：http://pz.huixinmuqiang.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bc.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sm.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://oq.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://lf.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lt.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bw.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://ia.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://qr.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://af.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eq.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://os.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://hg.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vw.521024.cn

Py:   "第一行\n第二行"
来源：http://sn.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://dp.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://gy.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://aq.hahajie.cn

Java: "第一行\n第二行"
来源：http://nv.colortex.cn

Go:   "第一行\n第二行"
来源：http://yd.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://ay.asd995.cn

C#:   "第一行\n第二行"
来源：http://kb.bookmarksfly.cn

[A14] 注释写法
来源：http://uh.bjjhwx.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fh.9csxet.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vl.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://vh.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://vk.newstarts.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pd.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://vv.chemitech.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gx.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://wm.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://by.asd995.cn

Py:   value = data or "默认值"
来源：http://yp.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://co.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://cn.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://fk.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ni.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://tc.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://ua.huixinmuqiang.cn

C#:   var value = data ?? "默认值";
来源：http://im.muxihuayi.cn

[A16] 真假值判断规则
来源：http://hq.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://co.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ms.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zp.chemitech.net.cn

TS:   if (!x) {}
来源：http://hd.bookmarksfly.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bm.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ih.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://sf.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jm.huixiangedu.cn

[A17] 位运算
来源：http://ym.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kb.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gs.hahajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ji.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pp.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ee.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jz.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nf.yuntaijiaju.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ds.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://uv.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://bm.hahajie.cn

PHP:  ord("A"); chr(65)
来源：http://sg.521024.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nn.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://an.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://qy.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lh.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://xq.521024.cn

C#:   (int)'A'; (char)65
来源：http://cw.bjjhwx.cn

[A19] 交换两个变量
来源：http://aw.huixiangedu.cn

Py:   a, b = b, a
来源：http://zw.521024.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qw.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://jt.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://xr.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://cg.wgjwhj.cn

Go:   a, b = b, a
来源：http://ku.shxzukj.cn

Ruby: a, b = b, a
来源：http://ht.bookmarksfly.cn

C#:   (a, b) = (b, a);
来源：http://na.asd995.cn

[A20] 读取标准输入
来源：http://gs.nicolike.cn

Py:   name = input("请输入：")
来源：http://gb.colortex.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nn.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fb.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://hh.huanxung.cn

Java: new Scanner(System.in).nextLine()
来源：http://zv.chemitech.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sr.hahajie.cn

Ruby: gets.chomp
来源：http://ta.shxzukj.cn

C#:   Console.ReadLine();
来源：http://ki.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://kz.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://va.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mz.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://vs.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://ny.hahajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://hc.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ho.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://ku.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://yd.nicolike.cn

[A22] 获取字符串长度
来源：http://hs.bookmarksfly.cn

Py:   len(s)
来源：http://ws.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lv.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nw.gzmigu.cn

TS:   s.length
来源：http://lf.szxytkj.cn

Java: s.length()
来源：http://nr.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://le.panjiajie.cn

Ruby: s.length
来源：http://sl.shxzukj.cn

C#:   s.Length
来源：http://jk.panjiajie.cn

[A23] 大小写转换
来源：http://ty.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sr.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://if.lnxyls.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vy.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rb.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bz.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fx.wgjwhj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vv.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qa.huanxung.cn

[A24] 去除首尾空白
来源：http://sk.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fh.shtwfgs.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kn.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lg.panjiajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vh.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ft.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://qt.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fe.yuntaijiaju.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ah.huixiangedu.cn

[A25] 字符串比较
来源：http://uf.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://hf.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yg.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uu.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dv.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://se.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nq.shxzukj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://co.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yl.colortex.cn

[A26] 类型转换总览
来源：http://xv.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://df.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ka.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mz.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://xi.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://de.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tc.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pa.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ux.9csxet.cn

================================================================================
来源：http://dr.shxzukj.cn

B. 流程控制
来源：http://sn.yuntaijiaju.cn

================================================================================
来源：http://cb.hnjuh.cn

[B01] 条件判断 if / else
来源：http://dc.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jr.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tp.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://in.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ts.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jm.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oz.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sg.huanxung.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tb.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://cj.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hc.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fv.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://my.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qd.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ab.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xv.shxzukj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rq.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jn.shxzskj.cn

[B03] switch / match / case
来源：http://ul.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rb.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yq.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bu.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rq.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ff.bjjhwx.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vt.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rf.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pe.yuntaijiaju.cn

[B04] for 计数循环
来源：http://ci.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://bw.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cu.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fv.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ld.huanxung.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yn.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vt.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://ue.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://el.hahajie.cn

[B05] 遍历数组 / 列表
来源：http://cv.newstarts.cn

Py:   for item in arr: print(item)
来源：http://wo.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qr.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://az.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ft.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xq.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mz.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://mx.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pv.colortex.cn

[B06] 遍历字典 / 对象
来源：http://vt.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lz.shxzskj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tr.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qh.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wk.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ig.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jh.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nb.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ua.haigaiapp.cn

[B07] while 循环
来源：http://uf.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://gw.bjjhwx.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qy.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://qo.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://wu.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://kd.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://st.nszjky.cn

Ruby: while i < 10; i += 1; end
来源：http://tj.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://bm.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://zf.gzmigu.cn


<!-- 参考信息 -->