代发 wailian999

Py:   print("Hello, World!")
来源：http://qh.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://ll.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://qk.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rj.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://me.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://an.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://bg.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ua.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://sf.jianghongdianzi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mz.haigaiapp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ta.huixiangedu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xg.colortex.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mv.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://km.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://vs.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://kb.yuexingan06.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cn.chemitech.net.cn

[A03] 常量定义
来源：http://jc.muxihuayi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vx.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://et.bjjhwx.cn

JS:   const PI = 3.14159;
来源：http://ru.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://cd.haigaiapp.cn

Java: static final double PI = 3.14159;
来源：http://sm.shxzukj.cn

Go:   const PI = 3.14159
来源：http://th.hnjuh.cn

Ruby: PI = 3.14159
来源：http://ei.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://gc.gzmigu.cn

[A04] 判断变量类型
来源：http://wc.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pq.lnxyls.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lo.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lk.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://zr.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tk.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cv.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jd.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://qc.panjiajie.cn

[A05] 整数除法与取模
来源：http://mi.gzmigu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sb.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vc.yuntaijiaju.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ki.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://km.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://xy.bjjhwx.cn

Go:   7 / 2; 7 % 2
来源：http://ya.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://ei.yuexingan06.cn

C#:   7 / 2; 7 % 2
来源：http://um.nszjky.cn

[A06] 字符串转数字
来源：http://nz.panjiajie.cn

Py:   int("42"); float("3.14")
来源：http://gs.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yt.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gp.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mo.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nm.colortex.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qo.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jk.chemitech.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tv.521024.cn

[A07] 数字转字符串
来源：http://xn.chemitech.net.cn

Py:   str(42)
来源：http://qm.panjiajie.cn

PHP:  (string) 42; strval(42)
来源：http://oc.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://lw.huixiangedu.cn

TS:   String(42)
来源：http://tr.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fy.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://cl.nicolike.cn

Ruby: 42.to_s
来源：http://kf.lnxyls.cn

C#:   42.ToString()
来源：http://th.521024.cn

[A08] 取整与四舍五入
来源：http://xf.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rh.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zk.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vw.9csxet.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://je.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://le.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lq.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fy.jctech888.com.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zk.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://ms.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ds.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://by.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nh.colortex.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://of.wgjwhj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dl.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gl.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vm.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jp.hahajie.cn

[A10] 生成随机数
来源：http://mx.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://cw.yuntaijiaju.cn

PHP:  random_int(1, 100);
来源：http://hi.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rt.nicolike.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cr.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://rs.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zk.hnjuh.cn

Ruby: rand(1..100)
来源：http://rn.huixiangedu.cn

C#:   new Random().Next(1, 101)
来源：http://yg.colortex.cn

[A11] 条件表达式（三元）
来源：http://np.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://if.colortex.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://go.panjiajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ab.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sq.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://md.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rd.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://bv.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://dw.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://by.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ax.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vu.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://lh.huixinmuqiang.cn

TS:   `Hello, ${name}!`
来源：http://nv.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://mp.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uv.huanxung.cn

Ruby: "Hello, #{name}!"
来源：http://oc.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://ml.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://au.huixinmuqiang.cn

Py:   "第一行\n第二行"
来源：http://wf.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://gg.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://wd.521024.cn

TS:   "第一行\n第二行"
来源：http://qu.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://bo.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://hx.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://pz.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://uu.9csxet.cn

[A14] 注释写法
来源：http://ie.huanxung.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rt.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://og.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://xy.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://ut.szxytkj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bh.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://ba.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tu.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://wc.szsharing.cn

[A15] 空值判断与默认值
来源：http://yq.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://dp.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://iw.huixinmuqiang.cn

JS:   const value = data ?? "默认值";
来源：http://gb.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://ii.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ak.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://um.nicolike.cn

Ruby: value = data || "默认值"
来源：http://qt.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://oz.huixiangedu.cn

