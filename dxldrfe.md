代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vh.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ug.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bi.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ce.bookmarksfly.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://li.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ow.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://av.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zs.lnxyls.cn

[A10] 生成随机数
来源：http://bo.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://ub.jianghongdianzi.cn

PHP:  random_int(1, 100);
来源：http://yn.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ro.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vl.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://yk.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ba.shxzukj.cn

Ruby: rand(1..100)
来源：http://sh.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://hw.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://ib.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://xz.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rp.bjjhwx.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sd.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ku.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://lm.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://oz.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://yq.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tc.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://sj.chemitech.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fa.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ir.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://gz.asd995.cn

TS:   `Hello, ${name}!`
来源：http://nj.jctech888.com.cn

Java: "Hello, %s!".formatted(name)
来源：http://ls.huixinmuqiang.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kg.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://xx.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://zd.szxytkj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xl.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://zx.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://tx.gzmigu.cn

JS:   "第一行\n第二行"
来源：http://pl.szsharing.cn

TS:   "第一行\n第二行"
来源：http://bu.szsharing.cn

Java: "第一行\n第二行"
来源：http://tv.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://kd.yuntaijiaju.cn

Ruby: "第一行\n第二行"
来源：http://vu.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://cs.521024.cn

[A14] 注释写法
来源：http://ef.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xp.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yz.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://qw.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://lw.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://il.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://ja.9csxet.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tj.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://zg.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://vd.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://im.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://xv.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://fj.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://rw.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nf.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://ab.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://re.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://rd.chemitech.net.cn

[A16] 真假值判断规则
来源：http://em.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zs.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vk.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://km.lnxyls.cn

TS:   if (!x) {}
来源：http://kw.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zx.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tj.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oq.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qc.asd995.cn

[A17] 位运算
来源：http://os.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fw.shxzukj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ov.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://je.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xv.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yf.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ui.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ai.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fr.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://jy.lnxyls.cn

Py:   ord("A"); chr(65)
来源：http://bg.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://bk.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ns.9csxet.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ej.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://kw.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ek.521024.cn

Ruby: "A".ord; 65.chr
来源：http://gi.gzmigu.cn

C#:   (int)'A'; (char)65
来源：http://io.jctech888.com.cn

[A19] 交换两个变量
来源：http://uy.hnjuh.cn

Py:   a, b = b, a
来源：http://sw.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ut.szsharing.cn

JS:   [a, b] = [b, a];
来源：http://vs.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://dz.shtwfgs.cn

Java: int t = a; a = b; b = t;
来源：http://ih.gzmigu.cn

Go:   a, b = b, a
来源：http://hn.hahajie.cn

Ruby: a, b = b, a
来源：http://il.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://it.chemitech.net.cn

[A20] 读取标准输入
来源：http://dv.hahajie.cn

Py:   name = input("请输入：")
来源：http://rp.colortex.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ri.hahajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eq.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://ir.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://kr.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://te.haigaiapp.cn

Ruby: gets.chomp
来源：http://np.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://oa.bjjhwx.cn

[A21] 保留指定小数位输出
来源：http://eq.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://jd.shtwfgs.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zj.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://zo.521024.cn

TS:   (3.14159).toFixed(2)
来源：http://nj.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://uq.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ma.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://vp.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://af.huixiangedu.cn

[A22] 获取字符串长度
来源：http://ju.nszjky.cn

Py:   len(s)
来源：http://to.huanxung.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ai.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sp.chemitech.net.cn

TS:   s.length
来源：http://ur.huixinmuqiang.cn

Java: s.length()
来源：http://ez.hnjuh.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ck.bookmarksfly.cn

Ruby: s.length
来源：http://tm.jianghongdianzi.cn

C#:   s.Length
来源：http://rl.521024.cn

[A23] 大小写转换
来源：http://js.nicolike.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ae.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tl.szxytkj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tl.hnjuh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bm.521024.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fd.jianghongdianzi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kw.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uy.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lg.muxihuayi.cn

[A24] 去除首尾空白
来源：http://yn.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oa.9csxet.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xb.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lh.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eq.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gi.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://up.panjiajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dr.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sc.lnxyls.cn

