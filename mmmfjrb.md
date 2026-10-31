代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sd.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://df.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sc.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tq.newstarts.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vp.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://la.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cb.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gb.asd995.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oy.9csxet.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cg.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nu.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qo.bookmarksfly.cn

================================================================================
来源：http://fd.huixinmuqiang.cn

A. 基础语法与类型
来源：http://ae.colortex.cn

================================================================================
来源：http://kf.jctech888.com.cn

[A01] Hello World
来源：http://fn.colortex.cn

Py:   print("Hello, World!")
来源：http://dc.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://ii.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://ia.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gh.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://kt.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://rg.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://xd.huanxung.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dn.jctech888.com.cn

[A02] 变量声明与赋值
来源：http://yl.jctech888.com.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ug.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mu.shtwfgs.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xz.lnxyls.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yk.lnxyls.cn

Java: String name = "Alex"; int age = 20;
来源：http://py.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://xs.jianghongdianzi.cn

Ruby: name = "Alex"; age = 20
来源：http://ct.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xi.shxzskj.cn

[A03] 常量定义
来源：http://mi.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vh.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://yg.hnjuh.cn

JS:   const PI = 3.14159;
来源：http://tg.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://ru.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://bs.lnxyls.cn

Go:   const PI = 3.14159
来源：http://kv.huixiangedu.cn

Ruby: PI = 3.14159
来源：http://pd.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://dg.szsharing.cn

[A04] 判断变量类型
来源：http://ni.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ta.colortex.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ph.lnxyls.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://on.yuexingan06.cn

TS:   typeof x; x instanceof Date
来源：http://za.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fr.huixinmuqiang.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dn.muxihuayi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qu.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://fo.colortex.cn

[A05] 整数除法与取模
来源：http://dg.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ro.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://aw.asd995.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hj.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://li.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://yi.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://jw.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://mb.shxzukj.cn

C#:   7 / 2; 7 % 2
来源：http://yl.colortex.cn

[A06] 字符串转数字
来源：http://lu.yuexingan06.cn

Py:   int("42"); float("3.14")
来源：http://zn.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lr.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wv.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yn.newstarts.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bj.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pc.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ku.chemitech.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lg.panjiajie.cn

[A07] 数字转字符串
来源：http://ja.chemitech.net.cn

Py:   str(42)
来源：http://mb.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://mp.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://nv.huixinmuqiang.cn

TS:   String(42)
来源：http://we.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://aa.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://ln.szsharing.cn

Ruby: 42.to_s
来源：http://xc.jctech888.com.cn

C#:   42.ToString()
来源：http://wl.newstarts.cn

[A08] 取整与四舍五入
来源：http://bi.hahajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ar.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://um.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vo.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ex.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ji.shtwfgs.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nr.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xf.panjiajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xz.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://lb.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rq.bjjhwx.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://og.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sa.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cq.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://la.huixinmuqiang.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ux.newstarts.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uw.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cy.colortex.cn

[A10] 生成随机数
来源：http://nc.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://sx.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://he.521024.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rz.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ed.lnxyls.cn

Java: new Random().nextInt(100) + 1
来源：http://dk.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ag.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://pc.shtwfgs.cn

C#:   new Random().Next(1, 101)
来源：http://df.lnxyls.cn

[A11] 条件表达式（三元）
来源：http://vz.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://lf.szxytkj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xk.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ij.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yh.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://yq.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://io.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cj.szxytkj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vt.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://vh.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vv.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bu.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://kc.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://oa.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://pd.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qt.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://dr.muxihuayi.cn

C#:   $"Hello, {name}!"
来源：http://pv.colortex.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hj.newstarts.cn

Py:   "第一行\n第二行"
来源：http://dj.bjjhwx.cn

PHP:  "第一行\n第二行"
来源：http://kr.nicolike.cn

JS:   "第一行\n第二行"
来源：http://wo.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://dt.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://zr.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://pu.colortex.cn

Ruby: "第一行\n第二行"
来源：http://im.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://lp.jctech888.com.cn

[A14] 注释写法
来源：http://ah.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zq.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fv.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://tv.bjjhwx.cn

