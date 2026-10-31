代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://ti.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rk.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ft.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ma.521024.cn

================================================================================
来源：http://hv.gzmigu.cn

A. 基础语法与类型
来源：http://fy.wgjwhj.cn

================================================================================
来源：http://xo.newstarts.cn

[A01] Hello World
来源：http://qv.szsharing.cn

Py:   print("Hello, World!")
来源：http://xx.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://xj.muxihuayi.cn

JS:   console.log("Hello, World!");
来源：http://cf.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vf.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://nt.lnxyls.cn

Go:   fmt.Println("Hello, World!")
来源：http://sq.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://ys.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ap.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://me.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eg.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nu.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qz.yuntaijiaju.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hr.hahajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://hp.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://bm.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://bd.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lw.panjiajie.cn

[A03] 常量定义
来源：http://gn.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kg.chemitech.net.cn

PHP:  const PI = 3.14159;
来源：http://ax.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://ge.hnjuh.cn

TS:   const PI: number = 3.14159;
来源：http://mp.szsharing.cn

Java: static final double PI = 3.14159;
来源：http://is.newstarts.cn

Go:   const PI = 3.14159
来源：http://um.hnjuh.cn

Ruby: PI = 3.14159
来源：http://ca.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://nx.panjiajie.cn

[A04] 判断变量类型
来源：http://pg.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zf.521024.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://av.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fd.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://av.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tg.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wf.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pr.hahajie.cn

C#:   x.GetType().Name; x is int
来源：http://cs.chemitech.net.cn

[A05] 整数除法与取模
来源：http://mj.521024.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kr.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://an.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ks.hahajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wt.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://wx.bookmarksfly.cn

Go:   7 / 2; 7 % 2
来源：http://rk.521024.cn

Ruby: 7 / 2; 7 % 2
来源：http://kd.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://ko.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://sn.jianghongdianzi.cn

Py:   int("42"); float("3.14")
来源：http://rk.9csxet.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rd.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xx.newstarts.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yf.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vx.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://df.521024.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://er.jctech888.com.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fs.hnjuh.cn

[A07] 数字转字符串
来源：http://zi.hnjuh.cn

Py:   str(42)
来源：http://hv.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://qq.9csxet.cn

JS:   String(42); (42).toString()
来源：http://ck.521024.cn

TS:   String(42)
来源：http://qi.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://er.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://eo.nszjky.cn

Ruby: 42.to_s
来源：http://mf.huanxung.cn

C#:   42.ToString()
来源：http://sc.colortex.cn

[A08] 取整与四舍五入
来源：http://ls.szxytkj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ei.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jd.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kr.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://an.muxihuayi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://br.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tv.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yk.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fl.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://pr.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nd.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ux.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ue.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uq.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ok.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xd.hnjuh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ym.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://aj.bookmarksfly.cn

[A10] 生成随机数
来源：http://zp.shxzukj.cn

Py:   import random; random.randint(1, 100)
来源：http://ip.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://zk.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hr.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qh.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://ph.newstarts.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tn.gzmigu.cn

Ruby: rand(1..100)
来源：http://ro.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://dx.newstarts.cn

[A11] 条件表达式（三元）
来源：http://er.newstarts.cn

Py:   "yes" if x > 0 else "no"
来源：http://fq.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ag.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dl.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ar.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://mb.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nx.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rt.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ht.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://cj.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ed.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fq.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://bb.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://pl.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://ri.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vk.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://wu.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://gk.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ww.shxzskj.cn

Py:   "第一行\n第二行"
来源：http://id.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://ys.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://te.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://xz.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://xw.lnxyls.cn

Go:   "第一行\n第二行"
来源：http://mc.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://ff.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://uw.colortex.cn

[A14] 注释写法
来源：http://er.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dp.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ut.huanxung.cn

JS:   // 单行；/* 多行 */
来源：http://ok.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://lf.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ex.521024.cn

