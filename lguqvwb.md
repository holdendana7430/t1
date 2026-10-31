代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://zy.huixinmuqiang.cn

[A03] 常量定义
来源：http://zw.nicolike.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://em.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://al.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://pu.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://pj.haigaiapp.cn

Java: static final double PI = 3.14159;
来源：http://ke.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://qn.shtwfgs.cn

Ruby: PI = 3.14159
来源：http://wz.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://cw.bookmarksfly.cn

[A04] 判断变量类型
来源：http://tu.shtwfgs.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://by.asd995.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oc.nszjky.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uh.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://ci.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ob.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fg.chemitech.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sa.wgjwhj.cn

C#:   x.GetType().Name; x is int
来源：http://xl.asd995.cn

[A05] 整数除法与取模
来源：http://gh.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ce.jianghongdianzi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://oh.521024.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qu.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://th.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://kl.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://ke.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://sx.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://mw.gzmigu.cn

[A06] 字符串转数字
来源：http://hj.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://jg.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ia.newstarts.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wq.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gl.huixinmuqiang.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nr.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ru.huixinmuqiang.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xb.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jd.szxytkj.cn

[A07] 数字转字符串
来源：http://xv.panjiajie.cn

Py:   str(42)
来源：http://hf.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://vo.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://fq.muxihuayi.cn

TS:   String(42)
来源：http://en.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ln.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://ry.huixinmuqiang.cn

Ruby: 42.to_s
来源：http://kc.panjiajie.cn

C#:   42.ToString()
来源：http://ia.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://cd.haigaiapp.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oa.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ge.szxytkj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cv.bookmarksfly.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sv.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pq.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kz.jianghongdianzi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pg.shxzskj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dk.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://gz.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://go.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://we.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ae.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xw.szsharing.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pu.lnxyls.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vf.521024.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://za.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zd.lnxyls.cn

[A10] 生成随机数
来源：http://tj.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://yy.huanxung.cn

PHP:  random_int(1, 100);
来源：http://ew.shxzukj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ve.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://aa.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://nu.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wz.jctech888.com.cn

Ruby: rand(1..100)
来源：http://mu.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://qv.gzmigu.cn

[A11] 条件表达式（三元）
来源：http://ca.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://mc.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://md.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://le.hahajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kc.szsharing.cn

Java: x > 0 ? "yes" : "no"
来源：http://jr.wgjwhj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xa.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hd.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fp.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://cz.yuntaijiaju.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hm.huixiangedu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bp.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://pe.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://xv.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://kd.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jo.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://fb.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://ke.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://nx.colortex.cn

Py:   "第一行\n第二行"
来源：http://cg.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://sb.asd995.cn

JS:   "第一行\n第二行"
来源：http://vm.huanxung.cn

TS:   "第一行\n第二行"
来源：http://ml.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://rr.huixinmuqiang.cn

Go:   "第一行\n第二行"
来源：http://ug.asd995.cn

Ruby: "第一行\n第二行"
来源：http://dl.asd995.cn

C#:   "第一行\n第二行"
来源：http://ue.hnjuh.cn

[A14] 注释写法
来源：http://fs.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kr.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kd.huanxung.cn

JS:   // 单行；/* 多行 */
来源：http://av.wgjwhj.cn

TS:   // 单行；/* 多行 */
来源：http://tz.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pt.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://cc.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ld.bookmarksfly.cn

C#:   // 单行；/* 多行 */
来源：http://yb.shtwfgs.cn

[A15] 空值判断与默认值
来源：http://oc.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://ei.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://fv.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://bs.muxihuayi.cn

TS:   const value = data ?? "默认值";
来源：http://xc.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gp.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://px.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://eh.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://fz.huanxung.cn

[A16] 真假值判断规则
来源：http://xp.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eh.nicolike.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tx.panjiajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xz.yuexingan06.cn

TS:   if (!x) {}
来源：http://kk.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ml.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yy.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yy.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://li.wgjwhj.cn

[A17] 位运算
来源：http://md.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vz.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bt.bookmarksfly.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hg.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dj.szxytkj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yl.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gd.huixinmuqiang.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nf.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wi.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://bg.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://zk.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://nq.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nx.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tn.haigaiapp.cn

Java: (int) 'A'; (char) 65
来源：http://rt.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qa.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://qk.colortex.cn

C#:   (int)'A'; (char)65
来源：http://rq.yuexingan06.cn

