代发 wailian999

Py:   print("Hello, World!")
来源：http://kn.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://uq.wgjwhj.cn

JS:   console.log("Hello, World!");
来源：http://yj.bookmarksfly.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vv.yuexingan06.cn

Java: System.out.println("Hello, World!");
来源：http://yh.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://pt.bookmarksfly.cn

Ruby: puts "Hello, World!"
来源：http://dy.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sp.newstarts.cn

[A02] 变量声明与赋值
来源：http://xj.9csxet.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nx.szxytkj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vu.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qx.jianghongdianzi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jc.wgjwhj.cn

Java: String name = "Alex"; int age = 20;
来源：http://ab.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://ao.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://xu.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ly.nicolike.cn

[A03] 常量定义
来源：http://wi.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yj.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://ia.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://oh.521024.cn

TS:   const PI: number = 3.14159;
来源：http://yr.asd995.cn

Java: static final double PI = 3.14159;
来源：http://yi.panjiajie.cn

Go:   const PI = 3.14159
来源：http://qb.shxzukj.cn

Ruby: PI = 3.14159
来源：http://nl.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://nq.jctech888.com.cn

[A04] 判断变量类型
来源：http://sr.chemitech.net.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rn.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://he.521024.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xv.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://lx.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dd.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yr.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://cn.muxihuayi.cn

C#:   x.GetType().Name; x is int
来源：http://xy.gzmigu.cn

[A05] 整数除法与取模
来源：http://hb.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ja.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://aq.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nl.chemitech.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dc.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://xm.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://zd.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://mn.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://ac.asd995.cn

[A06] 字符串转数字
来源：http://cm.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://xm.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ha.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eq.9csxet.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ae.haigaiapp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://an.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sx.chemitech.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://if.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tu.9csxet.cn

[A07] 数字转字符串
来源：http://lk.nszjky.cn

Py:   str(42)
来源：http://mc.jianghongdianzi.cn

PHP:  (string) 42; strval(42)
来源：http://df.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://gp.9csxet.cn

TS:   String(42)
来源：http://ca.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ab.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://dw.muxihuayi.cn

Ruby: 42.to_s
来源：http://ul.bjjhwx.cn

C#:   42.ToString()
来源：http://go.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://jy.yuntaijiaju.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xn.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vu.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://in.9csxet.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://on.huixinmuqiang.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://om.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eb.huanxung.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://px.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pc.haigaiapp.cn

[A09] 绝对值与最大最小值
来源：http://wm.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xg.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sy.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mg.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ip.wgjwhj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://id.szxytkj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ke.jianghongdianzi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nz.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eg.chemitech.net.cn

[A10] 生成随机数
来源：http://wu.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://fi.521024.cn

PHP:  random_int(1, 100);
来源：http://bd.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ab.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gt.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://aj.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cg.nicolike.cn

Ruby: rand(1..100)
来源：http://zz.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://bc.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://tl.szxytkj.cn

Py:   "yes" if x > 0 else "no"
来源：http://hh.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pa.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dz.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://eb.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://ri.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qp.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fr.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ey.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://lf.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://le.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yc.nszjky.cn

JS:   `Hello, ${name}!`
来源：http://dy.colortex.cn

TS:   `Hello, ${name}!`
来源：http://de.huanxung.cn

Java: "Hello, %s!".formatted(name)
来源：http://cs.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ef.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://hb.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://am.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ju.szsharing.cn

Py:   "第一行\n第二行"
来源：http://nd.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://oi.hahajie.cn

JS:   "第一行\n第二行"
来源：http://gy.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://en.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://cb.colortex.cn

Go:   "第一行\n第二行"
来源：http://lw.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://sj.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://el.newstarts.cn

[A14] 注释写法
来源：http://qa.hnjuh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yh.muxihuayi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ii.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://or.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://nk.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://by.huixiangedu.cn

Go:   // 单行；/* 多行 */
来源：http://uh.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ms.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://tk.9csxet.cn

[A15] 空值判断与默认值
来源：http://rz.521024.cn

Py:   value = data or "默认值"
来源：http://nj.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://aw.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://wb.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://wx.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kk.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://si.521024.cn

