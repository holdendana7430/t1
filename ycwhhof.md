代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://by.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xd.yuexingan06.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wc.huixinmuqiang.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cm.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ay.jctech888.com.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hq.bjjhwx.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ix.jctech888.com.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://av.9csxet.cn

[A10] 生成随机数
来源：http://ek.nszjky.cn

Py:   import random; random.randint(1, 100)
来源：http://nr.bjjhwx.cn

PHP:  random_int(1, 100);
来源：http://yj.hnjuh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bv.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jk.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://zg.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vp.shxzskj.cn

Ruby: rand(1..100)
来源：http://ho.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://az.lnxyls.cn

[A11] 条件表达式（三元）
来源：http://mr.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://zz.szxytkj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fu.9csxet.cn

JS:   x > 0 ? "yes" : "no"
来源：http://mp.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mu.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://gp.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mt.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pu.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sw.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://gw.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cs.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kl.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://iz.521024.cn

TS:   `Hello, ${name}!`
来源：http://wo.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://yg.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ci.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://of.huixinmuqiang.cn

C#:   $"Hello, {name}!"
来源：http://se.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sh.colortex.cn

Py:   "第一行\n第二行"
来源：http://li.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://yo.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://xk.colortex.cn

TS:   "第一行\n第二行"
来源：http://or.chemitech.net.cn

Java: "第一行\n第二行"
来源：http://br.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://nb.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://yr.9csxet.cn

C#:   "第一行\n第二行"
来源：http://nh.yuntaijiaju.cn

[A14] 注释写法
来源：http://ir.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vz.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ru.yuexingan06.cn

JS:   // 单行；/* 多行 */
来源：http://zo.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://tf.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ct.huixiangedu.cn

Go:   // 单行；/* 多行 */
来源：http://rw.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zq.hnjuh.cn

C#:   // 单行；/* 多行 */
来源：http://wt.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://dz.9csxet.cn

Py:   value = data or "默认值"
来源：http://vp.wgjwhj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ic.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://mg.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://xt.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cq.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://gp.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://ak.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://hn.shxzukj.cn

[A16] 真假值判断规则
来源：http://uq.hnjuh.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ws.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jr.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vo.asd995.cn

TS:   if (!x) {}
来源：http://xr.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cs.huanxung.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://as.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ze.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rc.hnjuh.cn

[A17] 位运算
来源：http://ik.jctech888.com.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ie.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mg.huanxung.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://em.nszjky.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://np.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sg.yuntaijiaju.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zu.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yk.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://be.huixiangedu.cn

[A18] 字符与 ASCII 码互转
来源：http://em.521024.cn

Py:   ord("A"); chr(65)
来源：http://qx.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://bz.szsharing.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bi.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://od.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://tc.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kb.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://wt.521024.cn

C#:   (int)'A'; (char)65
来源：http://sj.shtwfgs.cn

[A19] 交换两个变量
来源：http://fc.shxzukj.cn

Py:   a, b = b, a
来源：http://es.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://et.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://hw.panjiajie.cn

TS:   [a, b] = [b, a];
来源：http://gl.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://ad.huixiangedu.cn

Go:   a, b = b, a
来源：http://uf.521024.cn

Ruby: a, b = b, a
来源：http://nd.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://il.gzmigu.cn

[A20] 读取标准输入
来源：http://hm.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://du.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mu.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fr.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://is.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://bf.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rn.hnjuh.cn

Ruby: gets.chomp
来源：http://ux.hnjuh.cn

C#:   Console.ReadLine();
来源：http://mj.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://ll.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://ur.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zw.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://xy.huixinmuqiang.cn

TS:   (3.14159).toFixed(2)
来源：http://cg.panjiajie.cn

Java: String.format("%.2f", 3.14159)
来源：http://nd.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sx.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://cd.panjiajie.cn

C#:   3.14159.ToString("F2")
来源：http://if.lnxyls.cn

[A22] 获取字符串长度
来源：http://ar.huanxung.cn

Py:   len(s)
来源：http://zt.9csxet.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lh.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ou.shtwfgs.cn

TS:   s.length
来源：http://cr.panjiajie.cn

Java: s.length()
来源：http://nv.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cd.szxytkj.cn

Ruby: s.length
来源：http://su.haigaiapp.cn

C#:   s.Length
来源：http://bi.panjiajie.cn

[A23] 大小写转换
来源：http://xb.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ne.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ua.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wu.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kx.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pb.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eb.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ij.lnxyls.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tk.szxytkj.cn

