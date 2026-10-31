代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://gp.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ux.huixinmuqiang.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yh.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kh.haigaiapp.cn

================================================================================
来源：http://ff.9csxet.cn

A. 基础语法与类型
来源：http://vi.yuntaijiaju.cn

================================================================================
来源：http://dw.panjiajie.cn

[A01] Hello World
来源：http://fz.szsharing.cn

Py:   print("Hello, World!")
来源：http://rj.colortex.cn

PHP:  echo "Hello, World!";
来源：http://tu.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://lh.hahajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tn.yuexingan06.cn

Java: System.out.println("Hello, World!");
来源：http://ld.huixiangedu.cn

Go:   fmt.Println("Hello, World!")
来源：http://eh.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://lb.lnxyls.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nw.huixinmuqiang.cn

[A02] 变量声明与赋值
来源：http://pt.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zb.chemitech.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ru.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vm.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qz.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://hr.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://wi.wgjwhj.cn

Ruby: name = "Alex"; age = 20
来源：http://tj.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nz.shtwfgs.cn

[A03] 常量定义
来源：http://sr.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dh.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://es.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://ah.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://fx.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://iu.nszjky.cn

Go:   const PI = 3.14159
来源：http://ve.szxytkj.cn

Ruby: PI = 3.14159
来源：http://vy.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://so.newstarts.cn

[A04] 判断变量类型
来源：http://px.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zn.nszjky.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ep.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jm.muxihuayi.cn

TS:   typeof x; x instanceof Date
来源：http://jk.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://et.yuexingan06.cn

Go:   reflect.TypeOf(x).Name()
来源：http://oo.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ak.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://es.chemitech.net.cn

[A05] 整数除法与取模
来源：http://nn.yuexingan06.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ji.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wz.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zn.shxzukj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jd.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://ql.521024.cn

Go:   7 / 2; 7 % 2
来源：http://qb.521024.cn

Ruby: 7 / 2; 7 % 2
来源：http://mp.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://it.szsharing.cn

[A06] 字符串转数字
来源：http://ok.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://ua.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cc.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gq.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xc.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rv.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ib.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ai.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rk.shxzskj.cn

[A07] 数字转字符串
来源：http://ty.shtwfgs.cn

Py:   str(42)
来源：http://uz.bjjhwx.cn

PHP:  (string) 42; strval(42)
来源：http://qb.szsharing.cn

JS:   String(42); (42).toString()
来源：http://vm.9csxet.cn

TS:   String(42)
来源：http://mz.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://mk.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://fd.gzmigu.cn

Ruby: 42.to_s
来源：http://sv.yuexingan06.cn

C#:   42.ToString()
来源：http://zi.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://nw.shxzukj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://id.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xs.shxzukj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nf.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ca.521024.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://df.huixiangedu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wy.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vf.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fj.asd995.cn

[A09] 绝对值与最大最小值
来源：http://az.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vd.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qo.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rv.colortex.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mo.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ea.gzmigu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kn.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zc.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bf.jianghongdianzi.cn

[A10] 生成随机数
来源：http://bm.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://hw.yuntaijiaju.cn

PHP:  random_int(1, 100);
来源：http://xc.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gz.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xa.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://mr.newstarts.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ln.panjiajie.cn

Ruby: rand(1..100)
来源：http://cx.shtwfgs.cn

C#:   new Random().Next(1, 101)
来源：http://rs.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://nt.huixiangedu.cn

Py:   "yes" if x > 0 else "no"
来源：http://pu.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fi.huixinmuqiang.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fn.asd995.cn

TS:   x > 0 ? "yes" : "no"
来源：http://tc.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://fj.yuexingan06.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pi.panjiajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ql.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kw.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://da.gzmigu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uq.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zz.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://nc.asd995.cn

TS:   `Hello, ${name}!`
来源：http://ka.9csxet.cn

Java: "Hello, %s!".formatted(name)
来源：http://ow.shxzskj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zv.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://fg.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://qi.newstarts.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ge.yuexingan06.cn

Py:   "第一行\n第二行"
来源：http://vt.bjjhwx.cn

PHP:  "第一行\n第二行"
来源：http://ld.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://gg.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://an.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://tb.colortex.cn

Go:   "第一行\n第二行"
来源：http://gw.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://aa.shtwfgs.cn

C#:   "第一行\n第二行"
来源：http://sp.shxzukj.cn