[A19] 交换两个变量
来源：http://il.9csxet.cn

Py:   a, b = b, a
来源：http://us.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lo.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://ju.nszjky.cn

TS:   [a, b] = [b, a];
来源：http://vs.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://uc.9csxet.cn

Go:   a, b = b, a
来源：http://zy.chemitech.net.cn

Ruby: a, b = b, a
来源：http://od.huanxung.cn

C#:   (a, b) = (b, a);
来源：http://me.szsharing.cn

[A20] 读取标准输入
来源：http://hl.hnjuh.cn

Py:   name = input("请输入：")
来源：http://yp.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fc.newstarts.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rh.asd995.cn

TS:   // Node.js：readline 模块
来源：http://ux.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://ng.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bo.colortex.cn

Ruby: gets.chomp
来源：http://eq.yuntaijiaju.cn

C#:   Console.ReadLine();
来源：http://cy.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://mr.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://gy.chemitech.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ko.huanxung.cn

JS:   (3.14159).toFixed(2)
来源：http://ts.yuexingan06.cn

TS:   (3.14159).toFixed(2)
来源：http://gh.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://fn.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://el.szsharing.cn

Ruby: format("%.2f", 3.14159)
来源：http://qy.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://mw.jctech888.com.cn

[A22] 获取字符串长度
来源：http://sm.chemitech.net.cn

Py:   len(s)
来源：http://vq.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bf.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vm.bjjhwx.cn

TS:   s.length
来源：http://sx.szxytkj.cn

Java: s.length()
来源：http://fm.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wk.jctech888.com.cn

Ruby: s.length
来源：http://kn.shxzskj.cn

C#:   s.Length
来源：http://zi.yuntaijiaju.cn

[A23] 大小写转换
来源：http://nq.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ib.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jf.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mi.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qe.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tb.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ez.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gx.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ha.huixiangedu.cn

[A24] 去除首尾空白
来源：http://yn.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ve.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mb.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ub.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jz.panjiajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wh.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://sv.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ar.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xz.521024.cn

[A25] 字符串比较
来源：http://vn.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://lu.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wv.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ab.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ln.muxihuayi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pu.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lg.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hn.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tt.hnjuh.cn

[A26] 类型转换总览
来源：http://tf.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nf.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://by.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xp.lnxyls.cn

TS:   Number() String() Boolean() x as number
来源：http://vf.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://um.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hw.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://sx.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hv.szsharing.cn

================================================================================
来源：http://qo.bookmarksfly.cn

B. 流程控制
来源：http://yq.huanxung.cn

================================================================================
来源：http://hq.muxihuayi.cn

[B01] 条件判断 if / else
来源：http://lv.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hl.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zf.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gs.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://il.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pl.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fm.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rx.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ke.haigaiapp.cn

[B02] 多分支 else if / elif
来源：http://bc.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xv.nszjky.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xf.haigaiapp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ah.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oh.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cw.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ps.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tf.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ht.jianghongdianzi.cn

[B03] switch / match / case
来源：http://yp.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tm.muxihuayi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mf.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bq.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ez.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gb.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kv.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uw.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mz.bookmarksfly.cn

[B04] for 计数循环
来源：http://th.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://so.521024.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ll.shxzukj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xv.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vc.yuexingan06.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fz.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ml.shxzukj.cn

Ruby: 10.times { |i| puts i }
来源：http://fv.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ns.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://um.colortex.cn

Py:   for item in arr: print(item)
来源：http://nz.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ac.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nv.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nu.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://df.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zn.szsharing.cn

Ruby: arr.each { |item| puts item }
来源：http://yg.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eq.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://ed.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pj.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tk.jianghongdianzi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://id.shxzskj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ve.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ux.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ty.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qh.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zg.yuexingan06.cn

[B07] while 循环
来源：http://cv.nicolike.cn

Py:   while i < 10: i += 1
来源：http://in.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kf.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://ty.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://iy.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://mm.gzmigu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ii.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://mz.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://wn.muxihuayi.cn

[B08] do-while（至少执行一次）
来源：http://ky.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://qo.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://hw.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://mm.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://yg.huixiangedu.cn

Java: do { i++; } while (i < 10);
来源：http://zp.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xn.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yq.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://qc.szxytkj.cn

[B09] break 与 continue
来源：http://kr.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pm.jianghongdianzi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lv.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fv.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jw.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gu.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vy.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://za.huixinmuqiang.cn


<!-- 参考信息 -->