TS:   // 单行；/* 多行 */
来源：http://kg.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rn.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://uo.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fi.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://qt.9csxet.cn

[A15] 空值判断与默认值
来源：http://jy.colortex.cn

Py:   value = data or "默认值"
来源：http://ol.hnjuh.cn

PHP:  $value = $data ?? "默认值";
来源：http://oi.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://ss.gzmigu.cn

TS:   const value = data ?? "默认值";
来源：http://qy.9csxet.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rp.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://qv.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://fw.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://gu.nicolike.cn

[A16] 真假值判断规则
来源：http://iv.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jq.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gu.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ei.nicolike.cn

TS:   if (!x) {}
来源：http://si.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uu.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ay.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oh.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zy.nicolike.cn

[A17] 位运算
来源：http://zp.huanxung.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uo.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nb.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cl.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dj.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zq.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ag.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ax.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cq.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://ms.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://xv.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://sh.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ir.newstarts.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lw.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://sk.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dk.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://cm.521024.cn

C#:   (int)'A'; (char)65
来源：http://al.hahajie.cn

[A19] 交换两个变量
来源：http://iy.huanxung.cn

Py:   a, b = b, a
来源：http://oj.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://oe.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://rc.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://km.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://xv.wgjwhj.cn

Go:   a, b = b, a
来源：http://qu.shxzukj.cn

Ruby: a, b = b, a
来源：http://sk.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://jz.szxytkj.cn

[A20] 读取标准输入
来源：http://tz.asd995.cn

Py:   name = input("请输入：")
来源：http://se.szxytkj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ok.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hx.colortex.cn

TS:   // Node.js：readline 模块
来源：http://kv.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://kv.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hl.shtwfgs.cn

Ruby: gets.chomp
来源：http://ax.huanxung.cn

C#:   Console.ReadLine();
来源：http://gy.asd995.cn

[A21] 保留指定小数位输出
来源：http://ua.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://mk.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ag.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://dn.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://sj.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://kt.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wd.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://ds.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://gd.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://us.yuexingan06.cn

Py:   len(s)
来源：http://kt.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ok.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cl.yuntaijiaju.cn

TS:   s.length
来源：http://nc.yuexingan06.cn

Java: s.length()
来源：http://cj.gzmigu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hi.yuexingan06.cn

Ruby: s.length
来源：http://wh.asd995.cn

C#:   s.Length
来源：http://su.yuntaijiaju.cn

[A23] 大小写转换
来源：http://xl.bookmarksfly.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ac.chemitech.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ex.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mm.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qj.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ka.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ga.shtwfgs.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lg.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eg.lnxyls.cn

[A24] 去除首尾空白
来源：http://cn.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sz.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rr.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ib.shxzskj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tr.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ry.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://zu.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kg.huixiangedu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dh.asd995.cn

[A25] 字符串比较
来源：http://oe.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://ax.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bp.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wm.szsharing.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nh.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xl.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://el.gzmigu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lv.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pt.chemitech.net.cn

[A26] 类型转换总览
来源：http://nq.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://df.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://db.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ur.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://bd.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cm.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bu.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://at.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mt.colortex.cn

================================================================================
来源：http://xq.szsharing.cn

B. 流程控制
来源：http://yd.shxzskj.cn

================================================================================
来源：http://kd.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://ep.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kn.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gt.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nj.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uo.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://eu.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qt.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mv.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pt.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://nv.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rj.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oj.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ur.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mg.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ta.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qb.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ku.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sf.nicolike.cn

[B03] switch / match / case
来源：http://lh.9csxet.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tj.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jo.nicolike.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mq.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fg.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oo.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kc.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ub.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ei.jctech888.com.cn

[B04] for 计数循环
来源：http://qd.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://zh.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zr.asd995.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ko.panjiajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ht.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ms.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vq.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://cd.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ae.bjjhwx.cn

[B05] 遍历数组 / 列表
来源：http://dv.nicolike.cn

Py:   for item in arr: print(item)
来源：http://jo.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fr.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oo.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xp.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tu.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pz.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://pz.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hq.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://yh.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qu.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://te.asd995.cn


<!-- 参考信息 -->