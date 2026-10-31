代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nl.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://un.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tl.colortex.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fx.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fv.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hr.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://oa.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dp.jianghongdianzi.cn

================================================================================
来源：http://fv.hahajie.cn

A. 基础语法与类型
来源：http://ss.muxihuayi.cn

================================================================================
来源：http://af.jctech888.com.cn

[A01] Hello World
来源：http://fz.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://ig.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://uy.asd995.cn

JS:   console.log("Hello, World!");
来源：http://sp.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rc.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://rs.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://sw.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://ve.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://az.jctech888.com.cn

[A02] 变量声明与赋值
来源：http://ik.bookmarksfly.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nw.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ws.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jm.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sb.bookmarksfly.cn

Java: String name = "Alex"; int age = 20;
来源：http://vf.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://ha.nicolike.cn

Ruby: name = "Alex"; age = 20
来源：http://db.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yy.colortex.cn

[A03] 常量定义
来源：http://tq.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vd.shtwfgs.cn

PHP:  const PI = 3.14159;
来源：http://vm.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://fs.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://lw.bjjhwx.cn

Java: static final double PI = 3.14159;
来源：http://bi.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://ub.colortex.cn

Ruby: PI = 3.14159
来源：http://cq.bjjhwx.cn

C#:   const double PI = 3.14159;
来源：http://cm.bjjhwx.cn

[A04] 判断变量类型
来源：http://tt.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://si.colortex.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ca.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://es.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://cl.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ge.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fx.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ma.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://el.wgjwhj.cn

[A05] 整数除法与取模
来源：http://dz.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kp.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fd.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zm.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qb.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://qp.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://ew.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://nu.asd995.cn

C#:   7 / 2; 7 % 2
来源：http://fb.wgjwhj.cn

[A06] 字符串转数字
来源：http://pz.colortex.cn

Py:   int("42"); float("3.14")
来源：http://uy.9csxet.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wh.nszjky.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mq.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pd.szsharing.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://re.nicolike.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://iv.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mr.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cl.huixiangedu.cn

[A07] 数字转字符串
来源：http://wu.9csxet.cn

Py:   str(42)
来源：http://se.lnxyls.cn

PHP:  (string) 42; strval(42)
来源：http://px.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://af.huixiangedu.cn

TS:   String(42)
来源：http://xv.9csxet.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bc.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://dd.nicolike.cn

Ruby: 42.to_s
来源：http://fg.szsharing.cn

C#:   42.ToString()
来源：http://mp.huixiangedu.cn

[A08] 取整与四舍五入
来源：http://ql.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ka.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ut.haigaiapp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ro.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oi.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fg.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hw.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qb.shxzukj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bt.wgjwhj.cn

[A09] 绝对值与最大最小值
来源：http://ba.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dl.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://im.521024.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zy.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nn.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://it.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://aa.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vw.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ls.huixiangedu.cn

[A10] 生成随机数
来源：http://cv.521024.cn

Py:   import random; random.randint(1, 100)
来源：http://jq.bookmarksfly.cn

PHP:  random_int(1, 100);
来源：http://he.521024.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://go.nicolike.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jt.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://tr.muxihuayi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jc.muxihuayi.cn

Ruby: rand(1..100)
来源：http://md.gzmigu.cn

C#:   new Random().Next(1, 101)
来源：http://pf.lnxyls.cn

[A11] 条件表达式（三元）
来源：http://ek.yuntaijiaju.cn

Py:   "yes" if x > 0 else "no"
来源：http://ld.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cc.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sg.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://de.yuexingan06.cn

Java: x > 0 ? "yes" : "no"
来源：http://sl.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ud.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ge.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ok.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://ke.newstarts.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qp.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lr.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://xu.huanxung.cn

TS:   `Hello, ${name}!`
来源：http://ir.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://kg.szsharing.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://su.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://zf.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://ve.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zg.521024.cn

Py:   "第一行\n第二行"
来源：http://ky.bjjhwx.cn

PHP:  "第一行\n第二行"
来源：http://ah.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://uc.szsharing.cn

TS:   "第一行\n第二行"
来源：http://tn.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://nq.hahajie.cn

Go:   "第一行\n第二行"
来源：http://sw.asd995.cn

Ruby: "第一行\n第二行"
来源：http://la.huanxung.cn

