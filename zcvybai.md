代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://ww.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://bm.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://ui.nszjky.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lt.hahajie.cn

[A02] 变量声明与赋值
来源：http://yq.muxihuayi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tf.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nq.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hw.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hx.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://cz.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://qx.nicolike.cn

Ruby: name = "Alex"; age = 20
来源：http://zn.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fh.huixiangedu.cn

[A03] 常量定义
来源：http://gz.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://al.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://ka.shxzukj.cn

JS:   const PI = 3.14159;
来源：http://yl.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://ga.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://vm.nszjky.cn

Go:   const PI = 3.14159
来源：http://wv.shtwfgs.cn

Ruby: PI = 3.14159
来源：http://vb.huanxung.cn

C#:   const double PI = 3.14159;
来源：http://ck.szsharing.cn

[A04] 判断变量类型
来源：http://aw.shtwfgs.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bs.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://eo.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sc.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://xl.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sk.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ws.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lt.szsharing.cn

C#:   x.GetType().Name; x is int
来源：http://dg.jctech888.com.cn

[A05] 整数除法与取模
来源：http://rd.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rr.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gc.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ec.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sa.jctech888.com.cn

Java: 7 / 2; 7 % 2
来源：http://yr.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://fs.szxytkj.cn

Ruby: 7 / 2; 7 % 2
来源：http://fd.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://ba.lnxyls.cn

[A06] 字符串转数字
来源：http://vn.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://ln.asd995.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ze.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gr.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ac.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wh.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ng.asd995.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://aa.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://au.chemitech.net.cn

[A07] 数字转字符串
来源：http://uq.szsharing.cn

Py:   str(42)
来源：http://zg.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://hs.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://jz.521024.cn

TS:   String(42)
来源：http://pj.bookmarksfly.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yq.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://iv.9csxet.cn

Ruby: 42.to_s
来源：http://sq.521024.cn

C#:   42.ToString()
来源：http://hv.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://mc.chemitech.net.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://py.szsharing.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wk.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mk.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kf.jctech888.com.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kj.bookmarksfly.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bx.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dc.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kh.bookmarksfly.cn

[A09] 绝对值与最大最小值
来源：http://hc.gzmigu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://op.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zi.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://il.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vs.szxytkj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kj.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ok.huanxung.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cf.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://em.bjjhwx.cn

[A10] 生成随机数
来源：http://pb.shxzukj.cn

Py:   import random; random.randint(1, 100)
来源：http://vk.9csxet.cn

PHP:  random_int(1, 100);
来源：http://uc.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://od.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ct.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://vf.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sp.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://og.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://rw.yuexingan06.cn

[A11] 条件表达式（三元）
来源：http://rm.huixiangedu.cn

Py:   "yes" if x > 0 else "no"
来源：http://au.521024.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://uf.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ov.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://el.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://ob.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gl.yuntaijiaju.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mj.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jh.521024.cn

[A12] 字符串插值 / 格式化
来源：http://rt.lnxyls.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xi.yuntaijiaju.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pw.asd995.cn

JS:   `Hello, ${name}!`
来源：http://zf.gzmigu.cn

TS:   `Hello, ${name}!`
来源：http://ga.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://kp.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cn.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://mt.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://pv.yuexingan06.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ay.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://gu.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://cd.wgjwhj.cn

JS:   "第一行\n第二行"
来源：http://gp.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://jl.panjiajie.cn

Java: "第一行\n第二行"
来源：http://xc.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://oy.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://bc.asd995.cn

C#:   "第一行\n第二行"
来源：http://hz.bjjhwx.cn

[A14] 注释写法
来源：http://dc.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ur.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ya.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://kw.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://uv.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://st.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://rq.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jr.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://qh.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://tx.9csxet.cn

Py:   value = data or "默认值"
来源：http://ai.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://sl.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://oj.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://hr.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xz.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://ko.newstarts.cn

Ruby: value = data || "默认值"
来源：http://sb.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://ce.jianghongdianzi.cn

[A16] 真假值判断规则
来源：http://hi.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ka.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kd.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://id.muxihuayi.cn

