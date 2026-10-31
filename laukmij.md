代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lc.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ym.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xf.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tx.jctech888.com.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fe.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rg.chemitech.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hn.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fw.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://if.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yz.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kx.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vi.hnjuh.cn

================================================================================
来源：http://fo.chemitech.net.cn

A. 基础语法与类型
来源：http://wn.9csxet.cn

================================================================================
来源：http://gn.9csxet.cn

[A01] Hello World
来源：http://ws.huanxung.cn

Py:   print("Hello, World!")
来源：http://fv.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://gn.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://be.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zz.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://be.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://hv.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://di.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nv.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://fs.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oo.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wy.bjjhwx.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pt.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://da.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://va.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://en.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://py.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ej.hahajie.cn

[A03] 常量定义
来源：http://ub.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://up.521024.cn

PHP:  const PI = 3.14159;
来源：http://tj.chemitech.net.cn

JS:   const PI = 3.14159;
来源：http://dp.wgjwhj.cn

TS:   const PI: number = 3.14159;
来源：http://xd.bjjhwx.cn

Java: static final double PI = 3.14159;
来源：http://zk.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://pg.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://nf.chemitech.net.cn

C#:   const double PI = 3.14159;
来源：http://yk.hahajie.cn

[A04] 判断变量类型
来源：http://el.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tx.bjjhwx.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://th.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://my.lnxyls.cn

TS:   typeof x; x instanceof Date
来源：http://kx.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ii.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://da.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vx.shtwfgs.cn

C#:   x.GetType().Name; x is int
来源：http://ks.huanxung.cn

[A05] 整数除法与取模
来源：http://ol.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pb.shtwfgs.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dv.asd995.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nu.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lu.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://fv.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://wz.shxzskj.cn

Ruby: 7 / 2; 7 % 2
来源：http://yc.haigaiapp.cn

C#:   7 / 2; 7 % 2
来源：http://tp.9csxet.cn

[A06] 字符串转数字
来源：http://vi.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://eo.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ww.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dm.shxzskj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yp.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ww.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sw.colortex.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kx.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://im.huixiangedu.cn

[A07] 数字转字符串
来源：http://sw.nszjky.cn

Py:   str(42)
来源：http://ms.muxihuayi.cn

PHP:  (string) 42; strval(42)
来源：http://qk.huixinmuqiang.cn

JS:   String(42); (42).toString()
来源：http://gt.yuexingan06.cn

TS:   String(42)
来源：http://pu.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://co.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://ng.521024.cn

Ruby: 42.to_s
来源：http://rh.wgjwhj.cn

C#:   42.ToString()
来源：http://is.panjiajie.cn

[A08] 取整与四舍五入
来源：http://mj.yuexingan06.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ol.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ib.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ga.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://js.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hf.yuexingan06.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eu.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://re.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ah.yuexingan06.cn

[A09] 绝对值与最大最小值
来源：http://gu.chemitech.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ve.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rr.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zg.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qw.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hj.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lj.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ty.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mq.lnxyls.cn

[A10] 生成随机数
来源：http://li.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://uv.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://fa.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wm.gzmigu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://si.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://gz.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lg.jctech888.com.cn

Ruby: rand(1..100)
来源：http://pv.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://hj.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://ll.huixinmuqiang.cn

Py:   "yes" if x > 0 else "no"
来源：http://ru.panjiajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://iv.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hl.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pk.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://mu.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qq.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hd.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gj.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://op.panjiajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cc.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iu.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://jb.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://qp.shxzukj.cn

Java: "Hello, %s!".formatted(name)
来源：http://uq.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fi.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://fm.9csxet.cn

C#:   $"Hello, {name}!"
来源：http://yh.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qs.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://le.asd995.cn

PHP:  "第一行\n第二行"
来源：http://tk.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://du.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://mx.panjiajie.cn

Java: "第一行\n第二行"
来源：http://tf.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://sx.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://yc.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://wa.jianghongdianzi.cn

[A14] 注释写法
来源：http://th.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ao.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://is.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://sl.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://xc.colortex.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mq.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://pb.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://je.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://tx.chemitech.net.cn

[A15] 空值判断与默认值
来源：http://mp.shxzskj.cn

Py:   value = data or "默认值"
来源：http://wk.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://bf.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://ku.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://la.9csxet.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wr.newstarts.cn

