代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ws.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://av.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xy.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://lg.panjiajie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wa.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zn.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xw.asd995.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mr.bookmarksfly.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wy.chemitech.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vc.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ry.nszjky.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gr.haigaiapp.cn

[A10] 生成随机数
来源：http://wo.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://ep.nszjky.cn

PHP:  random_int(1, 100);
来源：http://vk.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dd.bookmarksfly.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ez.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://sw.shxzukj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lr.huixiangedu.cn

Ruby: rand(1..100)
来源：http://gk.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://qn.lnxyls.cn

[A11] 条件表达式（三元）
来源：http://jr.haigaiapp.cn

Py:   "yes" if x > 0 else "no"
来源：http://fq.wgjwhj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jb.haigaiapp.cn

JS:   x > 0 ? "yes" : "no"
来源：http://se.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vl.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://ao.shxzukj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dd.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://el.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wv.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://io.chemitech.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ol.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qr.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://av.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://mv.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://az.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hn.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://cm.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://sp.bjjhwx.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ge.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://ca.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://jr.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://ac.gzmigu.cn

TS:   "第一行\n第二行"
来源：http://ya.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://ay.panjiajie.cn

Go:   "第一行\n第二行"
来源：http://cg.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://dm.nszjky.cn

C#:   "第一行\n第二行"
来源：http://qz.hnjuh.cn

[A14] 注释写法
来源：http://hy.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://js.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mh.newstarts.cn

JS:   // 单行；/* 多行 */
来源：http://sr.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://vj.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pu.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://tz.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vq.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://oj.yuexingan06.cn

[A15] 空值判断与默认值
来源：http://fu.shxzskj.cn

Py:   value = data or "默认值"
来源：http://go.nszjky.cn

PHP:  $value = $data ?? "默认值";
来源：http://sm.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://ln.shxzskj.cn

TS:   const value = data ?? "默认值";
来源：http://xx.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zu.muxihuayi.cn

Go:   if data == "" { data = "默认值" }
来源：http://mn.huanxung.cn

Ruby: value = data || "默认值"
来源：http://ss.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://ts.szsharing.cn

[A16] 真假值判断规则
来源：http://ou.huixinmuqiang.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fa.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cp.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xf.nszjky.cn

TS:   if (!x) {}
来源：http://wd.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pr.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gc.huixiangedu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jl.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sh.521024.cn

[A17] 位运算
来源：http://pq.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tx.huanxung.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wk.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ib.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yq.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tq.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zd.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ut.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://me.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://jr.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://ct.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://rn.hnjuh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ue.wgjwhj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ff.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://wh.muxihuayi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uk.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://nr.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://sq.shxzukj.cn

[A19] 交换两个变量
来源：http://ir.lnxyls.cn

Py:   a, b = b, a
来源：http://xv.newstarts.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vc.huixiangedu.cn

JS:   [a, b] = [b, a];
来源：http://bo.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://oy.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://jk.muxihuayi.cn

Go:   a, b = b, a
来源：http://uh.nszjky.cn

Ruby: a, b = b, a
来源：http://hp.szsharing.cn

C#:   (a, b) = (b, a);
来源：http://eq.lnxyls.cn

[A20] 读取标准输入
来源：http://ro.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://oz.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://um.newstarts.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hi.jctech888.com.cn

TS:   // Node.js：readline 模块
来源：http://xl.huixinmuqiang.cn

Java: new Scanner(System.in).nextLine()
来源：http://ve.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pj.szxytkj.cn

Ruby: gets.chomp
来源：http://ig.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://db.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://wr.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://tx.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tc.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://nw.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://mu.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://oo.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fl.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://aa.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://qg.521024.cn

[A22] 获取字符串长度
来源：http://ru.yuntaijiaju.cn

Py:   len(s)
来源：http://pu.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://io.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pj.colortex.cn

TS:   s.length
来源：http://xg.shxzukj.cn

Java: s.length()
来源：http://hx.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ec.nicolike.cn

Ruby: s.length
来源：http://bd.shxzskj.cn

C#:   s.Length
来源：http://go.shtwfgs.cn

[A23] 大小写转换
来源：http://os.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jr.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fo.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ze.chemitech.net.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bx.jianghongdianzi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yy.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://um.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://iv.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jd.lnxyls.cn

