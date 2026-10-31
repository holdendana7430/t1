代发 wailian999

[A10] 生成随机数
来源：http://ku.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://mm.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://kz.nszjky.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tg.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jg.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://gd.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pe.hahajie.cn

Ruby: rand(1..100)
来源：http://sv.wgjwhj.cn

C#:   new Random().Next(1, 101)
来源：http://mk.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://xk.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://ab.colortex.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hm.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fg.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xh.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://kp.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://uo.bjjhwx.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nr.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ww.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://do.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lo.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://je.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://ki.nicolike.cn

TS:   `Hello, ${name}!`
来源：http://hw.panjiajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://oa.asd995.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sj.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://pg.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://md.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mt.521024.cn

Py:   "第一行\n第二行"
来源：http://qc.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://im.521024.cn

JS:   "第一行\n第二行"
来源：http://ey.colortex.cn

TS:   "第一行\n第二行"
来源：http://cx.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://ca.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://ik.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://br.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://ny.newstarts.cn

[A14] 注释写法
来源：http://wn.panjiajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kk.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xk.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://tx.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://tj.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ya.bookmarksfly.cn

Go:   // 单行；/* 多行 */
来源：http://gl.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kr.9csxet.cn

C#:   // 单行；/* 多行 */
来源：http://sh.lnxyls.cn

[A15] 空值判断与默认值
来源：http://oo.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://gq.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://ik.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://xz.huixiangedu.cn

TS:   const value = data ?? "默认值";
来源：http://vm.colortex.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://td.bookmarksfly.cn

Go:   if data == "" { data = "默认值" }
来源：http://fv.chemitech.net.cn

Ruby: value = data || "默认值"
来源：http://nc.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://mv.huixiangedu.cn

[A16] 真假值判断规则
来源：http://ck.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fl.gzmigu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qq.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hg.gzmigu.cn

TS:   if (!x) {}
来源：http://pu.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qg.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pg.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hh.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pb.chemitech.net.cn

[A17] 位运算
来源：http://bp.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zu.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nr.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sw.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ew.wgjwhj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://em.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yy.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xm.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ej.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://vs.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://it.9csxet.cn

PHP:  ord("A"); chr(65)
来源：http://ev.huixinmuqiang.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kr.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fk.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://ug.wgjwhj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ca.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://dr.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://nu.colortex.cn

[A19] 交换两个变量
来源：http://ot.9csxet.cn

Py:   a, b = b, a
来源：http://yg.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yp.bjjhwx.cn

JS:   [a, b] = [b, a];
来源：http://tz.asd995.cn

TS:   [a, b] = [b, a];
来源：http://pw.jctech888.com.cn

Java: int t = a; a = b; b = t;
来源：http://uz.nicolike.cn

Go:   a, b = b, a
来源：http://hk.9csxet.cn

Ruby: a, b = b, a
来源：http://up.hahajie.cn

C#:   (a, b) = (b, a);
来源：http://fn.szxytkj.cn

[A20] 读取标准输入
来源：http://ig.521024.cn

Py:   name = input("请输入：")
来源：http://vs.newstarts.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mv.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yt.521024.cn

TS:   // Node.js：readline 模块
来源：http://oh.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://ii.panjiajie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xn.panjiajie.cn

Ruby: gets.chomp
来源：http://ws.newstarts.cn

C#:   Console.ReadLine();
来源：http://tk.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://qe.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://zy.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yw.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://qc.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://un.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://gq.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ak.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://rg.szsharing.cn

C#:   3.14159.ToString("F2")
来源：http://sn.colortex.cn

[A22] 获取字符串长度
来源：http://sa.shxzskj.cn

Py:   len(s)
来源：http://di.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ed.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jv.bjjhwx.cn

TS:   s.length
来源：http://bs.muxihuayi.cn

Java: s.length()
来源：http://gs.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bn.hnjuh.cn

Ruby: s.length
来源：http://ph.shtwfgs.cn

C#:   s.Length
来源：http://gk.szsharing.cn

[A23] 大小写转换
来源：http://hk.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rr.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://su.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tb.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dh.nicolike.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ec.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rp.szsharing.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yg.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gg.gzmigu.cn

[A24] 去除首尾空白
来源：http://yc.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oe.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xq.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jc.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rh.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://br.521024.cn

Go:   strings.TrimSpace(s)
来源：http://mj.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qz.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://up.nszjky.cn

[A25] 字符串比较
来源：http://vc.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://qf.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qf.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rp.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lv.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gi.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ft.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wo.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mz.yuexingan06.cn

