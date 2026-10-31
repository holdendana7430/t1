代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xe.gzmigu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bf.haigaiapp.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zs.9csxet.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pc.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lb.bookmarksfly.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ce.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yy.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lz.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ef.bjjhwx.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lu.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vq.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ki.asd995.cn

================================================================================
来源：http://br.huanxung.cn

A. 基础语法与类型
来源：http://ui.szsharing.cn

================================================================================
来源：http://bd.asd995.cn

[A01] Hello World
来源：http://wn.nszjky.cn

Py:   print("Hello, World!")
来源：http://ub.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://up.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://be.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mg.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://js.nicolike.cn

Go:   fmt.Println("Hello, World!")
来源：http://tw.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://ga.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fu.newstarts.cn

[A02] 变量声明与赋值
来源：http://qo.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ya.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nv.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kb.huixiangedu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ma.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://dk.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://ja.newstarts.cn

Ruby: name = "Alex"; age = 20
来源：http://up.colortex.cn

C#:   string name = "Alex"; int age = 20;
来源：http://eg.asd995.cn

[A03] 常量定义
来源：http://yk.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://iy.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://vl.colortex.cn

JS:   const PI = 3.14159;
来源：http://ix.colortex.cn

TS:   const PI: number = 3.14159;
来源：http://om.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://ct.asd995.cn

Go:   const PI = 3.14159
来源：http://db.shxzukj.cn

Ruby: PI = 3.14159
来源：http://oq.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://vg.shxzukj.cn

[A04] 判断变量类型
来源：http://qn.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://os.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cj.521024.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dk.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://kd.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ma.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://aw.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tj.shxzukj.cn

C#:   x.GetType().Name; x is int
来源：http://jo.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://cj.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dw.jianghongdianzi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wl.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gh.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mg.shxzukj.cn

Java: 7 / 2; 7 % 2
来源：http://jy.huanxung.cn

Go:   7 / 2; 7 % 2
来源：http://xl.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://bf.521024.cn

C#:   7 / 2; 7 % 2
来源：http://by.shtwfgs.cn

[A06] 字符串转数字
来源：http://fl.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://dl.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://en.panjiajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lu.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ns.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://so.yuntaijiaju.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bs.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pc.asd995.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hf.9csxet.cn

[A07] 数字转字符串
来源：http://qk.jctech888.com.cn

Py:   str(42)
来源：http://ui.muxihuayi.cn

PHP:  (string) 42; strval(42)
来源：http://og.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://jk.huixiangedu.cn

TS:   String(42)
来源：http://cu.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nw.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://ot.huanxung.cn

Ruby: 42.to_s
来源：http://lv.shxzukj.cn

C#:   42.ToString()
来源：http://zb.nicolike.cn

[A08] 取整与四舍五入
来源：http://em.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cc.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qy.szxytkj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://np.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hy.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://by.huixiangedu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ox.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://kg.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hf.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://ga.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nc.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dq.newstarts.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mu.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gj.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xf.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dz.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ts.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ki.newstarts.cn

[A10] 生成随机数
来源：http://bv.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://xp.gzmigu.cn

PHP:  random_int(1, 100);
来源：http://ts.shxzukj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ee.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gi.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://pm.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://el.wgjwhj.cn

Ruby: rand(1..100)
来源：http://ut.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://yb.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://ls.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://fa.9csxet.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gm.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fp.panjiajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://hy.yuexingan06.cn

Java: x > 0 ? "yes" : "no"
来源：http://rd.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ja.yuntaijiaju.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://an.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ol.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://fb.huanxung.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rk.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uk.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://gg.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://gf.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://uf.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://op.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://hf.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://xe.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ij.szsharing.cn

Py:   "第一行\n第二行"
来源：http://jy.colortex.cn

PHP:  "第一行\n第二行"
来源：http://wn.szsharing.cn

JS:   "第一行\n第二行"
来源：http://sr.panjiajie.cn

TS:   "第一行\n第二行"
来源：http://lq.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://ze.newstarts.cn

Go:   "第一行\n第二行"
来源：http://bq.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://yv.nszjky.cn

C#:   "第一行\n第二行"
来源：http://hr.shxzukj.cn

[A14] 注释写法
来源：http://bj.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://df.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yv.bjjhwx.cn

