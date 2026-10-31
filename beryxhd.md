代发 wailian999

--------------------------------------------------------------------------------
来源：http://di.nicolike.cn

目  录
来源：http://sm.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://wp.lnxyls.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qo.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ts.9csxet.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ur.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nq.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dv.nszjky.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qx.lnxyls.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ta.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gn.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fk.szxytkj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dq.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rk.panjiajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://aj.lnxyls.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bm.szsharing.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xm.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vy.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wj.huixiangedu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yk.newstarts.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pv.asd995.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yz.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ip.wgjwhj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nx.colortex.cn

================================================================================
来源：http://gn.huixinmuqiang.cn

A. 基础语法与类型
来源：http://ij.huixiangedu.cn

================================================================================
来源：http://nb.lnxyls.cn

[A01] Hello World
来源：http://tv.hahajie.cn

Py:   print("Hello, World!")
来源：http://zj.bjjhwx.cn

PHP:  echo "Hello, World!";
来源：http://ef.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://kn.wgjwhj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bh.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://kq.szxytkj.cn

Go:   fmt.Println("Hello, World!")
来源：http://eh.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://np.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wg.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://sz.yuntaijiaju.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zz.chemitech.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bq.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://an.lnxyls.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ey.lnxyls.cn

Java: String name = "Alex"; int age = 20;
来源：http://ks.bjjhwx.cn

Go:   name := "Alex"; age := 20
来源：http://dr.huanxung.cn

Ruby: name = "Alex"; age = 20
来源：http://cu.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://us.chemitech.net.cn

[A03] 常量定义
来源：http://um.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zl.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://zi.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://ax.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://xa.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://pa.newstarts.cn

Go:   const PI = 3.14159
来源：http://ah.colortex.cn

Ruby: PI = 3.14159
来源：http://kv.huanxung.cn

C#:   const double PI = 3.14159;
来源：http://sp.huixiangedu.cn

[A04] 判断变量类型
来源：http://dj.shtwfgs.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://sp.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bv.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lb.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://mb.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://va.hahajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sb.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://du.shxzukj.cn

C#:   x.GetType().Name; x is int
来源：http://sq.521024.cn

[A05] 整数除法与取模
来源：http://uu.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ce.panjiajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hu.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nk.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sg.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://xz.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://il.yuntaijiaju.cn

Ruby: 7 / 2; 7 % 2
来源：http://ge.521024.cn

C#:   7 / 2; 7 % 2
来源：http://xn.asd995.cn

[A06] 字符串转数字
来源：http://po.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://sv.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ue.newstarts.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jp.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vq.gzmigu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uv.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ob.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ju.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jh.gzmigu.cn

[A07] 数字转字符串
来源：http://dd.haigaiapp.cn

Py:   str(42)
来源：http://hp.huixinmuqiang.cn

PHP:  (string) 42; strval(42)
来源：http://pz.521024.cn

JS:   String(42); (42).toString()
来源：http://lt.colortex.cn

TS:   String(42)
来源：http://ko.jianghongdianzi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sa.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://dh.bjjhwx.cn

Ruby: 42.to_s
来源：http://oy.9csxet.cn

C#:   42.ToString()
来源：http://sd.9csxet.cn

[A08] 取整与四舍五入
来源：http://gj.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oz.newstarts.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lz.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ay.gzmigu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hh.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oe.panjiajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mf.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ch.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://oe.bookmarksfly.cn

[A09] 绝对值与最大最小值
来源：http://zt.521024.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cj.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uz.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qa.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xl.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dr.haigaiapp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iw.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://aq.szsharing.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xh.wgjwhj.cn

[A10] 生成随机数
来源：http://ef.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://uc.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://et.bjjhwx.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kf.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uj.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://ay.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uw.asd995.cn

Ruby: rand(1..100)
来源：http://xc.hahajie.cn

C#:   new Random().Next(1, 101)
来源：http://hd.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://nx.yuexingan06.cn

Py:   "yes" if x > 0 else "no"
来源：http://qg.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://pj.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://od.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://iz.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://ds.shxzskj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ec.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nt.hnjuh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://si.shxzukj.cn

[A12] 字符串插值 / 格式化
来源：http://tf.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hu.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nq.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://vw.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://lx.newstarts.cn

Java: "Hello, %s!".formatted(name)
来源：http://hg.gzmigu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://na.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://vu.huixiangedu.cn

C#:   $"Hello, {name}!"
来源：http://ya.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qi.9csxet.cn

Py:   "第一行\n第二行"
来源：http://gv.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://pg.9csxet.cn

