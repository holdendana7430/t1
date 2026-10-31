代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://tw.chemitech.net.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ip.asd995.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://af.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lj.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cr.haigaiapp.cn

[A07] 数字转字符串
来源：http://xt.szxytkj.cn

Py:   str(42)
来源：http://iu.jctech888.com.cn

PHP:  (string) 42; strval(42)
来源：http://tf.huixinmuqiang.cn

JS:   String(42); (42).toString()
来源：http://qg.nicolike.cn

TS:   String(42)
来源：http://ss.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vb.yuntaijiaju.cn

Go:   strconv.Itoa(42)
来源：http://bd.jctech888.com.cn

Ruby: 42.to_s
来源：http://ch.jctech888.com.cn

C#:   42.ToString()
来源：http://da.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://gp.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bj.jianghongdianzi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ud.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mk.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fj.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ao.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://va.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rf.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jh.asd995.cn

[A09] 绝对值与最大最小值
来源：http://pj.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cy.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mn.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://np.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dm.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xy.bjjhwx.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xg.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fl.panjiajie.cn

[A10] 生成随机数
来源：http://dq.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://lv.yuntaijiaju.cn

PHP:  random_int(1, 100);
来源：http://se.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ox.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jd.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://zw.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yg.lnxyls.cn

Ruby: rand(1..100)
来源：http://vh.hnjuh.cn

C#:   new Random().Next(1, 101)
来源：http://td.hahajie.cn

[A11] 条件表达式（三元）
来源：http://ii.chemitech.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://xw.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lq.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kn.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kt.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://qe.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ef.jianghongdianzi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mg.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zh.asd995.cn

[A12] 字符串插值 / 格式化
来源：http://ua.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://it.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://af.bookmarksfly.cn

JS:   `Hello, ${name}!`
来源：http://iq.colortex.cn

TS:   `Hello, ${name}!`
来源：http://bm.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://yy.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kk.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://ar.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://qw.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gh.szxytkj.cn

Py:   "第一行\n第二行"
来源：http://bp.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://kk.muxihuayi.cn

JS:   "第一行\n第二行"
来源：http://tf.jianghongdianzi.cn

TS:   "第一行\n第二行"
来源：http://dp.asd995.cn

Java: "第一行\n第二行"
来源：http://za.panjiajie.cn

Go:   "第一行\n第二行"
来源：http://hf.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://hu.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://lg.9csxet.cn

[A14] 注释写法
来源：http://vp.szsharing.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zq.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dy.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://xm.chemitech.net.cn

TS:   // 单行；/* 多行 */
来源：http://qv.huixinmuqiang.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qr.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://hs.hahajie.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uk.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://ef.bjjhwx.cn

[A15] 空值判断与默认值
来源：http://ai.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://pj.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://qj.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://du.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://sj.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ru.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://he.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://yt.shtwfgs.cn

C#:   var value = data ?? "默认值";
来源：http://yl.521024.cn

[A16] 真假值判断规则
来源：http://bx.huixiangedu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xc.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zs.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yf.szsharing.cn

TS:   if (!x) {}
来源：http://pk.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bx.nicolike.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xg.hahajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hf.newstarts.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cw.colortex.cn

[A17] 位运算
来源：http://nw.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dj.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nt.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cv.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dl.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bx.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bk.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sg.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cd.bjjhwx.cn

[A18] 字符与 ASCII 码互转
来源：http://bh.521024.cn

Py:   ord("A"); chr(65)
来源：http://ap.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://jp.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kt.shxzukj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pt.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://wk.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tg.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://rm.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://qu.hahajie.cn

[A19] 交换两个变量
来源：http://yv.asd995.cn

Py:   a, b = b, a
来源：http://un.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nu.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://df.nicolike.cn

TS:   [a, b] = [b, a];
来源：http://xs.panjiajie.cn

Java: int t = a; a = b; b = t;
来源：http://rg.huixiangedu.cn

Go:   a, b = b, a
来源：http://kq.521024.cn

Ruby: a, b = b, a
来源：http://za.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://ok.bjjhwx.cn

[A20] 读取标准输入
来源：http://ml.bjjhwx.cn

Py:   name = input("请输入：")
来源：http://as.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hr.chemitech.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cg.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://yk.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://wg.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gq.muxihuayi.cn

