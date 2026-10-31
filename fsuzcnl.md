代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gs.gzmigu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jj.521024.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://np.jianghongdianzi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cz.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ci.huixiangedu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ct.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://op.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mq.asd995.cn

================================================================================
来源：http://wh.nicolike.cn

A. 基础语法与类型
来源：http://hk.yuexingan06.cn

================================================================================
来源：http://ib.hnjuh.cn

[A01] Hello World
来源：http://yr.colortex.cn

Py:   print("Hello, World!")
来源：http://fo.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://az.bjjhwx.cn

JS:   console.log("Hello, World!");
来源：http://kv.nszjky.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sk.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://av.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://rd.asd995.cn

Ruby: puts "Hello, World!"
来源：http://mg.huixiangedu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pj.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://qq.nicolike.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jc.huixinmuqiang.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://je.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qv.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lq.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://mp.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://nd.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://df.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://is.colortex.cn

[A03] 常量定义
来源：http://ds.huixiangedu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://up.shtwfgs.cn

PHP:  const PI = 3.14159;
来源：http://ig.521024.cn

JS:   const PI = 3.14159;
来源：http://ij.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://lh.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://yq.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://jx.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://ly.colortex.cn

C#:   const double PI = 3.14159;
来源：http://qu.9csxet.cn

[A04] 判断变量类型
来源：http://ls.shtwfgs.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://es.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gr.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zp.shxzskj.cn

TS:   typeof x; x instanceof Date
来源：http://aw.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pr.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nd.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qy.szsharing.cn

C#:   x.GetType().Name; x is int
来源：http://cm.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://cs.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yr.bookmarksfly.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://po.bookmarksfly.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wi.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wb.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://eu.haigaiapp.cn

Go:   7 / 2; 7 % 2
来源：http://jy.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://se.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://zc.hahajie.cn

[A06] 字符串转数字
来源：http://cm.yuntaijiaju.cn

Py:   int("42"); float("3.14")
来源：http://gy.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pd.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ly.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://oj.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sh.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ot.hahajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qr.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://en.shxzskj.cn

[A07] 数字转字符串
来源：http://nl.gzmigu.cn

Py:   str(42)
来源：http://kk.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://hh.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://ab.shxzskj.cn

TS:   String(42)
来源：http://bk.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hy.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://mf.yuexingan06.cn

Ruby: 42.to_s
来源：http://zm.muxihuayi.cn

C#:   42.ToString()
来源：http://ux.shtwfgs.cn

[A08] 取整与四舍五入
来源：http://ui.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pw.521024.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vh.shtwfgs.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bl.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fy.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zt.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gl.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://kh.nszjky.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ds.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://fr.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ms.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://is.bookmarksfly.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fn.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gz.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nu.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://om.jianghongdianzi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bv.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vw.jianghongdianzi.cn

[A10] 生成随机数
来源：http://ah.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://av.nszjky.cn

PHP:  random_int(1, 100);
来源：http://nl.521024.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vi.shtwfgs.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xl.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://ps.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xi.szsharing.cn

Ruby: rand(1..100)
来源：http://bz.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://nj.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://nk.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://je.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pq.panjiajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jp.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ai.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://xg.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xz.yuntaijiaju.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pb.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://eu.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://gy.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uh.shxzukj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zd.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://qv.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://ue.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://gm.yuexingan06.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nx.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://gc.9csxet.cn

C#:   $"Hello, {name}!"
来源：http://vl.bjjhwx.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://pa.lnxyls.cn

Py:   "第一行\n第二行"
来源：http://ze.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://dl.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://vt.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://oo.hnjuh.cn

Java: "第一行\n第二行"
来源：http://ub.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://dt.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://nv.jianghongdianzi.cn

C#:   "第一行\n第二行"
来源：http://ka.asd995.cn

[A14] 注释写法
来源：http://uf.huanxung.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vf.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wz.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://an.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://aa.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sy.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://aw.panjiajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qd.521024.cn

C#:   // 单行；/* 多行 */
来源：http://mf.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://fh.hnjuh.cn

Py:   value = data or "默认值"
来源：http://vy.chemitech.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://ta.shxzukj.cn

JS:   const value = data ?? "默认值";
来源：http://bw.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://tl.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ep.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://sj.jianghongdianzi.cn

