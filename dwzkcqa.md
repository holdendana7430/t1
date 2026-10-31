代发 wailian999

[A02] 变量声明与赋值
来源：http://mu.szxytkj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dg.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zz.panjiajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ru.gzmigu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gg.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://qj.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://zc.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://mo.bookmarksfly.cn

C#:   string name = "Alex"; int age = 20;
来源：http://th.szsharing.cn

[A03] 常量定义
来源：http://gj.521024.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ho.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://kp.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://kw.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://wh.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://hi.shxzukj.cn

Go:   const PI = 3.14159
来源：http://nh.hahajie.cn

Ruby: PI = 3.14159
来源：http://rl.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://ik.521024.cn

[A04] 判断变量类型
来源：http://tx.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ky.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ia.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gq.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://oh.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yd.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ik.asd995.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://bp.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://fe.hahajie.cn

[A05] 整数除法与取模
来源：http://de.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kq.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://an.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qc.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vj.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://zr.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://hd.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://lh.bookmarksfly.cn

C#:   7 / 2; 7 % 2
来源：http://ul.bjjhwx.cn

[A06] 字符串转数字
来源：http://tn.jianghongdianzi.cn

Py:   int("42"); float("3.14")
来源：http://qs.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pj.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vm.shxzukj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rd.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xu.lnxyls.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gl.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qp.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vw.huanxung.cn

[A07] 数字转字符串
来源：http://vw.muxihuayi.cn

Py:   str(42)
来源：http://ol.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://uk.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://ip.panjiajie.cn

TS:   String(42)
来源：http://xx.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ao.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://uv.hahajie.cn

Ruby: 42.to_s
来源：http://ol.9csxet.cn

C#:   42.ToString()
来源：http://kv.jctech888.com.cn

[A08] 取整与四舍五入
来源：http://dh.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ty.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qv.521024.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://le.szxytkj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eo.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sk.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://iw.yuntaijiaju.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gv.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sn.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://hl.jctech888.com.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ez.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dg.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://oz.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lx.szsharing.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ko.hahajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://st.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wc.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fw.huixiangedu.cn

[A10] 生成随机数
来源：http://qz.bjjhwx.cn

Py:   import random; random.randint(1, 100)
来源：http://xv.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://mj.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mn.jianghongdianzi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kz.szsharing.cn

Java: new Random().nextInt(100) + 1
来源：http://qf.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ye.shtwfgs.cn

Ruby: rand(1..100)
来源：http://kd.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://eg.newstarts.cn

[A11] 条件表达式（三元）
来源：http://sg.hnjuh.cn

Py:   "yes" if x > 0 else "no"
来源：http://vg.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rq.newstarts.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yh.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ea.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://dy.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xl.muxihuayi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cn.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ky.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://wv.hnjuh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kp.chemitech.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hk.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://ef.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://es.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://uf.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pt.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://ma.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://bx.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ja.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://xs.shxzukj.cn

PHP:  "第一行\n第二行"
来源：http://rw.hahajie.cn

JS:   "第一行\n第二行"
来源：http://zi.9csxet.cn

TS:   "第一行\n第二行"
来源：http://hf.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://ps.huanxung.cn

Go:   "第一行\n第二行"
来源：http://ym.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://jh.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://tc.nicolike.cn

[A14] 注释写法
来源：http://ol.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zz.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zj.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://ji.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://ge.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bb.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://pe.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pz.9csxet.cn

C#:   // 单行；/* 多行 */
来源：http://un.hnjuh.cn

[A15] 空值判断与默认值
来源：http://nd.nszjky.cn

Py:   value = data or "默认值"
来源：http://gf.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://kq.gzmigu.cn

JS:   const value = data ?? "默认值";
来源：http://if.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://bs.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hb.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://lg.colortex.cn

Ruby: value = data || "默认值"
来源：http://gb.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://ok.huanxung.cn

[A16] 真假值判断规则
来源：http://od.9csxet.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://co.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ke.nszjky.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rx.nicolike.cn

TS:   if (!x) {}
来源：http://tp.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ha.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bh.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gt.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qt.huanxung.cn

[A17] 位运算
来源：http://dh.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dj.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://aq.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nb.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bo.hahajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qh.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cz.lnxyls.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ll.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ls.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://qs.szsharing.cn

