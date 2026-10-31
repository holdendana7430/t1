代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hj.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gy.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://au.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pr.nszjky.cn

[A10] 生成随机数
来源：http://pe.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://ra.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://dy.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pw.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dn.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://ki.szsharing.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ne.521024.cn

Ruby: rand(1..100)
来源：http://af.szxytkj.cn

C#:   new Random().Next(1, 101)
来源：http://kr.huanxung.cn

[A11] 条件表达式（三元）
来源：http://vs.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://vd.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hh.wgjwhj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xb.lnxyls.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yl.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://qf.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kd.szxytkj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jc.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hq.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://hz.asd995.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pd.panjiajie.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fx.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://vp.colortex.cn

TS:   `Hello, ${name}!`
来源：http://tp.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://hi.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yb.521024.cn

Ruby: "Hello, #{name}!"
来源：http://rs.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://sr.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ll.wgjwhj.cn

Py:   "第一行\n第二行"
来源：http://yy.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://cs.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://ic.colortex.cn

TS:   "第一行\n第二行"
来源：http://do.nicolike.cn

Java: "第一行\n第二行"
来源：http://hl.szxytkj.cn

Go:   "第一行\n第二行"
来源：http://oz.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://ce.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://zb.jianghongdianzi.cn

[A14] 注释写法
来源：http://lp.asd995.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ov.haigaiapp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hj.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://ae.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://pp.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fn.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://jh.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wv.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://wy.newstarts.cn

[A15] 空值判断与默认值
来源：http://gy.nicolike.cn

Py:   value = data or "默认值"
来源：http://pt.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://if.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://eg.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://qy.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://do.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://og.lnxyls.cn

Ruby: value = data || "默认值"
来源：http://ib.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://if.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://ia.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fa.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fw.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hk.huanxung.cn

TS:   if (!x) {}
来源：http://lz.huixiangedu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fv.jianghongdianzi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uu.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vg.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://se.huixinmuqiang.cn

[A17] 位运算
来源：http://xm.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sa.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ky.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xw.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xf.newstarts.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eo.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wk.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://st.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kl.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://zn.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://jy.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://os.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ei.huixiangedu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eu.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://on.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lp.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://ki.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://pm.hnjuh.cn

[A19] 交换两个变量
来源：http://xq.shxzukj.cn

Py:   a, b = b, a
来源：http://pq.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vy.colortex.cn

JS:   [a, b] = [b, a];
来源：http://sh.huixiangedu.cn

TS:   [a, b] = [b, a];
来源：http://wf.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://ej.haigaiapp.cn

Go:   a, b = b, a
来源：http://ry.gzmigu.cn

Ruby: a, b = b, a
来源：http://oz.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://hw.colortex.cn

[A20] 读取标准输入
来源：http://jt.hahajie.cn

Py:   name = input("请输入：")
来源：http://vy.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://if.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://js.muxihuayi.cn

TS:   // Node.js：readline 模块
来源：http://ql.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://zi.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lm.panjiajie.cn

Ruby: gets.chomp
来源：http://bn.nszjky.cn

C#:   Console.ReadLine();
来源：http://wr.521024.cn

[A21] 保留指定小数位输出
来源：http://mz.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://sc.lnxyls.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://li.huixiangedu.cn

JS:   (3.14159).toFixed(2)
来源：http://qi.panjiajie.cn

TS:   (3.14159).toFixed(2)
来源：http://oc.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ah.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ui.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://fy.yuntaijiaju.cn

C#:   3.14159.ToString("F2")
来源：http://zf.gzmigu.cn

[A22] 获取字符串长度
来源：http://sv.bjjhwx.cn

Py:   len(s)
来源：http://hv.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://on.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oi.haigaiapp.cn

TS:   s.length
来源：http://ut.hahajie.cn

Java: s.length()
来源：http://ty.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dt.hnjuh.cn

Ruby: s.length
来源：http://ll.hahajie.cn

C#:   s.Length
来源：http://go.hnjuh.cn

[A23] 大小写转换
来源：http://ud.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dd.newstarts.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vr.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ky.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ma.gzmigu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vr.colortex.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dd.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rd.yuexingan06.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vk.huixiangedu.cn

[A24] 去除首尾空白
来源：http://xi.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hl.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qg.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iw.hnjuh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hp.gzmigu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xu.jianghongdianzi.cn

Go:   strings.TrimSpace(s)
来源：http://ma.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tz.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://to.wgjwhj.cn