Go:   // 单行；/* 多行 */
来源：http://wg.chemitech.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gs.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://ha.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://ta.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://ow.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://rn.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://rp.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://kh.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sc.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://so.521024.cn

Ruby: value = data || "默认值"
来源：http://cv.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://ty.huanxung.cn

[A16] 真假值判断规则
来源：http://ei.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bl.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mw.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wl.yuexingan06.cn

TS:   if (!x) {}
来源：http://et.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ay.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nj.panjiajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rg.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hr.jianghongdianzi.cn

[A17] 位运算
来源：http://au.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tu.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xv.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mu.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zv.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kk.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xj.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ba.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nj.521024.cn

[A18] 字符与 ASCII 码互转
来源：http://bm.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://qx.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://bp.bjjhwx.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sj.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kw.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://jp.panjiajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rf.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://wg.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://li.gzmigu.cn

[A19] 交换两个变量
来源：http://th.muxihuayi.cn

Py:   a, b = b, a
来源：http://mc.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kf.huixiangedu.cn

JS:   [a, b] = [b, a];
来源：http://yo.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://im.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://go.szxytkj.cn

Go:   a, b = b, a
来源：http://fy.colortex.cn

Ruby: a, b = b, a
来源：http://nx.shxzukj.cn

C#:   (a, b) = (b, a);
来源：http://fm.521024.cn

[A20] 读取标准输入
来源：http://uu.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://bt.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://iu.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ql.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://jy.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://jb.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rc.chemitech.net.cn

Ruby: gets.chomp
来源：http://at.newstarts.cn

C#:   Console.ReadLine();
来源：http://cq.hahajie.cn

[A21] 保留指定小数位输出
来源：http://vw.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://za.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://de.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://qu.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://al.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://gl.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qf.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://ja.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://fo.521024.cn

[A22] 获取字符串长度
来源：http://ns.huanxung.cn

Py:   len(s)
来源：http://ye.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fs.jianghongdianzi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mm.bjjhwx.cn

TS:   s.length
来源：http://de.newstarts.cn

Java: s.length()
来源：http://ao.jctech888.com.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qs.huixiangedu.cn

Ruby: s.length
来源：http://ys.muxihuayi.cn

C#:   s.Length
来源：http://sk.bjjhwx.cn

[A23] 大小写转换
来源：http://jh.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ts.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ck.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mu.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sz.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ou.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ib.yuntaijiaju.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gy.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jv.lnxyls.cn

[A24] 去除首尾空白
来源：http://pg.asd995.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hx.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lr.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://va.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vo.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qx.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://so.shxzukj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ds.asd995.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pc.bjjhwx.cn

[A25] 字符串比较
来源：http://df.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://sn.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gq.bookmarksfly.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zx.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wm.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://th.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xa.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oc.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cm.jctech888.com.cn

[A26] 类型转换总览
来源：http://of.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zo.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mn.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fz.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://uz.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ap.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ap.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://me.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jm.gzmigu.cn

================================================================================
来源：http://rv.jianghongdianzi.cn

B. 流程控制
来源：http://bs.huanxung.cn

================================================================================
来源：http://de.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://ug.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ey.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wg.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pb.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xm.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vw.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tm.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ok.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rp.asd995.cn

[B02] 多分支 else if / elif
来源：http://sw.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ag.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lw.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zz.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pe.9csxet.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fa.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vd.521024.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xu.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ym.shxzskj.cn

[B03] switch / match / case
来源：http://gq.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jr.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gr.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cl.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ar.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ml.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://np.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tu.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gr.shxzukj.cn

[B04] for 计数循环
来源：http://gs.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://ab.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pp.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fc.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cw.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uj.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kr.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://iq.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xb.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://ng.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://mx.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zp.huixiangedu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ay.muxihuayi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ha.asd995.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lj.gzmigu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tk.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://fl.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oi.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://sh.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tl.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hf.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fz.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pr.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mc.hnjuh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://er.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oi.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hw.shxzukj.cn

[B07] while 循环
来源：http://uy.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://dd.nicolike.cn


<!-- 参考信息 -->