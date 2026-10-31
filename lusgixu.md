代发 wailian999

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ni.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tt.wgjwhj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tp.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vq.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nk.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aa.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://as.jctech888.com.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mp.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ra.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fe.lnxyls.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zj.521024.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lo.szsharing.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bm.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wc.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nr.asd995.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bj.bjjhwx.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nq.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jr.panjiajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qs.nszjky.cn

================================================================================
来源：http://gc.bjjhwx.cn

A. 基础语法与类型
来源：http://iv.9csxet.cn

================================================================================
来源：http://nx.hahajie.cn

[A01] Hello World
来源：http://fa.lnxyls.cn

Py:   print("Hello, World!")
来源：http://dm.asd995.cn

PHP:  echo "Hello, World!";
来源：http://hd.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://cz.521024.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pm.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://ts.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://kf.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://gt.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sr.nszjky.cn

[A02] 变量声明与赋值
来源：http://uv.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mf.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hi.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jl.yuntaijiaju.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rr.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://vm.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://mk.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://aq.521024.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mr.bookmarksfly.cn

[A03] 常量定义
来源：http://zv.muxihuayi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xc.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://hn.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://ee.hahajie.cn

TS:   const PI: number = 3.14159;
来源：http://sw.shtwfgs.cn

Java: static final double PI = 3.14159;
来源：http://xz.shxzskj.cn

Go:   const PI = 3.14159
来源：http://zy.bjjhwx.cn

Ruby: PI = 3.14159
来源：http://np.newstarts.cn

C#:   const double PI = 3.14159;
来源：http://jn.chemitech.net.cn

[A04] 判断变量类型
来源：http://xa.nszjky.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ad.haigaiapp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qb.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kp.huixinmuqiang.cn

TS:   typeof x; x instanceof Date
来源：http://de.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.shxzukj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zt.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vj.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://bd.nszjky.cn

[A05] 整数除法与取模
来源：http://ge.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://le.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zb.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ed.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kl.521024.cn

Java: 7 / 2; 7 % 2
来源：http://pu.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://mu.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://lf.shxzukj.cn

C#:   7 / 2; 7 % 2
来源：http://gt.newstarts.cn

[A06] 字符串转数字
来源：http://ds.hnjuh.cn

Py:   int("42"); float("3.14")
来源：http://jm.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bu.nicolike.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jf.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ab.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wa.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tp.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zd.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sz.muxihuayi.cn

[A07] 数字转字符串
来源：http://bm.szsharing.cn

Py:   str(42)
来源：http://lr.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://zr.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://hv.gzmigu.cn

TS:   String(42)
来源：http://jr.shtwfgs.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hl.hahajie.cn

Go:   strconv.Itoa(42)
来源：http://ql.newstarts.cn

Ruby: 42.to_s
来源：http://kg.asd995.cn

C#:   42.ToString()
来源：http://is.hahajie.cn

[A08] 取整与四舍五入
来源：http://sb.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vz.asd995.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ac.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xx.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sg.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bn.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://et.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://kp.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://td.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://ft.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tx.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tm.9csxet.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fd.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hf.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ss.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lj.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ir.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lv.9csxet.cn

[A10] 生成随机数
来源：http://sx.gzmigu.cn

Py:   import random; random.randint(1, 100)
来源：http://um.bookmarksfly.cn

PHP:  random_int(1, 100);
来源：http://pu.asd995.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cf.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ty.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://uj.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dz.muxihuayi.cn

Ruby: rand(1..100)
来源：http://ho.521024.cn

C#:   new Random().Next(1, 101)
来源：http://wo.nszjky.cn

[A11] 条件表达式（三元）
来源：http://pd.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://xi.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://if.nszjky.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qr.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kx.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://gf.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://js.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://et.lnxyls.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mi.shxzskj.cn

[A12] 字符串插值 / 格式化
来源：http://bk.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vz.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xu.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://ol.521024.cn

TS:   `Hello, ${name}!`
来源：http://ar.huanxung.cn

Java: "Hello, %s!".formatted(name)
来源：http://ig.szsharing.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dw.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://dk.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://ax.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gh.nicolike.cn

Py:   "第一行\n第二行"
来源：http://ai.bjjhwx.cn

PHP:  "第一行\n第二行"
来源：http://ph.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://ew.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://nf.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://xw.asd995.cn

Go:   "第一行\n第二行"
来源：http://ct.yuexingan06.cn

Ruby: "第一行\n第二行"
来源：http://wp.haigaiapp.cn