C#:   "第一行\n第二行"
来源：http://wk.colortex.cn

[A14] 注释写法
来源：http://pg.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gz.lnxyls.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wz.521024.cn

JS:   // 单行；/* 多行 */
来源：http://ze.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://nk.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fy.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://tu.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tk.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://rc.nszjky.cn

[A15] 空值判断与默认值
来源：http://ax.huixiangedu.cn

Py:   value = data or "默认值"
来源：http://mp.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://qe.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://ty.jctech888.com.cn

TS:   const value = data ?? "默认值";
来源：http://np.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hs.jianghongdianzi.cn

Go:   if data == "" { data = "默认值" }
来源：http://bb.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://nh.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://ny.lnxyls.cn

[A16] 真假值判断规则
来源：http://on.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oa.yuntaijiaju.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jo.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ns.521024.cn

TS:   if (!x) {}
来源：http://wb.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://aq.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qy.jctech888.com.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oq.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hl.colortex.cn

[A17] 位运算
来源：http://az.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wg.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gq.hahajie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bu.gzmigu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hk.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ih.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gw.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oo.huixiangedu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://da.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://jr.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://vp.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://hn.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://db.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fq.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://ws.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lj.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://xz.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://mq.jctech888.com.cn

[A19] 交换两个变量
来源：http://os.haigaiapp.cn

Py:   a, b = b, a
来源：http://vf.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://da.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://rd.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://fz.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://yn.szxytkj.cn

Go:   a, b = b, a
来源：http://jo.shtwfgs.cn

Ruby: a, b = b, a
来源：http://ga.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://jo.szxytkj.cn

[A20] 读取标准输入
来源：http://ra.hahajie.cn

Py:   name = input("请输入：")
来源：http://yn.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vn.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://be.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://tr.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://ri.huixiangedu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ls.yuntaijiaju.cn

Ruby: gets.chomp
来源：http://ik.9csxet.cn

C#:   Console.ReadLine();
来源：http://hj.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://jy.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://ue.huanxung.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qr.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://tg.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://vv.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://ps.hnjuh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lh.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://nx.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://nf.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://hn.huanxung.cn

Py:   len(s)
来源：http://gk.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gk.lnxyls.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bx.wgjwhj.cn

TS:   s.length
来源：http://tv.shxzskj.cn

Java: s.length()
来源：http://vr.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fc.yuntaijiaju.cn

Ruby: s.length
来源：http://ax.gzmigu.cn

C#:   s.Length
来源：http://et.hahajie.cn

[A23] 大小写转换
来源：http://pg.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xw.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fl.panjiajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uh.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cr.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vd.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ox.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pu.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vz.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://oy.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nd.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ih.bookmarksfly.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lo.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cp.huanxung.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gv.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://wn.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ke.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pe.hahajie.cn

[A25] 字符串比较
来源：http://ns.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://kz.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vk.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://um.wgjwhj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hn.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://we.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qg.szxytkj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lx.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vd.haigaiapp.cn

[A26] 类型转换总览
来源：http://zj.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hd.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zz.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aj.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://gz.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uu.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iz.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oe.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ca.szsharing.cn

================================================================================
来源：http://gp.colortex.cn

B. 流程控制
来源：http://cp.shxzukj.cn

================================================================================
来源：http://se.yuexingan06.cn

[B01] 条件判断 if / else
来源：http://dh.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oe.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pg.hnjuh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yb.9csxet.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lp.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qq.colortex.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://px.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kw.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ef.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://ix.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tv.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ld.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iy.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qn.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nj.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xn.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nq.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bu.huixinmuqiang.cn

[B03] switch / match / case
来源：http://id.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ew.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pd.colortex.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yo.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mo.gzmigu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pb.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lt.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nd.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tv.lnxyls.cn

[B04] for 计数循环
来源：http://ri.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://er.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eq.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mo.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nr.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xp.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rv.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://ln.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://st.521024.cn

[B05] 遍历数组 / 列表
来源：http://tm.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://ni.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yn.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ej.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://it.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nv.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yw.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://dg.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ba.chemitech.net.cn

[B06] 遍历字典 / 对象
来源：http://le.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qc.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sk.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eg.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ps.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bx.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kb.huixiangedu.cn


<!-- 参考信息 -->