Ruby: value = data || "默认值"
来源：http://fh.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://bo.huixiangedu.cn

[A16] 真假值判断规则
来源：http://fh.huixinmuqiang.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vv.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tw.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yj.wgjwhj.cn

TS:   if (!x) {}
来源：http://ov.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xu.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gb.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zd.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tc.bjjhwx.cn

[A17] 位运算
来源：http://gb.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ye.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fr.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mm.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kv.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hy.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oi.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ma.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wq.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://gh.jctech888.com.cn

Py:   ord("A"); chr(65)
来源：http://lv.huixinmuqiang.cn

PHP:  ord("A"); chr(65)
来源：http://ul.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zl.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ou.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://sr.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dk.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://kh.panjiajie.cn

C#:   (int)'A'; (char)65
来源：http://si.huixiangedu.cn

[A19] 交换两个变量
来源：http://bw.huanxung.cn

Py:   a, b = b, a
来源：http://su.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jo.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://la.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://vz.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://qz.colortex.cn

Go:   a, b = b, a
来源：http://ko.chemitech.net.cn

Ruby: a, b = b, a
来源：http://cu.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://xe.bjjhwx.cn

[A20] 读取标准输入
来源：http://hv.shxzukj.cn

Py:   name = input("请输入：")
来源：http://lk.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yj.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lo.asd995.cn

TS:   // Node.js：readline 模块
来源：http://na.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://wi.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ky.jctech888.com.cn

Ruby: gets.chomp
来源：http://qa.asd995.cn

C#:   Console.ReadLine();
来源：http://zz.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://jq.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://jq.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://er.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://qz.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://jc.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://iv.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uq.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://el.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://cv.bjjhwx.cn

[A22] 获取字符串长度
来源：http://ys.wgjwhj.cn

Py:   len(s)
来源：http://jc.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kj.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vm.huixiangedu.cn

TS:   s.length
来源：http://sr.hnjuh.cn

Java: s.length()
来源：http://ef.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yu.haigaiapp.cn

Ruby: s.length
来源：http://xx.shxzukj.cn

C#:   s.Length
来源：http://sm.panjiajie.cn

[A23] 大小写转换
来源：http://nn.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bc.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ff.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hd.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lj.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jb.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hj.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ri.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gk.newstarts.cn

[A24] 去除首尾空白
来源：http://bp.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jm.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vd.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tv.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cu.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://au.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://xq.huixiangedu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xi.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dc.yuexingan06.cn

[A25] 字符串比较
来源：http://zi.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://tu.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ti.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xe.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uu.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://de.huixinmuqiang.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ux.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ty.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zh.lnxyls.cn

[A26] 类型转换总览
来源：http://ut.521024.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qp.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pn.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gn.chemitech.net.cn

TS:   Number() String() Boolean() x as number
来源：http://wh.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://am.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bu.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lq.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hg.huanxung.cn

================================================================================
来源：http://wg.jianghongdianzi.cn

B. 流程控制
来源：http://pc.nicolike.cn

================================================================================
来源：http://aw.huanxung.cn

[B01] 条件判断 if / else
来源：http://lb.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lr.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zb.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tf.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://br.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zu.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wf.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lp.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://os.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://ir.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lw.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yc.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zr.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yh.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ug.bookmarksfly.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rg.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xl.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://er.shxzskj.cn

[B03] switch / match / case
来源：http://fs.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zd.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cd.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pp.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vl.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rr.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cb.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hv.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ri.nicolike.cn

[B04] for 计数循环
来源：http://yb.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://zv.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fb.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vk.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gt.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gc.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eh.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://jy.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ac.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://hs.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://pk.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://js.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tp.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ml.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dq.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kc.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://ig.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vv.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://qs.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tx.gzmigu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://us.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vf.9csxet.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ks.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xn.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tl.yuntaijiaju.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kw.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zp.haigaiapp.cn

[B07] while 循环
来源：http://fx.huanxung.cn

Py:   while i < 10: i += 1
来源：http://uk.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sr.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://xc.huanxung.cn

TS:   while (i < 10) { i++; }
来源：http://jf.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://pd.nszjky.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://by.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://ad.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://ho.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://af.hnjuh.cn


<!-- 参考信息 -->