JS:   "第一行\n第二行"
来源：http://wj.newstarts.cn

TS:   "第一行\n第二行"
来源：http://ue.shxzukj.cn

Java: "第一行\n第二行"
来源：http://yw.nicolike.cn

Go:   "第一行\n第二行"
来源：http://af.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://ud.newstarts.cn

C#:   "第一行\n第二行"
来源：http://kj.9csxet.cn

[A14] 注释写法
来源：http://rx.asd995.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tk.hahajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tv.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://sn.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://ua.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vu.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://bk.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yb.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://rk.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://rt.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://je.hahajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://na.muxihuayi.cn

JS:   const value = data ?? "默认值";
来源：http://xi.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://xn.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://az.muxihuayi.cn

Go:   if data == "" { data = "默认值" }
来源：http://xt.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://fp.nszjky.cn

C#:   var value = data ?? "默认值";
来源：http://na.bjjhwx.cn

[A16] 真假值判断规则
来源：http://tb.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pv.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jw.wgjwhj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zt.asd995.cn

TS:   if (!x) {}
来源：http://jj.shxzukj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mn.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ov.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bq.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://du.bjjhwx.cn

[A17] 位运算
来源：http://fv.hahajie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yc.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vv.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tt.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sw.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gs.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jr.bjjhwx.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cb.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nb.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://rf.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://yv.nicolike.cn

PHP:  ord("A"); chr(65)
来源：http://ue.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zi.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wv.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://va.bookmarksfly.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mn.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://zh.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://th.panjiajie.cn

[A19] 交换两个变量
来源：http://hw.huixiangedu.cn

Py:   a, b = b, a
来源：http://ss.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://co.shxzukj.cn

JS:   [a, b] = [b, a];
来源：http://sv.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://zc.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://jh.nszjky.cn

Go:   a, b = b, a
来源：http://iu.bjjhwx.cn

Ruby: a, b = b, a
来源：http://nt.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://mj.colortex.cn

[A20] 读取标准输入
来源：http://hy.9csxet.cn

Py:   name = input("请输入：")
来源：http://gd.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ay.gzmigu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wg.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://fm.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://en.shxzukj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ju.szxytkj.cn

Ruby: gets.chomp
来源：http://rv.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://ht.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://dd.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://jv.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nx.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://tm.jianghongdianzi.cn

TS:   (3.14159).toFixed(2)
来源：http://vz.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://oa.asd995.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://au.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://bi.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://vh.521024.cn

[A22] 获取字符串长度
来源：http://yl.szsharing.cn

Py:   len(s)
来源：http://ck.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wn.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mz.szsharing.cn

TS:   s.length
来源：http://ys.yuexingan06.cn

Java: s.length()
来源：http://tz.nicolike.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ov.yuntaijiaju.cn

Ruby: s.length
来源：http://qf.muxihuayi.cn

C#:   s.Length
来源：http://ac.hnjuh.cn

[A23] 大小写转换
来源：http://ro.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gm.haigaiapp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hu.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vx.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hh.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://me.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rg.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dp.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eo.muxihuayi.cn

[A24] 去除首尾空白
来源：http://me.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dg.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://re.jctech888.com.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ns.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bm.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ef.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://vn.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vi.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fw.szxytkj.cn

[A25] 字符串比较
来源：http://am.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://rw.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xn.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zm.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rp.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ye.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uu.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ms.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://am.gzmigu.cn

[A26] 类型转换总览
来源：http://xj.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://af.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nf.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kz.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://na.shxzukj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qp.newstarts.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ly.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bv.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://go.huixiangedu.cn

================================================================================
来源：http://sy.hahajie.cn

B. 流程控制
来源：http://hh.panjiajie.cn

================================================================================
来源：http://fm.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://he.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fh.shxzskj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gg.bjjhwx.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://on.hahajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yq.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ua.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pr.shtwfgs.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qi.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://di.hnjuh.cn

[B02] 多分支 else if / elif
来源：http://ha.bookmarksfly.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dt.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ps.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ic.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vo.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ap.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vw.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rf.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sa.huanxung.cn

[B03] switch / match / case
来源：http://cb.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cb.shxzskj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yz.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hw.newstarts.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rv.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mb.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pq.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rh.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zi.yuntaijiaju.cn

[B04] for 计数循环
来源：http://bf.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://yc.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pt.gzmigu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vj.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ms.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fe.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zp.hnjuh.cn

Ruby: 10.times { |i| puts i }
来源：http://rc.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yt.jctech888.com.cn


<!-- 参考信息 -->