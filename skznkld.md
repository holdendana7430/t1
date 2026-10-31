代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ks.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ns.shxzskj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://se.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gq.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wf.nicolike.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://we.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mm.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sf.colortex.cn

[A10] 生成随机数
来源：http://bj.wgjwhj.cn

Py:   import random; random.randint(1, 100)
来源：http://nu.asd995.cn

PHP:  random_int(1, 100);
来源：http://vy.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://di.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ta.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://nv.shxzukj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qy.bookmarksfly.cn

Ruby: rand(1..100)
来源：http://gb.huixinmuqiang.cn

C#:   new Random().Next(1, 101)
来源：http://gt.9csxet.cn

[A11] 条件表达式（三元）
来源：http://sa.huixiangedu.cn

Py:   "yes" if x > 0 else "no"
来源：http://zx.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kk.hahajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ry.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ev.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://hq.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hb.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ki.huixiangedu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://su.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://hg.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mu.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lx.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://ui.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://nc.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://rq.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yy.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://nh.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://am.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gd.newstarts.cn

Py:   "第一行\n第二行"
来源：http://nr.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://fx.colortex.cn

JS:   "第一行\n第二行"
来源：http://lp.hahajie.cn

TS:   "第一行\n第二行"
来源：http://sj.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://is.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://ia.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://vp.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://vy.asd995.cn

[A14] 注释写法
来源：http://uk.colortex.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://or.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rx.szxytkj.cn

JS:   // 单行；/* 多行 */
来源：http://np.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://ex.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qs.yuntaijiaju.cn

Go:   // 单行；/* 多行 */
来源：http://jq.hnjuh.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ve.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://mz.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://of.shxzskj.cn

Py:   value = data or "默认值"
来源：http://aw.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://kf.nicolike.cn

JS:   const value = data ?? "默认值";
来源：http://go.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://li.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zh.lnxyls.cn

Go:   if data == "" { data = "默认值" }
来源：http://ah.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://hf.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://zs.chemitech.net.cn

[A16] 真假值判断规则
来源：http://oh.szsharing.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hi.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xa.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://no.wgjwhj.cn

TS:   if (!x) {}
来源：http://uc.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jh.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nh.shxzukj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bc.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ha.asd995.cn

[A17] 位运算
来源：http://mw.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://io.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bl.9csxet.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bf.huixiangedu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wa.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qq.newstarts.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bp.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://id.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://or.shxzukj.cn

[A18] 字符与 ASCII 码互转
来源：http://xu.jianghongdianzi.cn

Py:   ord("A"); chr(65)
来源：http://cz.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://ly.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dt.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zi.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://qm.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://kq.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://mv.muxihuayi.cn

[A19] 交换两个变量
来源：http://io.bjjhwx.cn

Py:   a, b = b, a
来源：http://dm.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ae.huanxung.cn

JS:   [a, b] = [b, a];
来源：http://ug.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://mr.gzmigu.cn

Java: int t = a; a = b; b = t;
来源：http://wt.yuexingan06.cn

Go:   a, b = b, a
来源：http://ib.wgjwhj.cn

Ruby: a, b = b, a
来源：http://oi.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://vs.chemitech.net.cn

[A20] 读取标准输入
来源：http://xp.hnjuh.cn

Py:   name = input("请输入：")
来源：http://hb.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rq.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kb.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://yp.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://tw.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xx.shxzskj.cn

Ruby: gets.chomp
来源：http://gs.nicolike.cn

C#:   Console.ReadLine();
来源：http://qu.panjiajie.cn

[A21] 保留指定小数位输出
来源：http://vo.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://gn.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nr.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://dg.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://mp.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://dg.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://am.9csxet.cn

Ruby: format("%.2f", 3.14159)
来源：http://gc.newstarts.cn

C#:   3.14159.ToString("F2")
来源：http://ic.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://nx.9csxet.cn

Py:   len(s)
来源：http://rq.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ho.jctech888.com.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oy.yuntaijiaju.cn

TS:   s.length
来源：http://yr.huixiangedu.cn

Java: s.length()
来源：http://iv.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fp.colortex.cn

Ruby: s.length
来源：http://mz.521024.cn

C#:   s.Length
来源：http://yp.huixinmuqiang.cn