[A24] 去除首尾空白
来源：http://zk.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://us.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://th.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yb.huixinmuqiang.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://op.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cl.521024.cn

Go:   strings.TrimSpace(s)
来源：http://af.nicolike.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xa.szxytkj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hl.nicolike.cn

[A25] 字符串比较
来源：http://sz.hahajie.cn

Py:   s1 == s2; s1 != s2
来源：http://lo.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mb.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tj.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hi.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oq.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://py.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kg.yuexingan06.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iw.lnxyls.cn

[A26] 类型转换总览
来源：http://lx.gzmigu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wc.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xx.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bl.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://il.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mj.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kh.hahajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kz.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pj.bjjhwx.cn

================================================================================
来源：http://ty.muxihuayi.cn

B. 流程控制
来源：http://hy.szxytkj.cn

================================================================================
来源：http://sz.wgjwhj.cn

[B01] 条件判断 if / else
来源：http://fb.bookmarksfly.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://au.asd995.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://um.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gy.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://li.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sx.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wa.jianghongdianzi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bd.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://su.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://lw.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sh.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nh.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oz.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://is.nicolike.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lk.szsharing.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vr.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zk.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qt.gzmigu.cn

[B03] switch / match / case
来源：http://se.shxzukj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bd.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aq.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tk.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ma.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zq.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ia.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tr.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://az.521024.cn

[B04] for 计数循环
来源：http://pc.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://ki.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ue.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zp.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://an.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lg.hahajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vb.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://zz.shtwfgs.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wf.haigaiapp.cn

[B05] 遍历数组 / 列表
来源：http://by.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://aa.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xy.szxytkj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qk.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://by.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://te.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oq.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://dz.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xo.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://ng.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hu.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tx.gzmigu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ue.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ne.huixinmuqiang.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://up.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://br.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://od.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wc.jianghongdianzi.cn

[B07] while 循环
来源：http://gd.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://bj.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lp.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://mh.huixiangedu.cn

TS:   while (i < 10) { i++; }
来源：http://wr.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://sn.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://um.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://rl.hnjuh.cn

C#:   while (i < 10) { i++; }
来源：http://nl.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://rf.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://mg.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pb.asd995.cn

JS:   do { i++; } while (i < 10);
来源：http://yz.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://om.szxytkj.cn

Java: do { i++; } while (i < 10);
来源：http://hb.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://it.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gj.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://tu.521024.cn

[B09] break 与 continue
来源：http://un.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tz.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://km.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dh.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qm.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jr.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rm.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xf.521024.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zq.nszjky.cn

[B10] 遍历同时拿索引
来源：http://dr.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hy.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://br.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xx.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sm.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ov.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zt.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pa.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ch.9csxet.cn

[B11] 生成数字序列 / 区间
来源：http://wa.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://kt.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://rp.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sh.jctech888.com.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pp.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mz.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zo.huixiangedu.cn

Ruby: (0...10).step(2).to_a
来源：http://dl.huanxung.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bm.huixinmuqiang.cn

[B12] 跳出多层循环
来源：http://ik.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://lv.huixinmuqiang.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rs.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://de.huanxung.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zw.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ec.wgjwhj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://su.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rf.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mi.lnxyls.cn

[B13] 判断是否为数字
来源：http://gz.shxzskj.cn

Py:   isinstance(x, (int, float))
来源：http://ql.shxzukj.cn

PHP:  is_numeric($x)
来源：http://ou.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tl.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lw.szsharing.cn

Java: x instanceof Number
来源：http://ru.gzmigu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qf.bjjhwx.cn

Ruby: x.is_a?(Numeric)
来源：http://iw.huanxung.cn

C#:   x is int or double or decimal
来源：http://uj.asd995.cn

[B14] 判断值是否在集合内
来源：http://sv.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ud.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vt.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://nh.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://do.haigaiapp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kv.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bf.szsharing.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tl.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://is.jctech888.com.cn

[B15] 布尔运算与取反
来源：http://ll.shxzukj.cn

Py:   a and b or not c
来源：http://fc.newstarts.cn

PHP:  $a && $b || !$c
来源：http://ah.wgjwhj.cn

JS:   a && b || !c
来源：http://sc.9csxet.cn

TS:   a && b || !c
来源：http://ck.shtwfgs.cn

Java: a && b || !c
来源：http://bd.521024.cn


<!-- 参考信息 -->