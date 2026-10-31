代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pa.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ny.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fo.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://qs.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cd.gzmigu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zz.huanxung.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pp.9csxet.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://np.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ib.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ts.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yg.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://do.panjiajie.cn

[A10] 生成随机数
来源：http://aw.lnxyls.cn

Py:   import random; random.randint(1, 100)
来源：http://fq.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://dn.szxytkj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jg.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nr.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://wo.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dz.nicolike.cn

Ruby: rand(1..100)
来源：http://hs.nicolike.cn

C#:   new Random().Next(1, 101)
来源：http://sz.muxihuayi.cn

[A11] 条件表达式（三元）
来源：http://dy.huixinmuqiang.cn

Py:   "yes" if x > 0 else "no"
来源：http://bx.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kc.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fo.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ah.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://dg.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://iq.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qm.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xz.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://zf.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pm.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ku.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://if.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://wp.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://xt.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yg.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://lo.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://ps.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qp.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://bj.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://af.newstarts.cn

JS:   "第一行\n第二行"
来源：http://je.asd995.cn

TS:   "第一行\n第二行"
来源：http://tq.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://gc.521024.cn

Go:   "第一行\n第二行"
来源：http://nr.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://od.panjiajie.cn

C#:   "第一行\n第二行"
来源：http://no.chemitech.net.cn

[A14] 注释写法
来源：http://ek.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bw.chemitech.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wb.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://ca.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://vi.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nd.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://yt.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vo.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://tq.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://en.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://ex.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://aw.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://ce.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://rp.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ym.haigaiapp.cn

Go:   if data == "" { data = "默认值" }
来源：http://nz.bjjhwx.cn

Ruby: value = data || "默认值"
来源：http://ar.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://hf.huanxung.cn

[A16] 真假值判断规则
来源：http://yh.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xu.yuexingan06.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bw.9csxet.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ea.colortex.cn

TS:   if (!x) {}
来源：http://ic.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ek.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nd.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ab.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ny.wgjwhj.cn

[A17] 位运算
来源：http://us.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pl.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ii.nicolike.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ao.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kz.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hb.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tq.jctech888.com.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wv.jctech888.com.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sf.bookmarksfly.cn

[A18] 字符与 ASCII 码互转
来源：http://zr.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://ye.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://qu.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hk.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://se.521024.cn

Java: (int) 'A'; (char) 65
来源：http://ay.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fw.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://ls.shtwfgs.cn

C#:   (int)'A'; (char)65
来源：http://cn.521024.cn

[A19] 交换两个变量
来源：http://tn.szxytkj.cn

Py:   a, b = b, a
来源：http://uv.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://se.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://kg.colortex.cn

TS:   [a, b] = [b, a];
来源：http://ro.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://qo.yuexingan06.cn

Go:   a, b = b, a
来源：http://bw.hahajie.cn

Ruby: a, b = b, a
来源：http://ws.colortex.cn

C#:   (a, b) = (b, a);
来源：http://ai.chemitech.net.cn

[A20] 读取标准输入
来源：http://fu.newstarts.cn

Py:   name = input("请输入：")
来源：http://bd.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ce.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ih.huanxung.cn

TS:   // Node.js：readline 模块
来源：http://ad.newstarts.cn

Java: new Scanner(System.in).nextLine()
来源：http://xb.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nd.muxihuayi.cn

Ruby: gets.chomp
来源：http://ym.huanxung.cn

C#:   Console.ReadLine();
来源：http://nh.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://za.521024.cn

Py:   f"{3.14159:.2f}"
来源：http://tc.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dq.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://ye.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://as.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://rb.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://te.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://tw.9csxet.cn

C#:   3.14159.ToString("F2")
来源：http://ub.szxytkj.cn

[A22] 获取字符串长度
来源：http://jn.jianghongdianzi.cn

Py:   len(s)
来源：http://nt.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vx.szsharing.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nc.haigaiapp.cn

TS:   s.length
来源：http://cy.shxzskj.cn

Java: s.length()
来源：http://sv.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qn.yuntaijiaju.cn

Ruby: s.length
来源：http://gl.yuexingan06.cn

