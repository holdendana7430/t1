代发 wailian999

Java: 7 / 2; 7 % 2
来源：http://jc.521024.cn

Go:   7 / 2; 7 % 2
来源：http://qm.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://ov.gzmigu.cn

C#:   7 / 2; 7 % 2
来源：http://mw.chemitech.net.cn

[A06] 字符串转数字
来源：http://uf.hahajie.cn

Py:   int("42"); float("3.14")
来源：http://if.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ug.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://uh.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pd.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qy.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qk.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wc.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hu.huanxung.cn

[A07] 数字转字符串
来源：http://wg.yuexingan06.cn

Py:   str(42)
来源：http://ai.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://nn.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://dp.szsharing.cn

TS:   String(42)
来源：http://xs.haigaiapp.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ue.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://kr.bjjhwx.cn

Ruby: 42.to_s
来源：http://ap.lnxyls.cn

C#:   42.ToString()
来源：http://yh.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://hq.muxihuayi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ew.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jk.chemitech.net.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jh.muxihuayi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hq.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gd.panjiajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jf.shxzskj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fr.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cc.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://wl.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yc.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ki.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://iz.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ub.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xn.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yn.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cp.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lp.shxzukj.cn

[A10] 生成随机数
来源：http://ko.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://yq.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://rs.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://av.521024.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yz.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://kv.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mo.shxzukj.cn

Ruby: rand(1..100)
来源：http://qu.521024.cn

C#:   new Random().Next(1, 101)
来源：http://yz.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://ay.yuexingan06.cn

Py:   "yes" if x > 0 else "no"
来源：http://oj.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kh.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://af.haigaiapp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sb.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://bf.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tx.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://be.hnjuh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uf.521024.cn

[A12] 字符串插值 / 格式化
来源：http://at.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kc.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rm.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://ev.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://hi.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://co.bjjhwx.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hq.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://lj.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://hn.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wh.9csxet.cn

Py:   "第一行\n第二行"
来源：http://rd.521024.cn

PHP:  "第一行\n第二行"
来源：http://fn.9csxet.cn

JS:   "第一行\n第二行"
来源：http://pr.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://fv.szxytkj.cn

Java: "第一行\n第二行"
来源：http://wt.shtwfgs.cn

Go:   "第一行\n第二行"
来源：http://sk.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://vi.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://wf.colortex.cn

[A14] 注释写法
来源：http://ve.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://am.nszjky.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pp.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://bg.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://iq.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vz.asd995.cn

Go:   // 单行；/* 多行 */
来源：http://ib.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rd.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://eo.colortex.cn

[A15] 空值判断与默认值
来源：http://ve.9csxet.cn

Py:   value = data or "默认值"
来源：http://do.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://pk.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://ph.chemitech.net.cn

TS:   const value = data ?? "默认值";
来源：http://qi.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jp.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://ek.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://tc.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://gr.shxzukj.cn

[A16] 真假值判断规则
来源：http://go.jctech888.com.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://at.szxytkj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ei.hahajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rg.huixiangedu.cn

TS:   if (!x) {}
来源：http://ss.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jg.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fx.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uk.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rr.nicolike.cn

[A17] 位运算
来源：http://id.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dn.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fn.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://au.nszjky.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rx.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fy.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oz.szsharing.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fr.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qf.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://ma.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://el.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://by.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qu.shxzukj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ip.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://zt.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cl.huanxung.cn

Ruby: "A".ord; 65.chr
来源：http://vw.szxytkj.cn

C#:   (int)'A'; (char)65
来源：http://tz.lnxyls.cn

[A19] 交换两个变量
来源：http://gh.szxytkj.cn

Py:   a, b = b, a
来源：http://mk.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gy.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://ys.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://rx.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://wf.gzmigu.cn

Go:   a, b = b, a
来源：http://jh.asd995.cn

Ruby: a, b = b, a
来源：http://vi.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://tg.bookmarksfly.cn

[A20] 读取标准输入
来源：http://li.hnjuh.cn

Py:   name = input("请输入：")
来源：http://cv.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kt.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tn.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://ij.huixiangedu.cn

