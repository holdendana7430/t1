代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qu.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gm.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fd.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zt.jctech888.com.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vw.bjjhwx.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cc.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://if.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qx.jianghongdianzi.cn

================================================================================
来源：http://pv.bjjhwx.cn

A. 基础语法与类型
来源：http://el.shtwfgs.cn

================================================================================
来源：http://kq.muxihuayi.cn

[A01] Hello World
来源：http://qb.huanxung.cn

Py:   print("Hello, World!")
来源：http://tr.asd995.cn

PHP:  echo "Hello, World!";
来源：http://qm.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://wg.yuntaijiaju.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rh.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://ju.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://fg.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://bz.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gb.shxzukj.cn

[A02] 变量声明与赋值
来源：http://as.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mx.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pj.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://co.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ru.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://tl.nszjky.cn

Go:   name := "Alex"; age := 20
来源：http://md.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://lv.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kh.9csxet.cn

[A03] 常量定义
来源：http://ev.shtwfgs.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://un.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://fj.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://wo.yuntaijiaju.cn

TS:   const PI: number = 3.14159;
来源：http://gt.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://po.shxzukj.cn

Go:   const PI = 3.14159
来源：http://re.asd995.cn

Ruby: PI = 3.14159
来源：http://fk.huixinmuqiang.cn

C#:   const double PI = 3.14159;
来源：http://qf.wgjwhj.cn

[A04] 判断变量类型
来源：http://uz.nszjky.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bt.wgjwhj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gl.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gt.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://em.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dj.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rl.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://to.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://bg.muxihuayi.cn

[A05] 整数除法与取模
来源：http://ad.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ek.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nd.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qe.nicolike.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cu.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://ue.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://el.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://ew.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://vv.muxihuayi.cn

[A06] 字符串转数字
来源：http://co.muxihuayi.cn

Py:   int("42"); float("3.14")
来源：http://eh.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ec.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ce.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ty.9csxet.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wb.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yy.asd995.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gk.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mo.bjjhwx.cn

[A07] 数字转字符串
来源：http://vo.szsharing.cn

Py:   str(42)
来源：http://uc.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://lp.huanxung.cn

JS:   String(42); (42).toString()
来源：http://rt.panjiajie.cn

TS:   String(42)
来源：http://wc.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lx.hahajie.cn

Go:   strconv.Itoa(42)
来源：http://im.jianghongdianzi.cn

Ruby: 42.to_s
来源：http://gl.haigaiapp.cn

C#:   42.ToString()
来源：http://pu.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://ia.jianghongdianzi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lw.chemitech.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yp.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ht.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zc.shxzukj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hh.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://co.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pp.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://oo.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://do.jianghongdianzi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zc.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qq.bookmarksfly.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xi.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bq.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://le.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kv.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wo.yuntaijiaju.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lm.bookmarksfly.cn

[A10] 生成随机数
来源：http://yv.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://uf.gzmigu.cn

PHP:  random_int(1, 100);
来源：http://oq.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bo.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ef.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://re.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xs.colortex.cn

Ruby: rand(1..100)
来源：http://yx.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://re.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://ef.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://od.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rn.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tj.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://wk.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://hx.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sp.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jf.panjiajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fb.521024.cn

[A12] 字符串插值 / 格式化
来源：http://le.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mn.jctech888.com.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ph.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://fm.hnjuh.cn

TS:   `Hello, ${name}!`
来源：http://us.chemitech.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://pz.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wq.lnxyls.cn

Ruby: "Hello, #{name}!"
来源：http://sv.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://fo.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lh.shxzukj.cn

Py:   "第一行\n第二行"
来源：http://is.yuexingan06.cn

PHP:  "第一行\n第二行"
来源：http://oa.colortex.cn

JS:   "第一行\n第二行"
来源：http://xn.nicolike.cn

TS:   "第一行\n第二行"
来源：http://kb.lnxyls.cn

Java: "第一行\n第二行"
来源：http://et.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://cn.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://sz.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://mh.colortex.cn

[A14] 注释写法
来源：http://rb.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lg.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dj.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://oy.chemitech.net.cn

TS:   // 单行；/* 多行 */
来源：http://tm.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ph.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://fa.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dn.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://et.wgjwhj.cn