JS:   // 单行；/* 多行 */
来源：http://hg.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://kh.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fp.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://ji.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qj.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://ad.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://ie.szxytkj.cn

Py:   value = data or "默认值"
来源：http://fn.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://ja.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://ut.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://kk.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qv.huixiangedu.cn

Go:   if data == "" { data = "默认值" }
来源：http://xz.bookmarksfly.cn

Ruby: value = data || "默认值"
来源：http://st.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://sj.521024.cn

[A16] 真假值判断规则
来源：http://eg.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ci.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xg.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pr.hahajie.cn

TS:   if (!x) {}
来源：http://tk.521024.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://je.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yb.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vd.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://or.haigaiapp.cn

[A17] 位运算
来源：http://vh.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ou.asd995.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mt.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nt.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://st.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kf.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oq.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hp.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pr.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://lx.wgjwhj.cn

Py:   ord("A"); chr(65)
来源：http://tw.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://ga.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pu.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wg.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://pk.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xt.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://ys.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://kt.haigaiapp.cn

[A19] 交换两个变量
来源：http://lu.colortex.cn

Py:   a, b = b, a
来源：http://ps.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ek.gzmigu.cn

JS:   [a, b] = [b, a];
来源：http://om.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://om.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://yq.jctech888.com.cn

Go:   a, b = b, a
来源：http://pj.panjiajie.cn

Ruby: a, b = b, a
来源：http://vh.yuexingan06.cn

C#:   (a, b) = (b, a);
来源：http://oq.huanxung.cn

[A20] 读取标准输入
来源：http://rv.chemitech.net.cn

Py:   name = input("请输入：")
来源：http://yp.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nv.lnxyls.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rr.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://gc.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://zw.colortex.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cq.jctech888.com.cn

Ruby: gets.chomp
来源：http://hl.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://ja.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://ta.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://oi.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kx.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://au.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://mu.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://pi.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mc.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://ts.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://yo.colortex.cn

[A22] 获取字符串长度
来源：http://rz.asd995.cn

Py:   len(s)
来源：http://kd.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ln.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gr.panjiajie.cn

TS:   s.length
来源：http://yz.haigaiapp.cn

Java: s.length()
来源：http://vo.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mq.newstarts.cn

Ruby: s.length
来源：http://jm.bookmarksfly.cn

C#:   s.Length
来源：http://eg.huixiangedu.cn

[A23] 大小写转换
来源：http://hn.lnxyls.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kn.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mp.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rk.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xl.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://na.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vt.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rd.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lx.newstarts.cn

[A24] 去除首尾空白
来源：http://ec.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://az.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rw.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sz.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vk.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oc.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://vr.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eg.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xb.huixinmuqiang.cn

[A25] 字符串比较
来源：http://ff.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://xw.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lg.hahajie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yd.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ax.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qq.panjiajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tg.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yc.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rb.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://mo.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sw.szxytkj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yw.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://av.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://ar.chemitech.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fd.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zw.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zw.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bi.colortex.cn

================================================================================
来源：http://al.panjiajie.cn

B. 流程控制
来源：http://bo.chemitech.net.cn

================================================================================
来源：http://nk.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://jh.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vb.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zf.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bx.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://at.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xo.huixiangedu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ef.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ey.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ql.nicolike.cn

[B02] 多分支 else if / elif
来源：http://zt.gzmigu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lb.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xq.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cw.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jx.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yx.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xf.nszjky.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mg.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://im.yuntaijiaju.cn

[B03] switch / match / case
来源：http://fr.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lt.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gg.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nw.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ru.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ol.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ol.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gk.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ut.yuntaijiaju.cn

[B04] for 计数循环
来源：http://de.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://al.hahajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ki.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mv.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nm.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bt.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tr.bookmarksfly.cn

Ruby: 10.times { |i| puts i }
来源：http://ri.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rl.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://ze.huixiangedu.cn

Py:   for item in arr: print(item)
来源：http://ru.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ej.yuntaijiaju.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bv.shxzskj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lk.colortex.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bz.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hl.shxzukj.cn

Ruby: arr.each { |item| puts item }
来源：http://kv.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sg.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://dh.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zf.newstarts.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rl.asd995.cn


<!-- 参考信息 -->