[A14] 注释写法
来源：http://jd.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nn.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wp.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://yq.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://yv.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rv.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://qd.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vn.9csxet.cn

C#:   // 单行；/* 多行 */
来源：http://do.nszjky.cn

[A15] 空值判断与默认值
来源：http://cg.newstarts.cn

Py:   value = data or "默认值"
来源：http://nj.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://hp.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://xs.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://bs.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yo.chemitech.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://vn.lnxyls.cn

Ruby: value = data || "默认值"
来源：http://gj.yuntaijiaju.cn

C#:   var value = data ?? "默认值";
来源：http://qi.panjiajie.cn

[A16] 真假值判断规则
来源：http://bs.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ji.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://up.jianghongdianzi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jd.nicolike.cn

TS:   if (!x) {}
来源：http://pj.521024.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ip.chemitech.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mn.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jx.huanxung.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bp.bookmarksfly.cn

[A17] 位运算
来源：http://bn.muxihuayi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lf.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://im.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mo.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://df.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ek.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qm.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ew.newstarts.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rj.panjiajie.cn

[A18] 字符与 ASCII 码互转
来源：http://kz.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://kh.newstarts.cn

PHP:  ord("A"); chr(65)
来源：http://nk.haigaiapp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pe.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wa.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://xj.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pk.newstarts.cn

Ruby: "A".ord; 65.chr
来源：http://ss.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://ho.gzmigu.cn

[A19] 交换两个变量
来源：http://hx.newstarts.cn

Py:   a, b = b, a
来源：http://qt.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mm.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://my.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://fm.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://sx.szxytkj.cn

Go:   a, b = b, a
来源：http://kg.lnxyls.cn

Ruby: a, b = b, a
来源：http://fe.haigaiapp.cn

C#:   (a, b) = (b, a);
来源：http://la.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://te.asd995.cn

Py:   name = input("请输入：")
来源：http://fs.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fr.nicolike.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ne.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://ri.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://xh.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eq.szxytkj.cn

Ruby: gets.chomp
来源：http://re.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://sp.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://om.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://jl.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gj.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://wt.huanxung.cn

TS:   (3.14159).toFixed(2)
来源：http://jh.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://nm.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jf.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://wn.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://wx.nszjky.cn

[A22] 获取字符串长度
来源：http://ht.yuexingan06.cn

Py:   len(s)
来源：http://lw.huixiangedu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wp.panjiajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zq.szsharing.cn

TS:   s.length
来源：http://tf.bjjhwx.cn

Java: s.length()
来源：http://si.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lm.huixinmuqiang.cn

Ruby: s.length
来源：http://hz.lnxyls.cn

C#:   s.Length
来源：http://ug.nicolike.cn

[A23] 大小写转换
来源：http://hz.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://np.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kk.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jl.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kt.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nd.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qq.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vi.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bo.asd995.cn

[A24] 去除首尾空白
来源：http://kv.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ap.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rl.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ul.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ut.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zm.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://jx.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rt.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kt.nszjky.cn

[A25] 字符串比较
来源：http://pl.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://ly.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pm.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://to.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wd.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rl.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cd.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pg.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sq.shxzukj.cn

[A26] 类型转换总览
来源：http://er.haigaiapp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sj.yuntaijiaju.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ox.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hv.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://gh.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mo.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vz.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gg.9csxet.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ut.9csxet.cn

================================================================================
来源：http://nr.shxzskj.cn

B. 流程控制
来源：http://on.nszjky.cn

================================================================================
来源：http://qe.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://kw.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aj.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ck.nszjky.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://al.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dh.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qh.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gl.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eb.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ar.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://tg.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xu.szxytkj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pe.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zb.panjiajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lm.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jz.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wo.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yx.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://el.bjjhwx.cn

[B03] switch / match / case
来源：http://ps.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cj.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cy.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://px.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zo.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jz.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ie.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zw.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vd.shxzukj.cn

[B04] for 计数循环
来源：http://ig.asd995.cn

Py:   for i in range(10): print(i)
来源：http://iy.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xq.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ca.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ix.newstarts.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sc.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ce.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://zh.huanxung.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mu.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://jf.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://ld.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://go.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://of.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oe.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://km.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pw.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://dw.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xt.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://ov.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://px.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://du.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ky.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yd.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vl.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ew.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hq.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zr.jianghongdianzi.cn

[B07] while 循环
来源：http://yt.szsharing.cn

Py:   while i < 10: i += 1
来源：http://rv.asd995.cn


<!-- 参考信息 -->