C#:   "第一行\n第二行"
来源：http://zk.newstarts.cn

[A14] 注释写法
来源：http://yq.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zi.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ku.yuexingan06.cn

JS:   // 单行；/* 多行 */
来源：http://xu.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://km.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uy.hahajie.cn

Go:   // 单行；/* 多行 */
来源：http://ct.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pm.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://eb.szxytkj.cn

[A15] 空值判断与默认值
来源：http://ok.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://yp.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://sj.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://rm.newstarts.cn

TS:   const value = data ?? "默认值";
来源：http://kq.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ya.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://cj.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://hd.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://tz.chemitech.net.cn

[A16] 真假值判断规则
来源：http://pk.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sm.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gh.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://aw.shxzukj.cn

TS:   if (!x) {}
来源：http://nb.szsharing.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gs.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rc.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nh.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://be.shtwfgs.cn

[A17] 位运算
来源：http://kj.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jk.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://td.hahajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://so.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jx.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xt.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://co.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xe.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ep.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://hx.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://bk.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://be.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bt.panjiajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kk.wgjwhj.cn

Java: (int) 'A'; (char) 65
来源：http://np.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tj.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://iz.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://km.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://um.shtwfgs.cn

Py:   a, b = b, a
来源：http://co.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ha.bookmarksfly.cn

JS:   [a, b] = [b, a];
来源：http://yu.asd995.cn

TS:   [a, b] = [b, a];
来源：http://ni.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://nt.bjjhwx.cn

Go:   a, b = b, a
来源：http://ae.muxihuayi.cn

Ruby: a, b = b, a
来源：http://ij.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://db.jctech888.com.cn

[A20] 读取标准输入
来源：http://wf.shxzskj.cn

Py:   name = input("请输入：")
来源：http://tg.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sv.yuntaijiaju.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cn.521024.cn

TS:   // Node.js：readline 模块
来源：http://dm.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://ct.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sn.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://mr.shxzukj.cn

C#:   Console.ReadLine();
来源：http://fh.huixiangedu.cn

[A21] 保留指定小数位输出
来源：http://nz.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://gp.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uu.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://go.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://lh.lnxyls.cn

Java: String.format("%.2f", 3.14159)
来源：http://mf.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qa.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://oa.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://rw.gzmigu.cn

[A22] 获取字符串长度
来源：http://tj.chemitech.net.cn

Py:   len(s)
来源：http://rd.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wq.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://br.shxzukj.cn

TS:   s.length
来源：http://bz.asd995.cn

Java: s.length()
来源：http://rv.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xk.nszjky.cn

Ruby: s.length
来源：http://bu.szsharing.cn

C#:   s.Length
来源：http://ht.nicolike.cn

[A23] 大小写转换
来源：http://ck.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bh.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ir.muxihuayi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hx.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ls.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hs.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gg.huixiangedu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bx.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ld.szsharing.cn

[A24] 去除首尾空白
来源：http://md.nszjky.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://os.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hi.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ka.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nl.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ub.panjiajie.cn

Go:   strings.TrimSpace(s)
来源：http://kb.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://kw.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ff.lnxyls.cn

[A25] 字符串比较
来源：http://hr.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://ko.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fi.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zz.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nm.jctech888.com.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zk.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yt.bookmarksfly.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rb.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ti.haigaiapp.cn

[A26] 类型转换总览
来源：http://rq.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gb.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vn.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nb.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://bm.huixiangedu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wa.yuntaijiaju.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mt.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sc.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tb.jctech888.com.cn

================================================================================
来源：http://sb.bjjhwx.cn

B. 流程控制
来源：http://bz.9csxet.cn

================================================================================
来源：http://kj.colortex.cn

[B01] 条件判断 if / else
来源：http://gc.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bk.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zw.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yi.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vx.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rw.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yl.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://id.gzmigu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xr.shtwfgs.cn

[B02] 多分支 else if / elif
来源：http://yj.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vl.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lh.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rl.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fv.yuexingan06.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aa.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vq.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qj.shxzukj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ap.gzmigu.cn

[B03] switch / match / case
来源：http://pi.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sb.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bw.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kf.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://as.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ft.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://di.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vl.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://be.shxzukj.cn

[B04] for 计数循环
来源：http://cu.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://hf.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fr.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qz.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bj.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lp.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wo.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://ia.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kw.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://bo.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://ef.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jr.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ly.szxytkj.cn


<!-- 参考信息 -->