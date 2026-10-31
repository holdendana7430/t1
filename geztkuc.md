代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cx.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ff.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pp.nicolike.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eu.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ne.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gm.huanxung.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qi.haigaiapp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mf.wgjwhj.cn

[A10] 生成随机数
来源：http://mt.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://oi.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://kj.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ig.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zn.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://rj.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bo.lnxyls.cn

Ruby: rand(1..100)
来源：http://kc.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://qa.521024.cn

[A11] 条件表达式（三元）
来源：http://tr.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://sh.bookmarksfly.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jx.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://iz.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ms.9csxet.cn

Java: x > 0 ? "yes" : "no"
来源：http://sb.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nr.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qu.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://wq.521024.cn

[A12] 字符串插值 / 格式化
来源：http://ij.haigaiapp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zs.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hk.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://aj.colortex.cn

TS:   `Hello, ${name}!`
来源：http://nm.asd995.cn

Java: "Hello, %s!".formatted(name)
来源：http://ur.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://on.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://vv.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://at.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lr.hahajie.cn

Py:   "第一行\n第二行"
来源：http://hi.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://bw.9csxet.cn

JS:   "第一行\n第二行"
来源：http://ie.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://rt.shxzskj.cn

Java: "第一行\n第二行"
来源：http://qo.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://el.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://aj.hahajie.cn

C#:   "第一行\n第二行"
来源：http://ex.muxihuayi.cn

[A14] 注释写法
来源：http://wq.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lp.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://eb.huanxung.cn

JS:   // 单行；/* 多行 */
来源：http://dz.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://wa.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dx.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://qb.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://yr.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://mv.huanxung.cn

[A15] 空值判断与默认值
来源：http://kh.521024.cn

Py:   value = data or "默认值"
来源：http://nn.newstarts.cn

PHP:  $value = $data ?? "默认值";
来源：http://bh.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://lx.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://yt.huixiangedu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wy.shxzskj.cn

Go:   if data == "" { data = "默认值" }
来源：http://xz.521024.cn

Ruby: value = data || "默认值"
来源：http://ri.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://ei.asd995.cn

[A16] 真假值判断规则
来源：http://vj.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dh.lnxyls.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cv.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kg.shtwfgs.cn

TS:   if (!x) {}
来源：http://jc.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pa.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ib.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ve.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zk.9csxet.cn

[A17] 位运算
来源：http://kl.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vz.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bh.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bj.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sv.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mi.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tw.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eu.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vo.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://kx.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://od.gzmigu.cn

PHP:  ord("A"); chr(65)
来源：http://fd.jianghongdianzi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://te.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qb.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://ri.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rn.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://un.szxytkj.cn

C#:   (int)'A'; (char)65
来源：http://yv.yuexingan06.cn

[A19] 交换两个变量
来源：http://bb.nszjky.cn

Py:   a, b = b, a
来源：http://sa.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nu.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://so.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://cf.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://ek.panjiajie.cn

Go:   a, b = b, a
来源：http://ka.asd995.cn

Ruby: a, b = b, a
来源：http://lk.yuntaijiaju.cn

C#:   (a, b) = (b, a);
来源：http://qt.nszjky.cn

[A20] 读取标准输入
来源：http://fx.huanxung.cn

Py:   name = input("请输入：")
来源：http://ag.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kt.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rp.lnxyls.cn

TS:   // Node.js：readline 模块
来源：http://qq.gzmigu.cn

Java: new Scanner(System.in).nextLine()
来源：http://sx.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ca.szxytkj.cn

Ruby: gets.chomp
来源：http://uj.shxzukj.cn

C#:   Console.ReadLine();
来源：http://th.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://jk.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://ym.shxzskj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xg.jianghongdianzi.cn

JS:   (3.14159).toFixed(2)
来源：http://lr.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://kw.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://bw.9csxet.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ub.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://hv.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://it.9csxet.cn

[A22] 获取字符串长度
来源：http://oa.gzmigu.cn

Py:   len(s)
来源：http://ln.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rx.lnxyls.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nj.newstarts.cn

TS:   s.length
来源：http://ou.jianghongdianzi.cn

Java: s.length()
来源：http://lv.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vt.bjjhwx.cn

Ruby: s.length
来源：http://xx.hahajie.cn

C#:   s.Length
来源：http://th.haigaiapp.cn

[A23] 大小写转换
来源：http://yq.newstarts.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://aj.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oy.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uw.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nc.huanxung.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://am.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hs.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zf.chemitech.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gx.szsharing.cn

[A24] 去除首尾空白
来源：http://cc.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gk.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xz.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tj.521024.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mm.shxzukj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ls.huanxung.cn