Go:   if data == "" { data = "默认值" }
来源：http://xc.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://rf.shxzukj.cn

C#:   var value = data ?? "默认值";
来源：http://as.gzmigu.cn

[A16] 真假值判断规则
来源：http://ju.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rm.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://da.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mc.bookmarksfly.cn

TS:   if (!x) {}
来源：http://cl.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zd.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ff.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rf.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qu.asd995.cn

[A17] 位运算
来源：http://hn.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wr.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jk.hahajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ym.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ds.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pz.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wx.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wf.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xe.shtwfgs.cn

[A18] 字符与 ASCII 码互转
来源：http://zj.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://ju.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://wh.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sn.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://az.chemitech.net.cn

Java: (int) 'A'; (char) 65
来源：http://so.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ot.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://gf.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://br.jctech888.com.cn

[A19] 交换两个变量
来源：http://fr.newstarts.cn

Py:   a, b = b, a
来源：http://yc.asd995.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kb.asd995.cn

JS:   [a, b] = [b, a];
来源：http://yg.jianghongdianzi.cn

TS:   [a, b] = [b, a];
来源：http://ff.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://xq.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://wj.asd995.cn

Ruby: a, b = b, a
来源：http://ym.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://ma.colortex.cn

[A20] 读取标准输入
来源：http://cz.huanxung.cn

Py:   name = input("请输入：")
来源：http://ya.huixiangedu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bz.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cm.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://ne.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://zi.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sq.huixiangedu.cn

Ruby: gets.chomp
来源：http://ai.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://hl.nicolike.cn

[A21] 保留指定小数位输出
来源：http://na.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://ik.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jd.asd995.cn

JS:   (3.14159).toFixed(2)
来源：http://tn.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://hm.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://mv.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pt.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://xq.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://ki.jctech888.com.cn

[A22] 获取字符串长度
来源：http://th.lnxyls.cn

Py:   len(s)
来源：http://cc.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://md.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://al.szxytkj.cn

TS:   s.length
来源：http://rw.bookmarksfly.cn

Java: s.length()
来源：http://hx.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jw.panjiajie.cn

Ruby: s.length
来源：http://gz.hahajie.cn

C#:   s.Length
来源：http://qb.asd995.cn

[A23] 大小写转换
来源：http://pe.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://eq.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cs.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sz.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jn.shxzukj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sh.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gk.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ix.huixinmuqiang.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cd.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://xu.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vk.yuexingan06.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yh.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eg.yuntaijiaju.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rd.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ux.haigaiapp.cn

Go:   strings.TrimSpace(s)
来源：http://lq.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qz.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mm.shtwfgs.cn

[A25] 字符串比较
来源：http://so.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://vs.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jn.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cg.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bp.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ch.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gm.bjjhwx.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bh.lnxyls.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kg.chemitech.net.cn

[A26] 类型转换总览
来源：http://uu.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yd.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ew.szxytkj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wp.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://pc.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cc.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aa.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nt.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kr.bookmarksfly.cn

================================================================================
来源：http://vk.yuntaijiaju.cn

B. 流程控制
来源：http://ba.bookmarksfly.cn

================================================================================
来源：http://lf.hahajie.cn

[B01] 条件判断 if / else
来源：http://bv.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qx.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lk.shxzukj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bi.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vi.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ha.chemitech.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hw.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ch.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gn.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://xs.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rr.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pk.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ay.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://al.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qx.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dm.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ox.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://th.jianghongdianzi.cn

[B03] switch / match / case
来源：http://bi.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kh.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tf.huixiangedu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://du.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kh.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://od.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mz.colortex.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://at.muxihuayi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ev.newstarts.cn

[B04] for 计数循环
来源：http://nl.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://vd.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pq.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hf.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wn.huixinmuqiang.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://es.szsharing.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ys.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://oc.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wp.521024.cn

[B05] 遍历数组 / 列表
来源：http://id.hahajie.cn

Py:   for item in arr: print(item)
来源：http://yl.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cj.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ej.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mn.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hq.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sf.jctech888.com.cn

Ruby: arr.each { |item| puts item }
来源：http://hd.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://un.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://sa.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tk.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ky.huixinmuqiang.cn


<!-- 参考信息 -->