[A23] 大小写转换
来源：http://du.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jg.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ou.shxzukj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tk.bjjhwx.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nb.szxytkj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://on.chemitech.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uv.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pi.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pn.nszjky.cn

[A24] 去除首尾空白
来源：http://qq.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kz.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ec.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zg.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://de.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dw.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://hj.jianghongdianzi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cs.muxihuayi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://af.szsharing.cn

[A25] 字符串比较
来源：http://mh.521024.cn

Py:   s1 == s2; s1 != s2
来源：http://jm.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ek.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mr.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ke.hnjuh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ha.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ix.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kv.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ye.shxzukj.cn

[A26] 类型转换总览
来源：http://ob.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wp.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uj.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dq.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://co.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lj.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jd.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oj.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vt.panjiajie.cn

================================================================================
来源：http://nt.jctech888.com.cn

B. 流程控制
来源：http://iv.bookmarksfly.cn

================================================================================
来源：http://gb.521024.cn

[B01] 条件判断 if / else
来源：http://mb.shxzukj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lb.chemitech.net.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dk.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bx.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fb.huanxung.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iw.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://az.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qs.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://of.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://ce.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ym.lnxyls.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pz.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ma.wgjwhj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yv.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uh.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ph.lnxyls.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://il.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dp.bjjhwx.cn

[B03] switch / match / case
来源：http://dm.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cy.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sh.jctech888.com.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jc.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ww.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://as.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gt.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sz.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://py.hahajie.cn

[B04] for 计数循环
来源：http://kf.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://jg.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rk.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mx.hnjuh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hi.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wl.bookmarksfly.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yp.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://am.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tt.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://cw.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://zi.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wk.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wj.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kw.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qu.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xx.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://il.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ff.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://bf.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ce.bjjhwx.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://un.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jz.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jq.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uf.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wv.jianghongdianzi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cx.colortex.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nj.521024.cn

[B07] while 循环
来源：http://br.asd995.cn

Py:   while i < 10: i += 1
来源：http://fv.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hh.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://xr.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://wr.hahajie.cn

Java: while (i < 10) { i++; }
来源：http://tl.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dt.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://cg.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://um.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://jy.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://ec.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ku.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://pl.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://yo.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://oa.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lq.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kl.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://tz.muxihuayi.cn

[B09] break 与 continue
来源：http://ir.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gf.szxytkj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oc.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sg.muxihuayi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gz.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zt.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pt.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yy.huixiangedu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ps.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://oz.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rh.bookmarksfly.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://by.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gm.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ky.newstarts.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fs.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ny.bjjhwx.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hi.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://el.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://ha.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://ks.9csxet.cn

PHP:  range(0, 10, 2);
来源：http://rr.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yv.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mn.jctech888.com.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cg.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ol.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://ui.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xw.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://pe.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://uh.colortex.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yq.newstarts.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dm.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qt.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tj.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ne.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gn.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eu.huixiangedu.cn

[B13] 判断是否为数字
来源：http://mx.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://ug.shxzukj.cn

PHP:  is_numeric($x)
来源：http://ke.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bk.panjiajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qd.yuexingan06.cn

Java: x instanceof Number
来源：http://rd.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tl.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://oh.lnxyls.cn

C#:   x is int or double or decimal
来源：http://ue.yuntaijiaju.cn

[B14] 判断值是否在集合内
来源：http://cu.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://om.huixiangedu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://se.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://or.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://da.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://et.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cm.nszjky.cn

Ruby: [1, 2, 3].include?(x)
来源：http://al.haigaiapp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fo.newstarts.cn

[B15] 布尔运算与取反
来源：http://kg.nszjky.cn

Py:   a and b or not c
来源：http://dz.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://jl.yuntaijiaju.cn

JS:   a && b || !c
来源：http://nb.shxzukj.cn

TS:   a && b || !c
来源：http://jg.chemitech.net.cn

Java: a && b || !c
来源：http://vs.shxzskj.cn

Go:   a && b || !c
来源：http://sy.nszjky.cn

Ruby: a && b || !c
来源：http://fq.jianghongdianzi.cn

C#:   a && b || !c
来源：http://xw.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cg.yuntaijiaju.cn


<!-- 参考信息 -->