Ruby: value = data || "默认值"
来源：http://fq.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://ga.huanxung.cn

[A16] 真假值判断规则
来源：http://hg.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ug.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uc.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sm.shtwfgs.cn

TS:   if (!x) {}
来源：http://re.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ac.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hn.asd995.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jc.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mj.szsharing.cn

[A17] 位运算
来源：http://va.newstarts.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ql.jianghongdianzi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mx.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ck.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://et.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qx.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xf.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ok.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vm.haigaiapp.cn

[A18] 字符与 ASCII 码互转
来源：http://av.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://ff.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://sc.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://et.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vp.colortex.cn

Java: (int) 'A'; (char) 65
来源：http://cv.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vm.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://kr.chemitech.net.cn

C#:   (int)'A'; (char)65
来源：http://mv.521024.cn

[A19] 交换两个变量
来源：http://tu.gzmigu.cn

Py:   a, b = b, a
来源：http://ik.jianghongdianzi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bf.9csxet.cn

JS:   [a, b] = [b, a];
来源：http://gq.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://yd.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://nh.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://hk.shxzskj.cn

Ruby: a, b = b, a
来源：http://an.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://su.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://nx.hnjuh.cn

Py:   name = input("请输入：")
来源：http://vq.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ow.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tl.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://dt.nszjky.cn

Java: new Scanner(System.in).nextLine()
来源：http://iq.hahajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mj.bookmarksfly.cn

Ruby: gets.chomp
来源：http://eu.newstarts.cn

C#:   Console.ReadLine();
来源：http://ql.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://xr.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://im.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vn.lnxyls.cn

JS:   (3.14159).toFixed(2)
来源：http://rf.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://cx.huanxung.cn

Java: String.format("%.2f", 3.14159)
来源：http://uv.wgjwhj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nu.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://oj.jianghongdianzi.cn

C#:   3.14159.ToString("F2")
来源：http://xu.wgjwhj.cn

[A22] 获取字符串长度
来源：http://sf.hahajie.cn

Py:   len(s)
来源：http://yj.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uz.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bc.huanxung.cn

TS:   s.length
来源：http://ht.wgjwhj.cn

Java: s.length()
来源：http://ey.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mw.bjjhwx.cn

Ruby: s.length
来源：http://gy.shtwfgs.cn

C#:   s.Length
来源：http://ae.haigaiapp.cn

[A23] 大小写转换
来源：http://rb.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ir.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eg.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zr.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rv.bjjhwx.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gg.shxzskj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nc.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pu.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eg.muxihuayi.cn

[A24] 去除首尾空白
来源：http://vh.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rt.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qt.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qm.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qt.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pn.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://dw.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ix.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ap.szxytkj.cn

[A25] 字符串比较
来源：http://um.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://yb.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nc.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kv.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ar.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mc.haigaiapp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cd.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wx.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hh.bookmarksfly.cn

[A26] 类型转换总览
来源：http://js.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ex.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bq.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ld.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://mh.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cj.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://so.newstarts.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cv.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zc.haigaiapp.cn

================================================================================
来源：http://cw.yuntaijiaju.cn

B. 流程控制
来源：http://tw.huanxung.cn

================================================================================
来源：http://uf.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://ai.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qg.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fq.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sj.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lh.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gv.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qe.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oe.shxzukj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fb.hahajie.cn

[B02] 多分支 else if / elif
来源：http://ft.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nb.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mb.hnjuh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xr.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ts.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lc.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jp.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mr.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wj.muxihuayi.cn

[B03] switch / match / case
来源：http://cq.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tv.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wq.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fq.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pg.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://us.hnjuh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fj.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ry.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kn.bookmarksfly.cn

[B04] for 计数循环
来源：http://lr.panjiajie.cn

Py:   for i in range(10): print(i)
来源：http://oy.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wo.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zt.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nf.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qs.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rx.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://bz.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://io.521024.cn

[B05] 遍历数组 / 列表
来源：http://yw.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://ky.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yk.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gb.hnjuh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gw.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sb.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jd.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://te.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hr.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://sa.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vc.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xl.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qh.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rr.wgjwhj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pz.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ud.muxihuayi.cn


<!-- 参考信息 -->