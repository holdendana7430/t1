代发 wailian999

Ruby: 42.to_s
来源：http://bp.colortex.cn

C#:   42.ToString()
来源：http://gb.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://ki.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ux.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hk.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ad.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wq.szxytkj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xt.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rg.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://uy.huanxung.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tn.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://il.huixinmuqiang.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xo.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ur.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kz.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ux.newstarts.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lq.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sf.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qd.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wx.szxytkj.cn

[A10] 生成随机数
来源：http://je.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://lc.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://ee.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ad.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fc.521024.cn

Java: new Random().nextInt(100) + 1
来源：http://pa.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jo.jctech888.com.cn

Ruby: rand(1..100)
来源：http://ka.chemitech.net.cn

C#:   new Random().Next(1, 101)
来源：http://gc.szxytkj.cn

[A11] 条件表达式（三元）
来源：http://ab.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://cn.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bb.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bc.szsharing.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mh.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://iq.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ds.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qs.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fu.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://jk.panjiajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://se.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vs.yuexingan06.cn

JS:   `Hello, ${name}!`
来源：http://mj.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://to.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://iy.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gb.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://ef.9csxet.cn

C#:   $"Hello, {name}!"
来源：http://ud.muxihuayi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://nn.huanxung.cn

Py:   "第一行\n第二行"
来源：http://xo.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://ae.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://xc.szsharing.cn

TS:   "第一行\n第二行"
来源：http://zk.nicolike.cn

Java: "第一行\n第二行"
来源：http://qw.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://vu.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://tr.nszjky.cn

C#:   "第一行\n第二行"
来源：http://zc.gzmigu.cn

[A14] 注释写法
来源：http://xs.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ez.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dp.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://pm.bjjhwx.cn

TS:   // 单行；/* 多行 */
来源：http://ns.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ma.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://oa.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pa.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://us.lnxyls.cn

[A15] 空值判断与默认值
来源：http://zk.colortex.cn

Py:   value = data or "默认值"
来源：http://uh.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://nf.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://yq.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://ta.huixiangedu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sj.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://bi.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://tq.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://ly.szsharing.cn

[A16] 真假值判断规则
来源：http://bw.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jm.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ye.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tj.bjjhwx.cn

TS:   if (!x) {}
来源：http://gb.yuntaijiaju.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wm.chemitech.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hh.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://eg.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fb.muxihuayi.cn

[A17] 位运算
来源：http://pv.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zu.panjiajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lb.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://io.hahajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vi.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fd.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yu.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xj.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lc.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://cd.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://la.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://nm.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wb.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ym.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://wr.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nr.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://bw.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://vy.panjiajie.cn

[A19] 交换两个变量
来源：http://rw.huixiangedu.cn

Py:   a, b = b, a
来源：http://ex.521024.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gz.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://uo.gzmigu.cn

TS:   [a, b] = [b, a];
来源：http://py.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://so.yuexingan06.cn

Go:   a, b = b, a
来源：http://yj.huixiangedu.cn

Ruby: a, b = b, a
来源：http://fq.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://ey.newstarts.cn

[A20] 读取标准输入
来源：http://lx.shxzskj.cn

Py:   name = input("请输入：")
来源：http://bg.huanxung.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kj.bjjhwx.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://km.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://bv.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://zv.chemitech.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mu.yuntaijiaju.cn

Ruby: gets.chomp
来源：http://ij.szsharing.cn

C#:   Console.ReadLine();
来源：http://lv.shxzukj.cn

[A21] 保留指定小数位输出
来源：http://xx.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://ai.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xs.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://vj.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://dy.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://gq.szxytkj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zn.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://rl.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://xr.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://sn.wgjwhj.cn

Py:   len(s)
来源：http://pz.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://st.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sg.asd995.cn

TS:   s.length
来源：http://qn.chemitech.net.cn

Java: s.length()
来源：http://zs.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://up.yuexingan06.cn

Ruby: s.length
来源：http://wh.jianghongdianzi.cn

C#:   s.Length
来源：http://dl.shxzskj.cn

[A23] 大小写转换
来源：http://co.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://om.521024.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://by.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ah.521024.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://on.yuntaijiaju.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ay.huixiangedu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://on.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ku.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://iy.shxzukj.cn

[A24] 去除首尾空白
来源：http://bf.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ds.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rl.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wg.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://en.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://th.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://lr.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pz.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aw.lnxyls.cn

[A25] 字符串比较
来源：http://hy.szsharing.cn

Py:   s1 == s2; s1 != s2
来源：http://ye.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://al.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rh.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mw.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cc.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zs.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rc.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bp.shxzskj.cn

[A26] 类型转换总览
来源：http://up.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mz.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uc.haigaiapp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nl.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://zt.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lk.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qr.hahajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uy.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jq.hahajie.cn

================================================================================
来源：http://mq.hahajie.cn

B. 流程控制
来源：http://cu.gzmigu.cn

================================================================================
来源：http://jq.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://pb.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nf.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xq.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://te.gzmigu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dy.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://py.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fq.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tt.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pp.9csxet.cn

[B02] 多分支 else if / elif
来源：http://at.9csxet.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ax.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dt.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lm.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://va.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gs.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zz.bjjhwx.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ys.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sq.asd995.cn

[B03] switch / match / case
来源：http://ne.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kp.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wh.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jw.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lm.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://af.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sa.panjiajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wo.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qc.gzmigu.cn

[B04] for 计数循环
来源：http://gl.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://gh.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zu.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ka.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lb.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://je.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ng.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://ec.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dl.lnxyls.cn

[B05] 遍历数组 / 列表
来源：http://hr.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://dd.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wf.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hj.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uk.haigaiapp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rl.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://li.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://yq.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fo.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://vr.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mh.hnjuh.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zq.nicolike.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kb.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lh.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ls.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://um.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vz.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bk.yuexingan06.cn

[B07] while 循环
来源：http://gd.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://uv.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fv.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://vn.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://tx.asd995.cn

Java: while (i < 10) { i++; }
来源：http://ae.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yq.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://ms.shtwfgs.cn

C#:   while (i < 10) { i++; }
来源：http://pk.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://vy.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://pa.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rt.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://ox.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://by.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://dx.panjiajie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jy.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kv.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://ke.jianghongdianzi.cn

[B09] break 与 continue
来源：http://db.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lz.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bj.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vt.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nd.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oy.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dh.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nh.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ri.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://vf.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sq.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tr.colortex.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xr.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://in.colortex.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rg.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uh.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://da.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ij.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://zn.9csxet.cn

Py:   list(range(0, 10, 2))
来源：http://ra.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://kh.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jd.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jz.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nz.9csxet.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tx.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://yl.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uu.haigaiapp.cn

[B12] 跳出多层循环
来源：http://oy.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://it.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://by.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hp.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lw.newstarts.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ek.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sg.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mw.nszjky.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bg.shxzskj.cn

[B13] 判断是否为数字
来源：http://bv.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://zl.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://as.gzmigu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ya.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sa.szsharing.cn

Java: x instanceof Number
来源：http://xm.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kd.gzmigu.cn

Ruby: x.is_a?(Numeric)
来源：http://wv.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://ji.nszjky.cn

[B14] 判断值是否在集合内
来源：http://cn.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ei.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jh.shxzskj.cn

JS:   [1, 2, 3].includes(x)
来源：http://ud.huixinmuqiang.cn

TS:   [1, 2, 3].includes(x)
来源：http://yg.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://br.shxzskj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dn.yuntaijiaju.cn


<!-- 参考信息 -->