[A25] 字符串比较
来源：http://ie.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://ev.huixinmuqiang.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wy.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hx.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://op.hahajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gx.9csxet.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://td.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xl.wgjwhj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yl.lnxyls.cn

[A26] 类型转换总览
来源：http://gc.szxytkj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jv.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ir.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mn.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://bg.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ia.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rw.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uv.colortex.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gi.521024.cn

================================================================================
来源：http://dl.colortex.cn

B. 流程控制
来源：http://dv.haigaiapp.cn

================================================================================
来源：http://tu.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://kb.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oc.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ek.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gf.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hf.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xt.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://az.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xs.panjiajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ng.yuexingan06.cn

[B02] 多分支 else if / elif
来源：http://cb.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ri.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qi.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cy.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gw.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wn.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hm.yuntaijiaju.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://si.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ns.bookmarksfly.cn

[B03] switch / match / case
来源：http://jb.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pc.bookmarksfly.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://us.yuexingan06.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rv.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ie.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ss.9csxet.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lz.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lw.hahajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yk.szxytkj.cn

[B04] for 计数循环
来源：http://ei.nicolike.cn

Py:   for i in range(10): print(i)
来源：http://qz.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gb.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wv.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vt.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ot.huixinmuqiang.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yi.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://iq.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pm.muxihuayi.cn

[B05] 遍历数组 / 列表
来源：http://ku.9csxet.cn

Py:   for item in arr: print(item)
来源：http://do.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kq.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zq.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oq.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sb.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ma.lnxyls.cn

Ruby: arr.each { |item| puts item }
来源：http://pe.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ea.jianghongdianzi.cn

[B06] 遍历字典 / 对象
来源：http://su.hahajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dl.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xw.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ar.hahajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hk.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rf.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nk.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bl.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wy.shtwfgs.cn

[B07] while 循环
来源：http://ui.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://hm.yuntaijiaju.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pf.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://of.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://ax.panjiajie.cn

Java: while (i < 10) { i++; }
来源：http://in.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xw.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://xm.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://xi.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://aj.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://vh.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pl.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://mt.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://cs.jianghongdianzi.cn

Java: do { i++; } while (i < 10);
来源：http://xr.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yu.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://iq.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://vx.asd995.cn

[B09] break 与 continue
来源：http://cq.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tv.lnxyls.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rd.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ea.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xp.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bk.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mt.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jv.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ce.asd995.cn

[B10] 遍历同时拿索引
来源：http://fe.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bn.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ok.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pu.huixiangedu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xk.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://om.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zf.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://po.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nm.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://bj.panjiajie.cn

Py:   list(range(0, 10, 2))
来源：http://kp.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://up.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gx.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tn.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fp.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://di.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://zk.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://np.muxihuayi.cn

[B12] 跳出多层循环
来源：http://dl.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wz.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ux.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tw.jctech888.com.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ix.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ks.huanxung.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ur.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://au.huixinmuqiang.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sd.chemitech.net.cn

[B13] 判断是否为数字
来源：http://zj.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://rf.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://zp.jianghongdianzi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gm.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ep.panjiajie.cn

Java: x instanceof Number
来源：http://fh.szsharing.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pt.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://fv.chemitech.net.cn

C#:   x is int or double or decimal
来源：http://wi.szsharing.cn

[B14] 判断值是否在集合内
来源：http://zo.nszjky.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ec.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wk.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://lf.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://ln.9csxet.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ez.jianghongdianzi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rz.shxzskj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ub.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ir.lnxyls.cn

[B15] 布尔运算与取反
来源：http://xj.huanxung.cn

Py:   a and b or not c
来源：http://ww.hahajie.cn

PHP:  $a && $b || !$c
来源：http://um.9csxet.cn

JS:   a && b || !c
来源：http://tq.newstarts.cn

TS:   a && b || !c
来源：http://fd.hahajie.cn

Java: a && b || !c
来源：http://ez.9csxet.cn

Go:   a && b || !c
来源：http://ok.colortex.cn

Ruby: a && b || !c
来源：http://cm.9csxet.cn

C#:   a && b || !c
来源：http://qy.haigaiapp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://se.colortex.cn


<!-- 参考信息 -->