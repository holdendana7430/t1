代发 wailian999

Py:   print("Hello, World!")
来源：http://fo.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://jm.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://tl.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wm.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://ut.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://nr.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://db.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nb.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://pa.szxytkj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hx.521024.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qb.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ou.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bf.bookmarksfly.cn

Java: String name = "Alex"; int age = 20;
来源：http://ev.nicolike.cn

Go:   name := "Alex"; age := 20
来源：http://kl.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://rs.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kj.huixinmuqiang.cn

[A03] 常量定义
来源：http://pi.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nw.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://lt.huanxung.cn

JS:   const PI = 3.14159;
来源：http://ej.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://rl.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://qh.521024.cn

Go:   const PI = 3.14159
来源：http://st.asd995.cn

Ruby: PI = 3.14159
来源：http://yk.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://tz.bookmarksfly.cn

[A04] 判断变量类型
来源：http://iw.shxzukj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ss.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uq.bookmarksfly.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dr.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://fw.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pd.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hx.newstarts.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ms.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://cs.newstarts.cn

[A05] 整数除法与取模
来源：http://ap.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qa.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wz.asd995.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zh.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hj.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://di.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://rp.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://ey.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://db.shxzskj.cn

[A06] 字符串转数字
来源：http://ac.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://fl.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nv.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://se.shxzukj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xb.9csxet.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qo.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qo.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qr.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jf.jctech888.com.cn

[A07] 数字转字符串
来源：http://xr.nszjky.cn

Py:   str(42)
来源：http://fg.nicolike.cn

PHP:  (string) 42; strval(42)
来源：http://py.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://kj.newstarts.cn

TS:   String(42)
来源：http://yx.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fk.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://bc.newstarts.cn

Ruby: 42.to_s
来源：http://dz.newstarts.cn

C#:   42.ToString()
来源：http://xg.nszjky.cn

[A08] 取整与四舍五入
来源：http://pi.shxzukj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pn.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bv.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yw.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ag.asd995.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fo.yuntaijiaju.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://te.bjjhwx.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zi.newstarts.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tb.wgjwhj.cn

[A09] 绝对值与最大最小值
来源：http://ar.hnjuh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dn.szxytkj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://on.newstarts.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ft.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://aw.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wg.haigaiapp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rn.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zl.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jy.bjjhwx.cn

[A10] 生成随机数
来源：http://oo.huanxung.cn

Py:   import random; random.randint(1, 100)
来源：http://qg.colortex.cn

PHP:  random_int(1, 100);
来源：http://me.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hr.lnxyls.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kz.lnxyls.cn

Java: new Random().nextInt(100) + 1
来源：http://qq.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://by.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://ax.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://uq.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://zh.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://jm.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mv.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fw.panjiajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://en.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://us.bjjhwx.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qn.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://dm.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://am.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://pm.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fb.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ro.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://wx.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://dz.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://zm.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yw.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://pn.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://aw.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ep.asd995.cn

Py:   "第一行\n第二行"
来源：http://wr.shtwfgs.cn

PHP:  "第一行\n第二行"
来源：http://gn.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://dc.panjiajie.cn

TS:   "第一行\n第二行"
来源：http://to.gzmigu.cn

Java: "第一行\n第二行"
来源：http://wj.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://va.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://po.shtwfgs.cn

C#:   "第一行\n第二行"
来源：http://su.yuntaijiaju.cn

[A14] 注释写法
来源：http://hr.huanxung.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://km.shxzskj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ji.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://nd.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://eh.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xa.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://bd.shxzukj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wa.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://qt.newstarts.cn

[A15] 空值判断与默认值
来源：http://jo.colortex.cn

Py:   value = data or "默认值"
来源：http://fu.hnjuh.cn

PHP:  $value = $data ?? "默认值";
来源：http://ck.shtwfgs.cn

JS:   const value = data ?? "默认值";
来源：http://wh.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://mk.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ma.nszjky.cn

Go:   if data == "" { data = "默认值" }
来源：http://ww.wgjwhj.cn

Ruby: value = data || "默认值"
来源：http://bc.nszjky.cn

C#:   var value = data ?? "默认值";
来源：http://js.nicolike.cn

[A16] 真假值判断规则
来源：http://ce.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ew.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://km.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fd.jctech888.com.cn