[A24] 去除首尾空白
来源：http://jd.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ds.hnjuh.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://np.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yj.szxytkj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ri.shxzskj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bn.521024.cn

Go:   strings.TrimSpace(s)
来源：http://im.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vd.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ub.muxihuayi.cn

[A25] 字符串比较
来源：http://zv.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://ye.chemitech.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wc.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rk.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zi.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ze.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://un.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://en.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ro.huixiangedu.cn

[A26] 类型转换总览
来源：http://er.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://un.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ph.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ba.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://rq.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://js.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nh.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ya.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dp.shxzukj.cn

================================================================================
来源：http://dn.shxzukj.cn

B. 流程控制
来源：http://ry.hahajie.cn

================================================================================
来源：http://sz.colortex.cn

[B01] 条件判断 if / else
来源：http://vc.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lu.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mt.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://of.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qj.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ka.muxihuayi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xp.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tk.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ss.panjiajie.cn

[B02] 多分支 else if / elif
来源：http://yd.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uo.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sl.panjiajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wt.hnjuh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bd.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://di.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vv.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://di.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wx.panjiajie.cn

[B03] switch / match / case
来源：http://wq.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nv.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ou.jianghongdianzi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://di.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ss.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sl.szxytkj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oc.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://an.huanxung.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ft.hnjuh.cn

[B04] for 计数循环
来源：http://px.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://wa.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ds.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nv.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lq.shtwfgs.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vp.jctech888.com.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zj.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://ao.gzmigu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wk.521024.cn

[B05] 遍历数组 / 列表
来源：http://jj.hnjuh.cn

Py:   for item in arr: print(item)
来源：http://aa.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gf.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gp.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xk.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://il.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gs.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://pz.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cw.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://vh.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gq.haigaiapp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hr.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rc.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mr.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hw.jctech888.com.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ud.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zq.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hv.lnxyls.cn

[B07] while 循环
来源：http://cp.newstarts.cn

Py:   while i < 10: i += 1
来源：http://zy.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jctech888.com.cn

JS:   while (i < 10) { i++; }
来源：http://hr.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://zh.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://vi.huixinmuqiang.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xm.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://aw.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://gc.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://bt.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://ql.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qc.hahajie.cn

JS:   do { i++; } while (i < 10);
来源：http://bs.yuntaijiaju.cn

TS:   do { i++; } while (i < 10);
来源：http://hw.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://lp.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jh.asd995.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jm.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://aj.szsharing.cn

[B09] break 与 continue
来源：http://ru.gzmigu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ch.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://er.asd995.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mm.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://re.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ef.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gg.9csxet.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cb.lnxyls.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ti.shtwfgs.cn

[B10] 遍历同时拿索引
来源：http://du.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yr.521024.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yy.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ex.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qd.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://re.nszjky.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xw.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vd.jianghongdianzi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jx.colortex.cn

[B11] 生成数字序列 / 区间
来源：http://xa.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://rh.haigaiapp.cn

PHP:  range(0, 10, 2);
来源：http://lm.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mu.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ra.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sm.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yc.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://xu.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xw.shxzskj.cn

[B12] 跳出多层循环
来源：http://dy.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mk.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ps.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zf.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://la.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://go.hahajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uz.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xc.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://no.muxihuayi.cn

[B13] 判断是否为数字
来源：http://eg.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://an.colortex.cn

PHP:  is_numeric($x)
来源：http://za.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kd.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cn.panjiajie.cn

Java: x instanceof Number
来源：http://bz.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cd.jianghongdianzi.cn

Ruby: x.is_a?(Numeric)
来源：http://jz.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://tr.jianghongdianzi.cn

[B14] 判断值是否在集合内
来源：http://dq.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gd.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yv.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://mw.lnxyls.cn

TS:   [1, 2, 3].includes(x)
来源：http://jp.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nx.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ub.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wf.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fm.panjiajie.cn

[B15] 布尔运算与取反
来源：http://md.chemitech.net.cn

Py:   a and b or not c
来源：http://oq.huanxung.cn

PHP:  $a && $b || !$c
来源：http://ek.szsharing.cn

JS:   a && b || !c
来源：http://po.nicolike.cn

TS:   a && b || !c
来源：http://sd.9csxet.cn

Java: a && b || !c
来源：http://bn.huixinmuqiang.cn

Go:   a && b || !c
来源：http://jp.colortex.cn

Ruby: a && b || !c
来源：http://ao.jianghongdianzi.cn

C#:   a && b || !c
来源：http://xu.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lm.nicolike.cn


<!-- 参考信息 -->