[A15] 空值判断与默认值
来源：http://le.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://jt.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://cj.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://yt.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://gg.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oa.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://sx.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://km.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://ba.asd995.cn

[A16] 真假值判断规则
来源：http://ho.yuntaijiaju.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pm.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ii.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uz.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://or.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rq.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zu.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kz.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mp.bookmarksfly.cn

[A17] 位运算
来源：http://zh.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fi.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nm.panjiajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tw.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vi.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ut.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ob.nszjky.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dc.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rc.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://vv.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://ea.521024.cn

PHP:  ord("A"); chr(65)
来源：http://vw.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qc.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pz.gzmigu.cn

Java: (int) 'A'; (char) 65
来源：http://on.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gg.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://zd.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://bt.nszjky.cn

[A19] 交换两个变量
来源：http://mj.huanxung.cn

Py:   a, b = b, a
来源：http://qh.panjiajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://uz.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://to.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://mf.nszjky.cn

Java: int t = a; a = b; b = t;
来源：http://wn.huixinmuqiang.cn

Go:   a, b = b, a
来源：http://ev.nicolike.cn

Ruby: a, b = b, a
来源：http://uy.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://ly.huixiangedu.cn

[A20] 读取标准输入
来源：http://sy.shxzukj.cn

Py:   name = input("请输入：")
来源：http://th.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bw.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://do.chemitech.net.cn

TS:   // Node.js：readline 模块
来源：http://nf.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://dz.chemitech.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hf.huanxung.cn

Ruby: gets.chomp
来源：http://za.huanxung.cn

C#:   Console.ReadLine();
来源：http://pa.yuexingan06.cn

[A21] 保留指定小数位输出
来源：http://lg.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://nw.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tm.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://vj.nszjky.cn

TS:   (3.14159).toFixed(2)
来源：http://xt.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://ri.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cw.yuexingan06.cn

Ruby: format("%.2f", 3.14159)
来源：http://ov.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://vk.szxytkj.cn

[A22] 获取字符串长度
来源：http://hl.hnjuh.cn

Py:   len(s)
来源：http://jw.521024.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vr.lnxyls.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qj.9csxet.cn

TS:   s.length
来源：http://qr.muxihuayi.cn

Java: s.length()
来源：http://jb.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xy.shxzskj.cn

Ruby: s.length
来源：http://oh.gzmigu.cn

C#:   s.Length
来源：http://rd.shtwfgs.cn

[A23] 大小写转换
来源：http://pw.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qi.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rk.yuntaijiaju.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gh.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yg.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zy.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tm.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ht.nszjky.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sp.yuexingan06.cn

[A24] 去除首尾空白
来源：http://ij.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nn.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bj.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sz.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ky.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oy.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://tv.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ck.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rn.jianghongdianzi.cn

[A25] 字符串比较
来源：http://fs.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://am.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kf.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hi.muxihuayi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://em.newstarts.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dr.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tv.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vc.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dq.szsharing.cn

[A26] 类型转换总览
来源：http://go.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vr.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fa.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ng.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://nj.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mf.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qq.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fn.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dv.jianghongdianzi.cn

================================================================================
来源：http://dp.wgjwhj.cn

B. 流程控制
来源：http://qd.lnxyls.cn

================================================================================
来源：http://sm.colortex.cn

[B01] 条件判断 if / else
来源：http://qt.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nv.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://un.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hw.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hx.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cg.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hf.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cm.szsharing.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gt.newstarts.cn

[B02] 多分支 else if / elif
来源：http://ra.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mb.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fy.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ae.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ii.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ef.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ol.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gp.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pu.521024.cn

[B03] switch / match / case
来源：http://vf.521024.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vm.nszjky.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cq.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fp.nicolike.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nz.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wo.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vr.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xj.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sk.chemitech.net.cn

[B04] for 计数循环
来源：http://oe.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://yb.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lg.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rm.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ut.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lx.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iy.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://jd.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nw.asd995.cn

[B05] 遍历数组 / 列表
来源：http://sl.huanxung.cn

Py:   for item in arr: print(item)
来源：http://mb.newstarts.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nj.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://km.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ca.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xr.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kj.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://fc.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://io.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://kh.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ol.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://al.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zb.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mo.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ij.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zq.yuexingan06.cn


<!-- 参考信息 -->