[A16] 真假值判断规则
来源：http://gs.haigaiapp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uq.asd995.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ck.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hm.bjjhwx.cn

TS:   if (!x) {}
来源：http://gq.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tx.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ry.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mb.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pd.bjjhwx.cn

[A17] 位运算
来源：http://jf.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fo.haigaiapp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zb.gzmigu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uj.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xy.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zf.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kc.newstarts.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yd.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iy.panjiajie.cn

[A18] 字符与 ASCII 码互转
来源：http://ye.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://wa.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://ex.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kg.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mm.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://ci.521024.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://os.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://rc.szxytkj.cn

C#:   (int)'A'; (char)65
来源：http://qr.shxzskj.cn

[A19] 交换两个变量
来源：http://yy.yuntaijiaju.cn

Py:   a, b = b, a
来源：http://an.521024.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://oy.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://dd.colortex.cn

TS:   [a, b] = [b, a];
来源：http://co.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://nn.hahajie.cn

Go:   a, b = b, a
来源：http://kx.newstarts.cn

Ruby: a, b = b, a
来源：http://dm.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://dt.newstarts.cn

[A20] 读取标准输入
来源：http://bn.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://ep.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://py.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rw.colortex.cn

TS:   // Node.js：readline 模块
来源：http://fe.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://xn.newstarts.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bq.colortex.cn

Ruby: gets.chomp
来源：http://dw.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://tw.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://qi.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://xs.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xm.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://zx.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://qy.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://vp.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fs.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://xe.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://vj.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://ju.wgjwhj.cn

Py:   len(s)
来源：http://en.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rx.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lr.shxzskj.cn

TS:   s.length
来源：http://fj.gzmigu.cn

Java: s.length()
来源：http://lf.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uc.bookmarksfly.cn

Ruby: s.length
来源：http://is.shxzukj.cn

C#:   s.Length
来源：http://zz.jianghongdianzi.cn

[A23] 大小写转换
来源：http://xe.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zp.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ly.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fp.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fx.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tt.9csxet.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tm.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cz.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://um.wgjwhj.cn

[A24] 去除首尾空白
来源：http://wx.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mp.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://av.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ff.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sd.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://aw.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://yx.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xu.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nr.shxzukj.cn

[A25] 字符串比较
来源：http://if.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://rl.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://os.muxihuayi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fy.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gm.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bg.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uc.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fg.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vp.nicolike.cn

[A26] 类型转换总览
来源：http://xm.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zr.colortex.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bx.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hl.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://zf.jianghongdianzi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://es.hnjuh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jp.yuntaijiaju.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://aa.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zb.haigaiapp.cn

================================================================================
来源：http://zw.newstarts.cn

B. 流程控制
来源：http://wx.huixinmuqiang.cn

================================================================================
来源：http://ms.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://vo.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ok.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://km.huixinmuqiang.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rj.jctech888.com.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zs.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://bn.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mt.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tr.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pf.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://rp.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hx.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nb.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://al.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yy.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eb.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ix.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nd.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ms.521024.cn

[B03] switch / match / case
来源：http://bo.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pk.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wi.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kl.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qu.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://go.wgjwhj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ci.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gr.haigaiapp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zv.yuexingan06.cn

[B04] for 计数循环
来源：http://lf.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://im.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rp.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qc.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qv.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lm.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://af.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://pc.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mr.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://eq.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://fe.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ea.521024.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oo.panjiajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yc.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://er.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qu.chemitech.net.cn

Ruby: arr.each { |item| puts item }
来源：http://wh.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lz.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://im.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pj.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mx.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pi.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wm.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zq.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uk.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sn.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bg.huixinmuqiang.cn

[B07] while 循环
来源：http://sf.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://ic.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yj.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://in.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://sr.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://cv.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ch.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://uv.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://do.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://lv.szxytkj.cn


<!-- 参考信息 -->