代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://ya.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bq.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ok.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rj.asd995.cn

================================================================================
来源：http://un.nszjky.cn

A. 基础语法与类型
来源：http://dw.hahajie.cn

================================================================================
来源：http://vs.shtwfgs.cn

[A01] Hello World
来源：http://jt.haigaiapp.cn

Py:   print("Hello, World!")
来源：http://pz.521024.cn

PHP:  echo "Hello, World!";
来源：http://xr.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://vh.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oc.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://xk.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://il.521024.cn

Ruby: puts "Hello, World!"
来源：http://jq.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cv.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://sv.nicolike.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wh.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bl.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jf.gzmigu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ql.jctech888.com.cn

Java: String name = "Alex"; int age = 20;
来源：http://ai.bjjhwx.cn

Go:   name := "Alex"; age := 20
来源：http://gr.jianghongdianzi.cn

Ruby: name = "Alex"; age = 20
来源：http://nc.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fe.nszjky.cn

[A03] 常量定义
来源：http://vk.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vr.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://gk.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://xj.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://qt.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://lc.lnxyls.cn

Go:   const PI = 3.14159
来源：http://mt.lnxyls.cn

Ruby: PI = 3.14159
来源：http://wq.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://za.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://uo.shtwfgs.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://as.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ml.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xu.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://hi.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cd.hnjuh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jv.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bp.wgjwhj.cn

C#:   x.GetType().Name; x is int
来源：http://cp.yuexingan06.cn

[A05] 整数除法与取模
来源：http://sx.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ah.jctech888.com.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://im.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cj.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://da.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://cx.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://db.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://bu.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://ju.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://kv.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://eq.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ox.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kq.wgjwhj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qh.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://au.muxihuayi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bt.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wh.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://il.hnjuh.cn

[A07] 数字转字符串
来源：http://cr.szxytkj.cn

Py:   str(42)
来源：http://gl.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://kb.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://se.huixinmuqiang.cn

TS:   String(42)
来源：http://fe.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ws.huixinmuqiang.cn

Go:   strconv.Itoa(42)
来源：http://tw.chemitech.net.cn

Ruby: 42.to_s
来源：http://wc.asd995.cn

C#:   42.ToString()
来源：http://zz.521024.cn

[A08] 取整与四舍五入
来源：http://gm.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zn.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ri.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xn.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pb.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vo.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ec.hnjuh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ha.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rl.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://hj.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nd.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://at.hahajie.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bj.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://in.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yk.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sz.yuexingan06.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bp.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wb.shxzukj.cn

[A10] 生成随机数
来源：http://kv.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://bz.hahajie.cn

PHP:  random_int(1, 100);
来源：http://qc.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fn.jianghongdianzi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ig.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://pd.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rp.huanxung.cn

Ruby: rand(1..100)
来源：http://gy.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://ry.shtwfgs.cn

[A11] 条件表达式（三元）
来源：http://yt.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://pg.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bb.newstarts.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ge.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://em.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://yk.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ov.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ee.huanxung.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ue.shxzskj.cn

[A12] 字符串插值 / 格式化
来源：http://zv.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zl.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ws.huixiangedu.cn

JS:   `Hello, ${name}!`
来源：http://yw.nicolike.cn

TS:   `Hello, ${name}!`
来源：http://rh.huixinmuqiang.cn

Java: "Hello, %s!".formatted(name)
来源：http://vh.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fg.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://my.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://gf.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tn.huanxung.cn

Py:   "第一行\n第二行"
来源：http://uh.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://gb.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://pg.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://ad.newstarts.cn

Java: "第一行\n第二行"
来源：http://ep.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://bw.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://ft.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://wu.lnxyls.cn

[A14] 注释写法
来源：http://cv.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yv.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://re.nicolike.cn

JS:   // 单行；/* 多行 */
来源：http://ir.panjiajie.cn

TS:   // 单行；/* 多行 */
来源：http://cz.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gp.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://dh.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rc.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://cf.shxzukj.cn

