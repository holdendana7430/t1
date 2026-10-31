代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fo.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://by.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://id.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qy.asd995.cn

[A10] 生成随机数
来源：http://ty.szxytkj.cn

Py:   import random; random.randint(1, 100)
来源：http://nw.gzmigu.cn

PHP:  random_int(1, 100);
来源：http://as.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jt.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ej.521024.cn

Java: new Random().nextInt(100) + 1
来源：http://bl.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mq.asd995.cn

Ruby: rand(1..100)
来源：http://hx.newstarts.cn

C#:   new Random().Next(1, 101)
来源：http://pg.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://sz.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://ht.521024.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wg.newstarts.cn

JS:   x > 0 ? "yes" : "no"
来源：http://wd.hahajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bn.521024.cn

Java: x > 0 ? "yes" : "no"
来源：http://ip.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dp.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nc.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yb.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://sx.panjiajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bd.nicolike.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mp.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://ck.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://xh.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://cr.shxzskj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kx.gzmigu.cn

Ruby: "Hello, #{name}!"
来源：http://ul.521024.cn

C#:   $"Hello, {name}!"
来源：http://lr.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ci.colortex.cn

Py:   "第一行\n第二行"
来源：http://bf.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://fg.hahajie.cn

JS:   "第一行\n第二行"
来源：http://kl.wgjwhj.cn

TS:   "第一行\n第二行"
来源：http://pm.shxzukj.cn

Java: "第一行\n第二行"
来源：http://bi.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://mq.jianghongdianzi.cn

Ruby: "第一行\n第二行"
来源：http://qo.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://ej.hnjuh.cn

[A14] 注释写法
来源：http://as.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dr.nszjky.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lj.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://ow.chemitech.net.cn

TS:   // 单行；/* 多行 */
来源：http://bg.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rv.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://dz.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vc.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://xs.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://yo.haigaiapp.cn

Py:   value = data or "默认值"
来源：http://om.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://bm.huixinmuqiang.cn

JS:   const value = data ?? "默认值";
来源：http://jc.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://jc.huanxung.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xn.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://dj.nszjky.cn

Ruby: value = data || "默认值"
来源：http://fz.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://qe.shxzukj.cn

[A16] 真假值判断规则
来源：http://xd.newstarts.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jp.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rv.lnxyls.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dm.nszjky.cn

TS:   if (!x) {}
来源：http://yv.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wu.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ns.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qm.gzmigu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ax.asd995.cn

[A17] 位运算
来源：http://mp.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jb.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://go.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sv.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://or.colortex.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hd.lnxyls.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vy.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gp.newstarts.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vf.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://bs.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://uo.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://aw.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wl.huanxung.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://es.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://op.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ku.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://jn.newstarts.cn

C#:   (int)'A'; (char)65
来源：http://jn.muxihuayi.cn

[A19] 交换两个变量
来源：http://hj.szsharing.cn

Py:   a, b = b, a
来源：http://nn.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://el.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://ne.hahajie.cn

TS:   [a, b] = [b, a];
来源：http://hd.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://zl.nicolike.cn

Go:   a, b = b, a
来源：http://wc.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://pb.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://pc.bookmarksfly.cn

[A20] 读取标准输入
来源：http://zq.lnxyls.cn

Py:   name = input("请输入：")
来源：http://pi.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sk.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yc.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://mw.lnxyls.cn

Java: new Scanner(System.in).nextLine()
来源：http://je.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pf.shtwfgs.cn

Ruby: gets.chomp
来源：http://vx.shxzukj.cn

C#:   Console.ReadLine();
来源：http://oz.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://rb.gzmigu.cn

Py:   f"{3.14159:.2f}"
来源：http://cw.bjjhwx.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ac.hahajie.cn

JS:   (3.14159).toFixed(2)
来源：http://gj.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://lx.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://rt.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tv.newstarts.cn

Ruby: format("%.2f", 3.14159)
来源：http://ab.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://zx.lnxyls.cn

[A22] 获取字符串长度
来源：http://sb.haigaiapp.cn

Py:   len(s)
来源：http://iq.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vu.colortex.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xe.szsharing.cn

TS:   s.length
来源：http://sz.colortex.cn

Java: s.length()
来源：http://mt.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pw.yuexingan06.cn

Ruby: s.length
来源：http://fl.jctech888.com.cn

C#:   s.Length
来源：http://ty.panjiajie.cn

[A23] 大小写转换
来源：http://hs.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://cb.huixinmuqiang.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bl.hnjuh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://re.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fu.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://my.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dy.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nz.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cr.jianghongdianzi.cn