C#:   s.Length
来源：http://hd.szsharing.cn

[A23] 大小写转换
来源：http://sd.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nh.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dm.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://un.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kb.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oh.szsharing.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xv.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://px.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ip.wgjwhj.cn

[A24] 去除首尾空白
来源：http://wl.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jv.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fp.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nr.shxzukj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ax.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wf.yuexingan06.cn

Go:   strings.TrimSpace(s)
来源：http://od.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bz.nicolike.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ww.huanxung.cn

[A25] 字符串比较
来源：http://ey.huixiangedu.cn

Py:   s1 == s2; s1 != s2
来源：http://qw.nszjky.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mv.shxzukj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://be.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wk.szxytkj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ib.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ev.chemitech.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vd.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kd.haigaiapp.cn

[A26] 类型转换总览
来源：http://jo.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mc.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ti.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bi.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://kj.wgjwhj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hp.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jl.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ch.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oj.huixiangedu.cn

================================================================================
来源：http://fv.yuntaijiaju.cn

B. 流程控制
来源：http://zb.szxytkj.cn

================================================================================
来源：http://ua.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://hh.nszjky.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ez.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ee.wgjwhj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fi.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zt.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hg.nszjky.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sn.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fc.yuexingan06.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://no.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://qo.yuexingan06.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zs.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ro.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rz.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cq.nszjky.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sc.huanxung.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gq.bookmarksfly.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vn.bookmarksfly.cn

[B03] switch / match / case
来源：http://bz.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vi.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ov.shxzukj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://js.panjiajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cd.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sa.huixiangedu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dp.nicolike.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pt.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jj.hahajie.cn

[B04] for 计数循环
来源：http://gu.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://gs.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ps.shxzskj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zj.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xm.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://au.nszjky.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vk.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://nn.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ub.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://eb.asd995.cn

Py:   for item in arr: print(item)
来源：http://rs.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tt.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jk.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gy.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nt.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tk.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://nm.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vo.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://oy.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jl.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ao.lnxyls.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nk.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://km.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vb.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dr.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gh.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wb.jctech888.com.cn

[B07] while 循环
来源：http://if.9csxet.cn

Py:   while i < 10: i += 1
来源：http://pk.haigaiapp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hw.shtwfgs.cn

JS:   while (i < 10) { i++; }
来源：http://mu.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://bo.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://vk.shtwfgs.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bs.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://zr.hahajie.cn

C#:   while (i < 10) { i++; }
来源：http://pi.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://sw.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://du.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yo.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://go.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://pc.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://ij.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fs.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hm.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://fm.szsharing.cn

[B09] break 与 continue
来源：http://qm.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lp.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kj.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ec.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://im.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ff.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nq.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ul.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uv.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://yl.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://in.wgjwhj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kg.bookmarksfly.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yh.521024.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://od.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zn.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sy.haigaiapp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ck.yuexingan06.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pr.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://nk.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://ip.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://xq.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vg.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rk.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jy.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ih.chemitech.net.cn

Ruby: (0...10).step(2).to_a
来源：http://uv.panjiajie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zv.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://dl.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qe.huanxung.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lu.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jm.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://og.chemitech.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qu.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ek.bookmarksfly.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://my.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zx.jctech888.com.cn

[B13] 判断是否为数字
来源：http://mz.521024.cn

Py:   isinstance(x, (int, float))
来源：http://lw.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://bz.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ud.haigaiapp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://su.szsharing.cn

Java: x instanceof Number
来源：http://ow.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gp.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://ob.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://zr.colortex.cn

[B14] 判断值是否在集合内
来源：http://gl.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wk.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ed.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://pc.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://ue.newstarts.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dv.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ii.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wc.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tz.colortex.cn

[B15] 布尔运算与取反
来源：http://jq.shxzskj.cn

Py:   a and b or not c
来源：http://cm.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://rj.hnjuh.cn

JS:   a && b || !c
来源：http://jw.521024.cn

TS:   a && b || !c
来源：http://yl.hahajie.cn

Java: a && b || !c
来源：http://cj.jianghongdianzi.cn


<!-- 参考信息 -->