[A15] 空值判断与默认值
来源：http://ac.gzmigu.cn

Py:   value = data or "默认值"
来源：http://ts.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://cs.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://sy.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://si.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cj.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://ze.huixiangedu.cn

Ruby: value = data || "默认值"
来源：http://zu.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://bv.colortex.cn

[A16] 真假值判断规则
来源：http://bj.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qs.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yw.shtwfgs.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ni.hnjuh.cn

TS:   if (!x) {}
来源：http://rw.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mb.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pd.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dd.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ff.haigaiapp.cn

[A17] 位运算
来源：http://xs.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uu.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mj.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qs.hnjuh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zl.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lj.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zx.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wt.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cd.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://cv.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://cx.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://vl.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mw.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ng.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://bp.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jt.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://bp.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://ww.szxytkj.cn

[A19] 交换两个变量
来源：http://pb.lnxyls.cn

Py:   a, b = b, a
来源：http://dx.jianghongdianzi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ax.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://go.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://ek.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://sc.gzmigu.cn

Go:   a, b = b, a
来源：http://gn.nszjky.cn

Ruby: a, b = b, a
来源：http://la.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://xz.hahajie.cn

[A20] 读取标准输入
来源：http://bl.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://op.huixinmuqiang.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://df.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lj.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://yz.gzmigu.cn

Java: new Scanner(System.in).nextLine()
来源：http://qy.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eh.yuexingan06.cn

Ruby: gets.chomp
来源：http://jm.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://bx.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://gj.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://fi.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jy.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://lt.bookmarksfly.cn

TS:   (3.14159).toFixed(2)
来源：http://ip.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://op.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xs.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://hd.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://ka.huixiangedu.cn

[A22] 获取字符串长度
来源：http://nj.szsharing.cn

Py:   len(s)
来源：http://nh.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nw.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ad.shxzskj.cn

TS:   s.length
来源：http://yq.muxihuayi.cn

Java: s.length()
来源：http://uh.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gu.huixinmuqiang.cn

Ruby: s.length
来源：http://fd.shxzskj.cn

C#:   s.Length
来源：http://yj.nszjky.cn

[A23] 大小写转换
来源：http://hi.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ym.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mu.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ss.bookmarksfly.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xm.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xc.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://na.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kv.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ls.nicolike.cn

[A24] 去除首尾空白
来源：http://xf.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rq.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wt.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lq.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cy.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cm.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://ay.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vc.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wt.haigaiapp.cn

[A25] 字符串比较
来源：http://fk.nszjky.cn

Py:   s1 == s2; s1 != s2
来源：http://gv.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oj.nicolike.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hk.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vj.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wo.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cj.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ix.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vi.szxytkj.cn

[A26] 类型转换总览
来源：http://zz.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cp.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wr.bjjhwx.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://li.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://ti.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vi.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bu.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://of.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wr.szxytkj.cn

================================================================================
来源：http://ao.panjiajie.cn

B. 流程控制
来源：http://nd.bookmarksfly.cn

================================================================================
来源：http://de.hahajie.cn

[B01] 条件判断 if / else
来源：http://ba.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ge.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://li.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kx.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wx.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qh.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ur.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lw.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uv.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://hj.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ai.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rn.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://li.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fg.newstarts.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://of.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wt.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gs.szsharing.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wl.huanxung.cn

[B03] switch / match / case
来源：http://lb.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vi.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wc.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dy.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ar.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cg.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hb.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://iu.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lo.panjiajie.cn

[B04] for 计数循环
来源：http://bh.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://zv.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://st.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vk.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://js.bookmarksfly.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ye.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cf.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://qk.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rj.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://fh.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://xv.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ku.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sr.huixinmuqiang.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yt.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qp.colortex.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://js.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://xi.shxzskj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ea.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://an.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ru.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ff.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cm.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rv.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nv.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lk.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://md.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tw.asd995.cn

[B07] while 循环
来源：http://ft.szsharing.cn

Py:   while i < 10: i += 1
来源：http://mj.bjjhwx.cn


<!-- 参考信息 -->