TS:   if (!x) {}
来源：http://ls.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kj.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bk.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://um.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gw.521024.cn

[A17] 位运算
来源：http://cc.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ho.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ic.yuntaijiaju.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zg.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ln.haigaiapp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zl.lnxyls.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jk.huixinmuqiang.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kb.wgjwhj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vf.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://bf.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://lo.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://iw.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ni.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zz.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://uc.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xs.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://rb.szxytkj.cn

C#:   (int)'A'; (char)65
来源：http://dc.jctech888.com.cn

[A19] 交换两个变量
来源：http://pt.yuexingan06.cn

Py:   a, b = b, a
来源：http://os.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dw.hnjuh.cn

JS:   [a, b] = [b, a];
来源：http://tl.yuexingan06.cn

TS:   [a, b] = [b, a];
来源：http://bb.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://oy.521024.cn

Go:   a, b = b, a
来源：http://mn.huanxung.cn

Ruby: a, b = b, a
来源：http://du.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://oy.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://mj.szxytkj.cn

Py:   name = input("请输入：")
来源：http://bw.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ze.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ki.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://zk.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://aj.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nm.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://oa.hnjuh.cn

C#:   Console.ReadLine();
来源：http://uo.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://nl.hahajie.cn

Py:   f"{3.14159:.2f}"
来源：http://qk.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jr.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://ui.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://em.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://yn.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wa.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://wq.wgjwhj.cn

C#:   3.14159.ToString("F2")
来源：http://ni.shxzskj.cn

[A22] 获取字符串长度
来源：http://ol.nicolike.cn

Py:   len(s)
来源：http://lo.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dh.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hm.shxzukj.cn

TS:   s.length
来源：http://ui.hahajie.cn

Java: s.length()
来源：http://pu.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bk.chemitech.net.cn

Ruby: s.length
来源：http://mn.chemitech.net.cn

C#:   s.Length
来源：http://vl.huixinmuqiang.cn

[A23] 大小写转换
来源：http://nv.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://iw.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pb.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qq.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ll.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qp.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gc.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bv.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://om.bjjhwx.cn

[A24] 去除首尾空白
来源：http://xc.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lw.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://it.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cj.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ru.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ug.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://mi.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wt.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://im.asd995.cn

[A25] 字符串比较
来源：http://dm.chemitech.net.cn

Py:   s1 == s2; s1 != s2
来源：http://fv.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mt.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pm.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rb.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sa.lnxyls.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jy.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pb.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ex.nszjky.cn

[A26] 类型转换总览
来源：http://yw.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gx.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ox.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rg.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://wr.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wg.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ff.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://eb.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vs.huixinmuqiang.cn

================================================================================
来源：http://ky.asd995.cn

B. 流程控制
来源：http://ge.panjiajie.cn

================================================================================
来源：http://pa.nicolike.cn

[B01] 条件判断 if / else
来源：http://xg.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uk.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lf.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dv.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qd.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vl.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sw.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wt.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fb.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://rg.nicolike.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://km.haigaiapp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lz.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dt.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fd.panjiajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://py.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sj.nicolike.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mv.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ai.huanxung.cn

[B03] switch / match / case
来源：http://kf.hahajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oa.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://su.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hs.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ok.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ab.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ay.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ov.nicolike.cn

[B04] for 计数循环
来源：http://ut.colortex.cn

Py:   for i in range(10): print(i)
来源：http://ea.lnxyls.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nu.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jm.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vy.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yt.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xr.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://ql.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://na.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://by.9csxet.cn

Py:   for item in arr: print(item)
来源：http://ce.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ik.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kn.asd995.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ae.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xy.lnxyls.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tt.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://hl.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jp.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://ox.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dl.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oz.panjiajie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mg.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://re.asd995.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rl.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qu.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aw.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qd.newstarts.cn

[B07] while 循环
来源：http://hl.asd995.cn

Py:   while i < 10: i += 1
来源：http://cn.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ez.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://pb.hnjuh.cn

TS:   while (i < 10) { i++; }
来源：http://ga.yuexingan06.cn

Java: while (i < 10) { i++; }
来源：http://lw.shxzskj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bq.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://lh.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://tt.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://pz.yuntaijiaju.cn


<!-- 参考信息 -->