Go:   strings.TrimSpace(s)
来源：http://gf.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wt.chemitech.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ze.hahajie.cn

[A25] 字符串比较
来源：http://uk.yuntaijiaju.cn

Py:   s1 == s2; s1 != s2
来源：http://pb.asd995.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nh.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ni.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vl.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zl.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rr.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vx.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wv.nicolike.cn

[A26] 类型转换总览
来源：http://tk.nicolike.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hv.521024.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xw.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ol.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://wu.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fb.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jv.shtwfgs.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uf.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pp.bjjhwx.cn

================================================================================
来源：http://lb.hahajie.cn

B. 流程控制
来源：http://qe.huixiangedu.cn

================================================================================
来源：http://ex.szsharing.cn

[B01] 条件判断 if / else
来源：http://ak.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pw.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://az.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uo.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uo.bookmarksfly.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wi.hahajie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pi.colortex.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ls.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sg.huanxung.cn

[B02] 多分支 else if / elif
来源：http://ap.haigaiapp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ei.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://df.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ig.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ti.shxzskj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yr.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kb.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yy.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eh.szsharing.cn

[B03] switch / match / case
来源：http://th.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dh.huixinmuqiang.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lk.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lv.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wz.szxytkj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ok.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xb.lnxyls.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hd.wgjwhj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cy.huanxung.cn

[B04] for 计数循环
来源：http://pl.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://cy.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pd.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rb.jianghongdianzi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ag.gzmigu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ng.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pu.newstarts.cn

Ruby: 10.times { |i| puts i }
来源：http://np.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tu.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://oe.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://su.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lg.bookmarksfly.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qq.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dp.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vq.jctech888.com.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qd.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://vv.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://by.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://gj.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://th.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hn.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ul.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bw.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mb.nicolike.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bf.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ln.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qs.nszjky.cn

[B07] while 循环
来源：http://vb.szsharing.cn

Py:   while i < 10: i += 1
来源：http://gq.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://td.muxihuayi.cn

JS:   while (i < 10) { i++; }
来源：http://lt.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://vc.nszjky.cn

Java: while (i < 10) { i++; }
来源：http://ra.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wd.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://ey.nicolike.cn

C#:   while (i < 10) { i++; }
来源：http://nv.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://aj.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://an.asd995.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vh.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://za.wgjwhj.cn

TS:   do { i++; } while (i < 10);
来源：http://nf.gzmigu.cn

Java: do { i++; } while (i < 10);
来源：http://uk.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sa.gzmigu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tm.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://zt.jctech888.com.cn

[B09] break 与 continue
来源：http://hr.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ax.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zv.haigaiapp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zn.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lg.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vm.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ul.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tm.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hf.nszjky.cn

[B10] 遍历同时拿索引
来源：http://do.huixiangedu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cm.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bf.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ta.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lb.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rp.asd995.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ui.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ze.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sj.muxihuayi.cn

[B11] 生成数字序列 / 区间
来源：http://pu.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://uy.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://lq.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ad.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dx.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hd.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gj.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://sn.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ls.huixiangedu.cn

[B12] 跳出多层循环
来源：http://fg.chemitech.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tg.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bb.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tk.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://do.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ps.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lk.colortex.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jr.newstarts.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dt.nszjky.cn

[B13] 判断是否为数字
来源：http://kx.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://lr.shxzskj.cn

PHP:  is_numeric($x)
来源：http://ew.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hn.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://td.521024.cn

Java: x instanceof Number
来源：http://lw.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ok.colortex.cn

Ruby: x.is_a?(Numeric)
来源：http://uq.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://ey.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://rm.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ix.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fv.huanxung.cn

JS:   [1, 2, 3].includes(x)
来源：http://cv.wgjwhj.cn

TS:   [1, 2, 3].includes(x)
来源：http://fz.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://te.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ao.huixinmuqiang.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dd.newstarts.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dl.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://pm.wgjwhj.cn

Py:   a and b or not c
来源：http://in.newstarts.cn

PHP:  $a && $b || !$c
来源：http://ma.shtwfgs.cn

JS:   a && b || !c
来源：http://cb.hnjuh.cn

TS:   a && b || !c
来源：http://wm.asd995.cn

Java: a && b || !c
来源：http://jl.colortex.cn

Go:   a && b || !c
来源：http://mp.shxzskj.cn

Ruby: a && b || !c
来源：http://kg.chemitech.net.cn

C#:   a && b || !c
来源：http://ga.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ie.wgjwhj.cn


<!-- 参考信息 -->