Py:   ord("A"); chr(65)
来源：http://ci.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://kf.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gp.lnxyls.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://es.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://gt.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ch.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://qx.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://jc.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://td.haigaiapp.cn

Py:   a, b = b, a
来源：http://nw.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://up.yuntaijiaju.cn

JS:   [a, b] = [b, a];
来源：http://jq.muxihuayi.cn

TS:   [a, b] = [b, a];
来源：http://zk.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://qg.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://vi.hnjuh.cn

Ruby: a, b = b, a
来源：http://rh.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://ih.wgjwhj.cn

[A20] 读取标准输入
来源：http://si.shxzskj.cn

Py:   name = input("请输入：")
来源：http://tu.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://df.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ed.nszjky.cn

TS:   // Node.js：readline 模块
来源：http://ox.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://at.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vp.nicolike.cn

Ruby: gets.chomp
来源：http://qa.szxytkj.cn

C#:   Console.ReadLine();
来源：http://gt.nicolike.cn

[A21] 保留指定小数位输出
来源：http://fk.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://lk.gzmigu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://if.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://vo.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://hb.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://ad.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zt.szxytkj.cn

Ruby: format("%.2f", 3.14159)
来源：http://hi.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://se.huixiangedu.cn

[A22] 获取字符串长度
来源：http://vq.jctech888.com.cn

Py:   len(s)
来源：http://ru.hnjuh.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xt.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wt.huanxung.cn

TS:   s.length
来源：http://ku.nszjky.cn

Java: s.length()
来源：http://qh.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wk.colortex.cn

Ruby: s.length
来源：http://ok.huixinmuqiang.cn

C#:   s.Length
来源：http://up.bjjhwx.cn

[A23] 大小写转换
来源：http://xp.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ou.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ba.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hj.jianghongdianzi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gf.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gh.521024.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nu.yuexingan06.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://od.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fs.newstarts.cn

[A24] 去除首尾空白
来源：http://fv.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://al.asd995.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cm.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qq.shxzukj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://is.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ho.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://im.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jp.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jo.asd995.cn

[A25] 字符串比较
来源：http://rf.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://qc.panjiajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hb.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iz.hnjuh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rm.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sd.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bi.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sq.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ta.wgjwhj.cn

[A26] 类型转换总览
来源：http://bp.colortex.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sz.hnjuh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nf.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gd.nszjky.cn

TS:   Number() String() Boolean() x as number
来源：http://pf.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wm.jianghongdianzi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nj.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ya.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ue.shtwfgs.cn

================================================================================
来源：http://fr.shtwfgs.cn

B. 流程控制
来源：http://fo.yuntaijiaju.cn

================================================================================
来源：http://kd.hahajie.cn

[B01] 条件判断 if / else
来源：http://ah.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://en.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zz.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hq.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bn.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mq.panjiajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pr.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ao.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yr.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://dk.shxzukj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mv.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tm.chemitech.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://in.9csxet.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gp.muxihuayi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jw.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ag.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xi.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ox.bookmarksfly.cn

[B03] switch / match / case
来源：http://oq.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lt.haigaiapp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lm.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uj.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tg.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ne.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nj.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://me.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://of.colortex.cn

[B04] for 计数循环
来源：http://fb.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://mk.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yd.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lg.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vz.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dz.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pn.huixinmuqiang.cn

Ruby: 10.times { |i| puts i }
来源：http://zh.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cs.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://ub.bookmarksfly.cn

Py:   for item in arr: print(item)
来源：http://pe.colortex.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ct.shtwfgs.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gu.szxytkj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pa.yuexingan06.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mr.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kc.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://bn.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gy.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://ct.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lg.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jv.muxihuayi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://te.jctech888.com.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qe.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vs.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tn.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tm.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ot.bjjhwx.cn

[B07] while 循环
来源：http://lp.chemitech.net.cn

Py:   while i < 10: i += 1
来源：http://jw.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ng.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://fe.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://cc.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://yp.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://us.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://vp.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://ar.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://an.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://fq.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ba.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://ne.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://hr.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://bk.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oz.yuexingan06.cn

Ruby: begin; i += 1; end while i < 10
来源：http://we.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://gb.huixinmuqiang.cn


<!-- 参考信息 -->