Ruby: gets.chomp
来源：http://zq.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://dz.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://qp.chemitech.net.cn

Py:   f"{3.14159:.2f}"
来源：http://wy.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zj.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://nc.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://zh.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://lo.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ir.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://ok.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://vw.9csxet.cn

[A22] 获取字符串长度
来源：http://qo.asd995.cn

Py:   len(s)
来源：http://tr.yuntaijiaju.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mq.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ly.newstarts.cn

TS:   s.length
来源：http://bq.panjiajie.cn

Java: s.length()
来源：http://rp.szxytkj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cg.bookmarksfly.cn

Ruby: s.length
来源：http://hz.lnxyls.cn

C#:   s.Length
来源：http://ms.gzmigu.cn

[A23] 大小写转换
来源：http://de.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://we.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ls.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rx.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mz.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bt.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mf.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://aq.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gi.haigaiapp.cn

[A24] 去除首尾空白
来源：http://do.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://be.shxzukj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tl.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zk.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zp.colortex.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sd.asd995.cn

Go:   strings.TrimSpace(s)
来源：http://sv.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tm.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yv.521024.cn

[A25] 字符串比较
来源：http://mj.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://tb.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sy.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://li.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ez.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yc.yuntaijiaju.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nn.huixiangedu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ev.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lg.shtwfgs.cn

[A26] 类型转换总览
来源：http://ut.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kz.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zk.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xa.asd995.cn

TS:   Number() String() Boolean() x as number
来源：http://xa.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fm.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pg.gzmigu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yn.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nj.hnjuh.cn

================================================================================
来源：http://mr.wgjwhj.cn

B. 流程控制
来源：http://ro.9csxet.cn

================================================================================
来源：http://el.szsharing.cn

[B01] 条件判断 if / else
来源：http://ow.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tg.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ia.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vp.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bi.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://mj.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jt.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ya.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tj.wgjwhj.cn

[B02] 多分支 else if / elif
来源：http://ov.hnjuh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://or.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uc.yuntaijiaju.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fd.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ku.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ue.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fn.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mv.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ya.jctech888.com.cn

[B03] switch / match / case
来源：http://tt.huixiangedu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ec.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sq.wgjwhj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rw.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iz.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dy.chemitech.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gl.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cw.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fl.9csxet.cn

[B04] for 计数循环
来源：http://oo.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://lt.nszjky.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pf.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jc.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gw.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fv.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cb.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://dj.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pz.huanxung.cn

[B05] 遍历数组 / 列表
来源：http://dj.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://vd.huixinmuqiang.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zv.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mu.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ku.gzmigu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pn.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gp.nszjky.cn

Ruby: arr.each { |item| puts item }
来源：http://eh.newstarts.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qm.szxytkj.cn

[B06] 遍历字典 / 对象
来源：http://xy.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gs.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vc.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lh.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dn.shxzukj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qw.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vr.shxzukj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yr.shtwfgs.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nl.shtwfgs.cn

[B07] while 循环
来源：http://lo.nszjky.cn

Py:   while i < 10: i += 1
来源：http://bf.shtwfgs.cn

PHP:  while ($i < 10) { $i++; }
来源：http://la.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://ib.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://dv.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://fm.bookmarksfly.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tc.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://li.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://vg.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://cd.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://xh.shtwfgs.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kv.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://tt.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://jn.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://et.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dv.bjjhwx.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tq.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://pr.wgjwhj.cn

[B09] break 与 continue
来源：http://gz.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cy.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vw.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bj.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ce.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gj.huixinmuqiang.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rt.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xf.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fz.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://jc.shtwfgs.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xo.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ih.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zf.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jb.gzmigu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kw.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sa.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aq.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xz.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://ka.shxzskj.cn

Py:   list(range(0, 10, 2))
来源：http://rn.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://qk.shtwfgs.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zx.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ul.jianghongdianzi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tj.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iv.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://kz.bookmarksfly.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yd.newstarts.cn

[B12] 跳出多层循环
来源：http://mi.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://li.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xv.shxzukj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://co.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uj.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wf.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ga.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jy.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ze.jctech888.com.cn

[B13] 判断是否为数字
来源：http://ll.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://ok.shtwfgs.cn

PHP:  is_numeric($x)
来源：http://df.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ys.chemitech.net.cn


<!-- 参考信息 -->