[A25] 字符串比较
来源：http://pu.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://yd.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mv.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bs.shxzskj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qe.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dp.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gm.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://co.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cg.jianghongdianzi.cn

[A26] 类型转换总览
来源：http://kc.lnxyls.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fn.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rd.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ji.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://ki.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://an.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xj.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ju.hahajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gp.521024.cn

================================================================================
来源：http://yq.521024.cn

B. 流程控制
来源：http://lr.shxzukj.cn

================================================================================
来源：http://gk.hnjuh.cn

[B01] 条件判断 if / else
来源：http://nl.haigaiapp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ad.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iq.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mi.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pz.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zo.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qa.yuexingan06.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ge.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sa.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://kb.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oi.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://op.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jd.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bf.jctech888.com.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zi.muxihuayi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jk.shtwfgs.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://av.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gn.gzmigu.cn

[B03] switch / match / case
来源：http://xi.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ob.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://il.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://is.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vt.nicolike.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rh.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dz.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wz.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ch.colortex.cn

[B04] for 计数循环
来源：http://sa.nszjky.cn

Py:   for i in range(10): print(i)
来源：http://ca.szsharing.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vm.nszjky.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ut.newstarts.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uk.jianghongdianzi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tj.panjiajie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ry.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://wg.panjiajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iq.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://rj.colortex.cn

Py:   for item in arr: print(item)
来源：http://ra.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jy.panjiajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kh.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fo.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pa.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rc.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://ds.jctech888.com.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kw.521024.cn

[B06] 遍历字典 / 对象
来源：http://fd.bjjhwx.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uy.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sh.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kv.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kk.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://je.huixinmuqiang.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ub.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://em.jianghongdianzi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vi.hahajie.cn

[B07] while 循环
来源：http://ku.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://ya.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ob.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://by.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://uh.wgjwhj.cn

Java: while (i < 10) { i++; }
来源：http://tz.panjiajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oz.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://bc.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://gx.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://xn.nicolike.cn

Py:   # 无 do-while：用 while True + break
来源：http://if.chemitech.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sm.panjiajie.cn

JS:   do { i++; } while (i < 10);
来源：http://ud.nszjky.cn

TS:   do { i++; } while (i < 10);
来源：http://lj.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://ny.muxihuayi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://io.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ba.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://sq.wgjwhj.cn

[B09] break 与 continue
来源：http://ia.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://le.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cz.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://em.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pd.nszjky.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sx.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hm.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ir.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nx.asd995.cn

[B10] 遍历同时拿索引
来源：http://ph.yuntaijiaju.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jm.bjjhwx.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fm.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qq.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jx.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tn.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xa.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rw.yuntaijiaju.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ke.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://uw.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://sk.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://di.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bk.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ru.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sl.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://om.huixinmuqiang.cn

Ruby: (0...10).step(2).to_a
来源：http://cr.szsharing.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lp.yuexingan06.cn

[B12] 跳出多层循环
来源：http://pg.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tp.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jh.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ua.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hn.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zc.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tp.huixiangedu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hp.nicolike.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qf.szsharing.cn

[B13] 判断是否为数字
来源：http://sg.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://ca.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://js.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ai.bjjhwx.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iw.bookmarksfly.cn

Java: x instanceof Number
来源：http://fi.haigaiapp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ul.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://eo.nszjky.cn

C#:   x is int or double or decimal
来源：http://fw.newstarts.cn

[B14] 判断值是否在集合内
来源：http://ru.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ta.gzmigu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yk.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://by.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://oe.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ic.muxihuayi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eh.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sc.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qy.lnxyls.cn

[B15] 布尔运算与取反
来源：http://dl.muxihuayi.cn

Py:   a and b or not c
来源：http://lj.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://cy.nszjky.cn

JS:   a && b || !c
来源：http://we.hahajie.cn

TS:   a && b || !c
来源：http://do.muxihuayi.cn

Java: a && b || !c
来源：http://qf.yuexingan06.cn

Go:   a && b || !c
来源：http://jn.lnxyls.cn

Ruby: a && b || !c
来源：http://ss.huixiangedu.cn

C#:   a && b || !c
来源：http://zk.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jd.gzmigu.cn

Py:   if not data: return
来源：http://cg.muxihuayi.cn

PHP:  if (!$data) { return; }
来源：http://yw.newstarts.cn

JS:   if (!data) return;
来源：http://nk.huanxung.cn

TS:   if (!data) return;
来源：http://ou.haigaiapp.cn


<!-- 参考信息 -->