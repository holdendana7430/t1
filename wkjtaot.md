代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mc.szsharing.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wb.bookmarksfly.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ai.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tl.huanxung.cn

Java: 7 / 2; 7 % 2
来源：http://do.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://xf.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://xq.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://sd.hahajie.cn

[A06] 字符串转数字
来源：http://mz.521024.cn

Py:   int("42"); float("3.14")
来源：http://sl.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nr.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uf.huanxung.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ws.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mn.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ky.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hh.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zi.asd995.cn

[A07] 数字转字符串
来源：http://rb.szxytkj.cn

Py:   str(42)
来源：http://dj.jianghongdianzi.cn

PHP:  (string) 42; strval(42)
来源：http://zm.9csxet.cn

JS:   String(42); (42).toString()
来源：http://dw.chemitech.net.cn

TS:   String(42)
来源：http://nm.nicolike.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://la.nszjky.cn

Go:   strconv.Itoa(42)
来源：http://wp.szsharing.cn

Ruby: 42.to_s
来源：http://bh.huixiangedu.cn

C#:   42.ToString()
来源：http://gr.haigaiapp.cn

[A08] 取整与四舍五入
来源：http://tu.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vp.yuexingan06.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wr.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://px.shxzskj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yu.wgjwhj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qa.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ec.bjjhwx.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://kh.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fh.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://vo.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vo.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rw.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rj.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jy.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zs.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ns.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ac.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ke.wgjwhj.cn

[A10] 生成随机数
来源：http://jh.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://nv.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://te.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xt.shxzukj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fm.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://uy.muxihuayi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ch.shtwfgs.cn

Ruby: rand(1..100)
来源：http://tj.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://lf.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://uf.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://du.colortex.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bh.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fx.huixiangedu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://za.yuexingan06.cn

Java: x > 0 ? "yes" : "no"
来源：http://ks.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://qc.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rq.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ap.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://uq.yuntaijiaju.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ae.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yg.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://lg.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://yu.panjiajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://jz.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cj.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://bn.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://tg.huixiangedu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mb.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://mi.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://yz.nszjky.cn

JS:   "第一行\n第二行"
来源：http://hq.szsharing.cn

TS:   "第一行\n第二行"
来源：http://vs.nszjky.cn

Java: "第一行\n第二行"
来源：http://fe.nicolike.cn

Go:   "第一行\n第二行"
来源：http://ke.yuexingan06.cn

Ruby: "第一行\n第二行"
来源：http://qe.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://ge.shtwfgs.cn

[A14] 注释写法
来源：http://pb.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fk.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jo.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://aa.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://no.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pi.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://ci.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://si.521024.cn

C#:   // 单行；/* 多行 */
来源：http://ad.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://rx.newstarts.cn

Py:   value = data or "默认值"
来源：http://rq.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://fc.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://md.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://ka.huixiangedu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fn.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://pm.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://sq.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://hn.shxzukj.cn

[A16] 真假值判断规则
来源：http://ut.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oa.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gy.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ts.bookmarksfly.cn

TS:   if (!x) {}
来源：http://jb.nszjky.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jz.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hr.jctech888.com.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nv.shxzukj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qq.panjiajie.cn

[A17] 位运算
来源：http://tp.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ud.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dv.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cd.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rf.chemitech.net.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ly.lnxyls.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rk.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sk.chemitech.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lb.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://ll.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://pm.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://ks.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xd.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://km.hnjuh.cn

Java: (int) 'A'; (char) 65
来源：http://id.huixiangedu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qx.panjiajie.cn

Ruby: "A".ord; 65.chr
来源：http://rv.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://yv.colortex.cn

[A19] 交换两个变量
来源：http://yc.shxzskj.cn

Py:   a, b = b, a
来源：http://gl.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lv.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://ln.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://ct.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://mn.521024.cn

Go:   a, b = b, a
来源：http://ld.gzmigu.cn

Ruby: a, b = b, a
来源：http://ii.huixiangedu.cn

C#:   (a, b) = (b, a);
来源：http://ks.nicolike.cn