Java: new Scanner(System.in).nextLine()
来源：http://xd.yuexingan06.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hh.asd995.cn

Ruby: gets.chomp
来源：http://ky.bjjhwx.cn

C#:   Console.ReadLine();
来源：http://ze.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://yd.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://tk.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wu.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://ps.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://xk.bookmarksfly.cn

Java: String.format("%.2f", 3.14159)
来源：http://gb.newstarts.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ih.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://dw.nicolike.cn

C#:   3.14159.ToString("F2")
来源：http://mu.szsharing.cn

[A22] 获取字符串长度
来源：http://qu.huanxung.cn

Py:   len(s)
来源：http://hg.jctech888.com.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tv.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gv.yuexingan06.cn

TS:   s.length
来源：http://mh.gzmigu.cn

Java: s.length()
来源：http://yp.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qf.hahajie.cn

Ruby: s.length
来源：http://wj.szxytkj.cn

C#:   s.Length
来源：http://wy.shxzskj.cn

[A23] 大小写转换
来源：http://il.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lz.shtwfgs.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gg.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mm.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yy.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mw.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vb.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uy.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fn.shxzukj.cn

[A24] 去除首尾空白
来源：http://jo.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mk.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ko.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://os.muxihuayi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aw.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xb.muxihuayi.cn

Go:   strings.TrimSpace(s)
来源：http://yv.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://to.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://es.nicolike.cn

[A25] 字符串比较
来源：http://us.muxihuayi.cn

Py:   s1 == s2; s1 != s2
来源：http://hf.huixiangedu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nc.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uz.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tt.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://br.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jb.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oj.szsharing.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sa.colortex.cn

[A26] 类型转换总览
来源：http://it.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://so.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vs.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xw.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://zp.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ul.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://te.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gg.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ec.colortex.cn

================================================================================
来源：http://bn.hahajie.cn

B. 流程控制
来源：http://tl.wgjwhj.cn

================================================================================
来源：http://ks.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://kf.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oi.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cx.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ct.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lh.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ae.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fa.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ld.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jk.jianghongdianzi.cn

[B02] 多分支 else if / elif
来源：http://hr.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fl.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rz.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yg.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mi.hnjuh.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vl.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ao.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://os.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oa.muxihuayi.cn

[B03] switch / match / case
来源：http://ck.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cf.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://se.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bo.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vr.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dr.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lk.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lb.yuntaijiaju.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ag.nszjky.cn

[B04] for 计数循环
来源：http://bk.yuntaijiaju.cn

Py:   for i in range(10): print(i)
来源：http://xf.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nb.haigaiapp.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fw.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wv.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xy.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ye.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://xg.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ov.jctech888.com.cn

[B05] 遍历数组 / 列表
来源：http://ns.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://cb.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://au.colortex.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://of.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://su.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://en.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fm.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://sp.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ug.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://cx.wgjwhj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fb.shtwfgs.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kp.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gg.asd995.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cb.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qm.bjjhwx.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wh.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zd.huanxung.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bm.wgjwhj.cn

[B07] while 循环
来源：http://xz.521024.cn

Py:   while i < 10: i += 1
来源：http://ee.9csxet.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dm.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://mm.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://aw.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://wu.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oi.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://mc.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://dx.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://xj.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://ah.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uf.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://lu.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://or.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://cn.nszjky.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mi.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kf.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://pd.shxzukj.cn

[B09] break 与 continue
来源：http://vd.panjiajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rt.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dn.shxzukj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nw.521024.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nx.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hp.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qi.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jn.yuntaijiaju.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ek.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://vx.9csxet.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://db.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lz.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bk.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rj.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ev.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wf.nszjky.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mg.szsharing.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ou.nszjky.cn

[B11] 生成数字序列 / 区间
来源：http://la.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://zs.bookmarksfly.cn

PHP:  range(0, 10, 2);
来源：http://mx.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://op.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nt.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tl.huanxung.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rx.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://ny.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ha.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://hr.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mr.shxzskj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bf.lnxyls.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vy.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uc.chemitech.net.cn


<!-- 参考信息 -->