[A26] 类型转换总览
来源：http://hb.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xw.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gi.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rg.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://rw.haigaiapp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yp.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://et.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ph.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://to.shtwfgs.cn

================================================================================
来源：http://xl.hnjuh.cn

B. 流程控制
来源：http://tg.szxytkj.cn

================================================================================
来源：http://ej.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://na.muxihuayi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nb.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hw.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mj.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ig.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hk.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://io.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ha.bookmarksfly.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bs.colortex.cn

[B02] 多分支 else if / elif
来源：http://mp.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aw.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kh.huixiangedu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tu.bjjhwx.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gz.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nh.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ny.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jw.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wh.wgjwhj.cn

[B03] switch / match / case
来源：http://gp.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://el.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mc.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jk.lnxyls.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yd.muxihuayi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ct.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kq.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tq.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://on.shxzukj.cn

[B04] for 计数循环
来源：http://gt.yuexingan06.cn

Py:   for i in range(10): print(i)
来源：http://rn.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cq.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xr.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gy.szsharing.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cw.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://is.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://bv.shxzukj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://di.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://qk.szsharing.cn

Py:   for item in arr: print(item)
来源：http://rk.bookmarksfly.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dv.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pz.szsharing.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qk.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jm.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dp.huixinmuqiang.cn

Ruby: arr.each { |item| puts item }
来源：http://jj.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gs.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://rq.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mp.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nu.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ig.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nt.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ef.bookmarksfly.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sx.panjiajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mr.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kz.asd995.cn

[B07] while 循环
来源：http://jc.huixiangedu.cn

Py:   while i < 10: i += 1
来源：http://lh.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lu.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://oy.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://ae.colortex.cn

Java: while (i < 10) { i++; }
来源：http://ox.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qg.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://di.huixiangedu.cn

C#:   while (i < 10) { i++; }
来源：http://rq.hnjuh.cn

[B08] do-while（至少执行一次）
来源：http://ot.9csxet.cn

Py:   # 无 do-while：用 while True + break
来源：http://ai.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://is.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://ix.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://cx.shxzskj.cn

Java: do { i++; } while (i < 10);
来源：http://um.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uq.hahajie.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qb.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://ph.521024.cn

[B09] break 与 continue
来源：http://ln.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zr.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eo.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ju.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oq.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gn.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ke.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://of.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nb.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://za.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fo.lnxyls.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ky.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qh.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hr.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lb.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ve.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ky.hnjuh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ff.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://ki.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://ea.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://qd.hahajie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oe.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://an.hahajie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ku.huixinmuqiang.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cn.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://fl.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bi.shtwfgs.cn

[B12] 跳出多层循环
来源：http://ba.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://od.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ox.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gj.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qd.jianghongdianzi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mx.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qy.bjjhwx.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qo.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cp.huixiangedu.cn

[B13] 判断是否为数字
来源：http://pq.nszjky.cn

Py:   isinstance(x, (int, float))
来源：http://el.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://xf.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gp.newstarts.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nv.wgjwhj.cn

Java: x instanceof Number
来源：http://xq.yuexingan06.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://or.shxzukj.cn

Ruby: x.is_a?(Numeric)
来源：http://lj.nicolike.cn

C#:   x is int or double or decimal
来源：http://gu.nszjky.cn

[B14] 判断值是否在集合内
来源：http://db.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aj.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cy.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://ob.newstarts.cn

TS:   [1, 2, 3].includes(x)
来源：http://jm.hnjuh.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vh.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ep.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jc.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dp.hnjuh.cn

[B15] 布尔运算与取反
来源：http://mn.gzmigu.cn

Py:   a and b or not c
来源：http://fo.muxihuayi.cn

PHP:  $a && $b || !$c
来源：http://eq.shxzskj.cn

JS:   a && b || !c
来源：http://pd.bjjhwx.cn

TS:   a && b || !c
来源：http://lu.jctech888.com.cn

Java: a && b || !c
来源：http://sv.szsharing.cn

Go:   a && b || !c
来源：http://oz.huanxung.cn

Ruby: a && b || !c
来源：http://hq.szsharing.cn

C#:   a && b || !c
来源：http://yj.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ps.shxzskj.cn

Py:   if not data: return
来源：http://ls.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://jq.bjjhwx.cn

JS:   if (!data) return;
来源：http://xo.yuexingan06.cn

TS:   if (!data) return;
来源：http://ta.nicolike.cn

Java: if (data == null) return;
来源：http://tz.yuexingan06.cn

Go:   if data == nil { return }
来源：http://mk.bjjhwx.cn

Ruby: return if data.nil?
来源：http://uz.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://yu.jianghongdianzi.cn


<!-- 参考信息 -->