TS:   if (!x) {}
来源：http://mm.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dd.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lh.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xu.hnjuh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pw.chemitech.net.cn

[A17] 位运算
来源：http://cc.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nv.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kz.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kf.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://es.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ly.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qw.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gk.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dv.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://xm.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://gw.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://rz.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xj.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pj.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://pr.bookmarksfly.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nx.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://je.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://do.hnjuh.cn

[A19] 交换两个变量
来源：http://cd.newstarts.cn

Py:   a, b = b, a
来源：http://ku.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lt.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://zx.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://kv.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://ew.nszjky.cn

Go:   a, b = b, a
来源：http://oi.shtwfgs.cn

Ruby: a, b = b, a
来源：http://lp.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://vk.bookmarksfly.cn

[A20] 读取标准输入
来源：http://jg.hahajie.cn

Py:   name = input("请输入：")
来源：http://iy.huixinmuqiang.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pc.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://iv.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://cl.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://tp.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xk.huixinmuqiang.cn

Ruby: gets.chomp
来源：http://te.newstarts.cn

C#:   Console.ReadLine();
来源：http://vj.jianghongdianzi.cn

[A21] 保留指定小数位输出
来源：http://bx.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://xl.nszjky.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ej.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://hz.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://vi.wgjwhj.cn

Java: String.format("%.2f", 3.14159)
来源：http://db.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://iz.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://ds.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://ss.shxzskj.cn

[A22] 获取字符串长度
来源：http://te.521024.cn

Py:   len(s)
来源：http://ra.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dw.hahajie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ls.huixinmuqiang.cn

TS:   s.length
来源：http://uy.lnxyls.cn

Java: s.length()
来源：http://tw.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://at.hahajie.cn

Ruby: s.length
来源：http://nb.521024.cn

C#:   s.Length
来源：http://xq.nicolike.cn

[A23] 大小写转换
来源：http://wr.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://at.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dr.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mb.szsharing.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ht.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sr.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lv.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xq.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fs.shxzskj.cn

[A24] 去除首尾空白
来源：http://jm.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pl.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://na.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://do.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://in.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pz.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://oi.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gu.colortex.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cp.shtwfgs.cn

[A25] 字符串比较
来源：http://hi.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://bp.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wc.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qm.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qu.chemitech.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ku.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zh.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://va.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hy.hahajie.cn

[A26] 类型转换总览
来源：http://sh.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zt.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qw.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://en.bookmarksfly.cn

TS:   Number() String() Boolean() x as number
来源：http://em.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tm.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fc.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ko.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qr.gzmigu.cn

================================================================================
来源：http://vz.lnxyls.cn

B. 流程控制
来源：http://in.asd995.cn

================================================================================
来源：http://is.haigaiapp.cn

[B01] 条件判断 if / else
来源：http://sy.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://id.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lj.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zb.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ti.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mh.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://da.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qk.haigaiapp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yx.521024.cn

[B02] 多分支 else if / elif
来源：http://os.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pw.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eu.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://er.gzmigu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mb.huixinmuqiang.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hl.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fm.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jh.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yk.panjiajie.cn

[B03] switch / match / case
来源：http://qn.newstarts.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jd.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ps.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pv.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ue.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tq.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vv.wgjwhj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qs.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mo.yuntaijiaju.cn

[B04] for 计数循环
来源：http://tj.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://pf.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://be.bookmarksfly.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ne.yuexingan06.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://td.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aa.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yo.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://jo.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yb.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://uu.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://wz.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nh.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qc.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ea.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rd.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kr.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://kb.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mp.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://if.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://od.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eo.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uy.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vi.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ap.colortex.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://im.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ab.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ye.shxzskj.cn

[B07] while 循环
来源：http://ti.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://sx.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://am.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://ap.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://ze.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://xa.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ce.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://jy.521024.cn

C#:   while (i < 10) { i++; }
来源：http://dc.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://kk.huixinmuqiang.cn

Py:   # 无 do-while：用 while True + break
来源：http://dp.hnjuh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yy.lnxyls.cn

JS:   do { i++; } while (i < 10);
来源：http://ys.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://gy.huanxung.cn


<!-- 参考信息 -->