[A24] 去除首尾空白
来源：http://mf.jctech888.com.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ir.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fe.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wx.huanxung.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dv.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nq.yuntaijiaju.cn

Go:   strings.TrimSpace(s)
来源：http://bq.szsharing.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bb.newstarts.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ef.jianghongdianzi.cn

[A25] 字符串比较
来源：http://li.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://uh.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uz.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://go.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lm.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bm.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ur.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hy.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zs.9csxet.cn

[A26] 类型转换总览
来源：http://iu.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://um.nicolike.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hp.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kt.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://ul.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ht.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kf.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ho.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fl.szsharing.cn

================================================================================
来源：http://eq.nszjky.cn

B. 流程控制
来源：http://ed.bjjhwx.cn

================================================================================
来源：http://ru.huixiangedu.cn

[B01] 条件判断 if / else
来源：http://zs.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aw.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yt.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yz.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pn.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pz.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ho.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wl.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://io.huanxung.cn

[B02] 多分支 else if / elif
来源：http://wv.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ph.nicolike.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://eu.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tt.nicolike.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://je.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kv.gzmigu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ya.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sm.chemitech.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qu.asd995.cn

[B03] switch / match / case
来源：http://nx.huixinmuqiang.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hk.9csxet.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://in.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oq.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ap.jianghongdianzi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gp.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jh.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lo.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ls.yuexingan06.cn

[B04] for 计数循环
来源：http://qh.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://kh.chemitech.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pu.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fj.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mn.shxzskj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ok.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jj.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://cd.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://te.asd995.cn

[B05] 遍历数组 / 列表
来源：http://af.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://hw.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eo.nicolike.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yh.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kh.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sj.muxihuayi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pr.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://mf.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://od.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://at.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wb.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sj.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zn.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://es.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vm.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ry.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qy.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cj.jianghongdianzi.cn

[B07] while 循环
来源：http://px.nicolike.cn

Py:   while i < 10: i += 1
来源：http://ty.hnjuh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hp.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://cu.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://zr.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://jm.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://az.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://lt.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://ub.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://xm.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://ax.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ll.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://cn.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://on.asd995.cn

Java: do { i++; } while (i < 10);
来源：http://cb.9csxet.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://da.huixinmuqiang.cn

Ruby: begin; i += 1; end while i < 10
来源：http://la.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://ar.hnjuh.cn

[B09] break 与 continue
来源：http://lz.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tq.shtwfgs.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xd.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ca.yuntaijiaju.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ls.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fl.9csxet.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://te.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ag.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hk.hnjuh.cn

[B10] 遍历同时拿索引
来源：http://cj.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yl.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ps.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vv.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://of.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://av.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mu.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tf.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cm.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://dv.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://pf.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://sk.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iz.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tf.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kf.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://em.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://wu.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rf.yuexingan06.cn

[B12] 跳出多层循环
来源：http://wn.szxytkj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nj.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qa.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nu.szxytkj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eu.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zu.gzmigu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ud.chemitech.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://io.chemitech.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ls.muxihuayi.cn

[B13] 判断是否为数字
来源：http://hm.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://sz.nszjky.cn

PHP:  is_numeric($x)
来源：http://sl.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pz.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tp.lnxyls.cn

Java: x instanceof Number
来源：http://wr.hahajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hr.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://jw.haigaiapp.cn

C#:   x is int or double or decimal
来源：http://uq.szxytkj.cn

[B14] 判断值是否在集合内
来源：http://ck.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bc.nicolike.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sq.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://qo.jctech888.com.cn

TS:   [1, 2, 3].includes(x)
来源：http://ds.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://aa.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vl.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cc.chemitech.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jn.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://tj.colortex.cn

Py:   a and b or not c
来源：http://uj.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://tv.bjjhwx.cn

JS:   a && b || !c
来源：http://hi.newstarts.cn

TS:   a && b || !c
来源：http://rk.nszjky.cn

Java: a && b || !c
来源：http://pw.huanxung.cn

Go:   a && b || !c
来源：http://qm.nicolike.cn

Ruby: a && b || !c
来源：http://ow.panjiajie.cn

C#:   a && b || !c
来源：http://ik.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gb.gzmigu.cn

Py:   if not data: return
来源：http://dg.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://bx.szsharing.cn

JS:   if (!data) return;
来源：http://pb.hnjuh.cn

TS:   if (!data) return;
来源：http://hm.wgjwhj.cn


<!-- 参考信息 -->