[A20] 读取标准输入
来源：http://eq.haigaiapp.cn

Py:   name = input("请输入：")
来源：http://kk.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xv.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cu.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://zi.wgjwhj.cn

Java: new Scanner(System.in).nextLine()
来源：http://kp.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vk.wgjwhj.cn

Ruby: gets.chomp
来源：http://cp.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://fy.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://vi.asd995.cn

Py:   f"{3.14159:.2f}"
来源：http://zh.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://aw.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://di.szxytkj.cn

TS:   (3.14159).toFixed(2)
来源：http://ef.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://vn.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://am.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://qf.gzmigu.cn

C#:   3.14159.ToString("F2")
来源：http://ls.haigaiapp.cn

[A22] 获取字符串长度
来源：http://pz.szsharing.cn

Py:   len(s)
来源：http://ew.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wd.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ln.huixinmuqiang.cn

TS:   s.length
来源：http://ta.newstarts.cn

Java: s.length()
来源：http://mq.newstarts.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://st.hnjuh.cn

Ruby: s.length
来源：http://lm.hnjuh.cn

C#:   s.Length
来源：http://wk.bookmarksfly.cn

[A23] 大小写转换
来源：http://ru.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qm.nicolike.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wm.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xa.hahajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dd.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eb.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vj.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ko.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gp.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://uq.yuexingan06.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ze.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ci.nszjky.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://og.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://li.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qw.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://ws.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ah.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://el.chemitech.net.cn

[A25] 字符串比较
来源：http://nv.9csxet.cn

Py:   s1 == s2; s1 != s2
来源：http://ux.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ju.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dp.szxytkj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fx.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fj.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zo.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tt.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kk.lnxyls.cn

[A26] 类型转换总览
来源：http://rb.asd995.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yy.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hw.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fl.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://rl.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ik.colortex.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xs.yuexingan06.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pp.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.panjiajie.cn

================================================================================
来源：http://mn.huixiangedu.cn

B. 流程控制
来源：http://yk.jctech888.com.cn

================================================================================
来源：http://bh.huanxung.cn

[B01] 条件判断 if / else
来源：http://bl.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fe.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qi.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ff.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jx.bjjhwx.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ot.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ll.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yh.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qu.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://hc.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eq.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wi.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jg.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gc.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nz.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rv.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jj.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wt.szsharing.cn

[B03] switch / match / case
来源：http://ov.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fc.shtwfgs.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://je.9csxet.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ub.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pq.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xe.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hb.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rb.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nk.chemitech.net.cn

[B04] for 计数循环
来源：http://df.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://qv.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pq.huixiangedu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ak.muxihuayi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ho.hahajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wy.newstarts.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ov.hahajie.cn

Ruby: 10.times { |i| puts i }
来源：http://to.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xi.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://cm.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://ui.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ty.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xd.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gi.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zw.chemitech.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lw.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://ds.shtwfgs.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vj.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://kj.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mf.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pq.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tj.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://th.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://id.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ps.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sd.haigaiapp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vv.newstarts.cn

[B07] while 循环
来源：http://dx.9csxet.cn

Py:   while i < 10: i += 1
来源：http://hb.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wh.gzmigu.cn

JS:   while (i < 10) { i++; }
来源：http://gr.szsharing.cn

TS:   while (i < 10) { i++; }
来源：http://ja.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://fl.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://he.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://wr.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://tj.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://wh.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://zn.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bh.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://nv.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://lb.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://xp.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ax.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kc.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://fo.bookmarksfly.cn

[B09] break 与 continue
来源：http://ux.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cl.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mc.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ua.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vu.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sc.521024.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qq.colortex.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ue.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qr.asd995.cn

[B10] 遍历同时拿索引
来源：http://hz.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zj.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mw.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://og.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sv.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bu.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://da.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wo.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sd.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://sn.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://cv.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://oh.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://di.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ce.panjiajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hd.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jk.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://br.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gj.bjjhwx.cn

[B12] 跳出多层循环
来源：http://ii.nicolike.cn


<!-- 参考信息 -->