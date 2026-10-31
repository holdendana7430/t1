代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tf.bjjhwx.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://my.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lk.521024.cn

[A09] 绝对值与最大最小值
来源：http://rb.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://eh.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wf.9csxet.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pp.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cc.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zn.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dt.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://aa.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gr.jianghongdianzi.cn

[A10] 生成随机数
来源：http://hh.shxzukj.cn

Py:   import random; random.randint(1, 100)
来源：http://bs.jctech888.com.cn

PHP:  random_int(1, 100);
来源：http://lu.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ss.bookmarksfly.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ln.huixiangedu.cn

Java: new Random().nextInt(100) + 1
来源：http://tl.bjjhwx.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cy.gzmigu.cn

Ruby: rand(1..100)
来源：http://zm.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://mq.colortex.cn

[A11] 条件表达式（三元）
来源：http://hl.muxihuayi.cn

Py:   "yes" if x > 0 else "no"
来源：http://lz.muxihuayi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://to.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xb.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ss.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://dm.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ix.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jl.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yi.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://pp.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xo.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pb.jianghongdianzi.cn

JS:   `Hello, ${name}!`
来源：http://vg.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://rj.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://yt.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ue.panjiajie.cn

Ruby: "Hello, #{name}!"
来源：http://qz.lnxyls.cn

C#:   $"Hello, {name}!"
来源：http://ol.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ab.yuntaijiaju.cn

Py:   "第一行\n第二行"
来源：http://mw.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://ai.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://lu.shxzskj.cn

TS:   "第一行\n第二行"
来源：http://ix.szsharing.cn

Java: "第一行\n第二行"
来源：http://xh.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://iz.asd995.cn

Ruby: "第一行\n第二行"
来源：http://nn.hahajie.cn

C#:   "第一行\n第二行"
来源：http://im.521024.cn

[A14] 注释写法
来源：http://ga.shxzskj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fb.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://aq.521024.cn

JS:   // 单行；/* 多行 */
来源：http://tp.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://fv.newstarts.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lj.colortex.cn

Go:   // 单行；/* 多行 */
来源：http://ph.bjjhwx.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ip.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://ce.shxzskj.cn

[A15] 空值判断与默认值
来源：http://vm.hnjuh.cn

Py:   value = data or "默认值"
来源：http://in.szxytkj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ue.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://yg.szsharing.cn

TS:   const value = data ?? "默认值";
来源：http://dh.hahajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wx.colortex.cn

Go:   if data == "" { data = "默认值" }
来源：http://ja.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://nj.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://uj.9csxet.cn

[A16] 真假值判断规则
来源：http://gb.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://us.chemitech.net.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mq.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ph.haigaiapp.cn

TS:   if (!x) {}
来源：http://kg.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tc.lnxyls.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hy.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bg.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pl.szsharing.cn

[A17] 位运算
来源：http://kj.521024.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ab.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kb.nszjky.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://de.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xj.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ki.huixiangedu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oi.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xc.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cx.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://gy.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://pe.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://tr.shxzskj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gw.yuntaijiaju.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fl.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://zo.haigaiapp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kw.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://un.521024.cn

C#:   (int)'A'; (char)65
来源：http://mw.lnxyls.cn

[A19] 交换两个变量
来源：http://jl.yuexingan06.cn

Py:   a, b = b, a
来源：http://qj.shxzskj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wk.huixiangedu.cn

JS:   [a, b] = [b, a];
来源：http://jr.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://yi.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://lr.bjjhwx.cn

Go:   a, b = b, a
来源：http://hw.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://ek.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://wb.nicolike.cn

[A20] 读取标准输入
来源：http://ee.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://rb.chemitech.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dk.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wy.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://vm.hahajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://od.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zr.muxihuayi.cn

Ruby: gets.chomp
来源：http://ed.9csxet.cn

C#:   Console.ReadLine();
来源：http://ub.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://vc.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://aq.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ir.nicolike.cn

JS:   (3.14159).toFixed(2)
来源：http://kp.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://ik.huixinmuqiang.cn

Java: String.format("%.2f", 3.14159)
来源：http://sm.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rf.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://sv.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://gw.haigaiapp.cn

[A22] 获取字符串长度
来源：http://cb.bookmarksfly.cn

Py:   len(s)
来源：http://gk.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zo.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bj.wgjwhj.cn

TS:   s.length
来源：http://wx.szsharing.cn

Java: s.length()
来源：http://oi.bookmarksfly.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://io.lnxyls.cn

Ruby: s.length
来源：http://vf.bookmarksfly.cn

C#:   s.Length
来源：http://zj.asd995.cn

[A23] 大小写转换
来源：http://hs.9csxet.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://yg.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jl.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cu.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lk.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wj.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wt.haigaiapp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://od.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sm.bookmarksfly.cn

[A24] 去除首尾空白
来源：http://lf.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xy.nicolike.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mz.shtwfgs.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dg.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bm.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://re.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://og.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dq.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cp.yuexingan06.cn

[A25] 字符串比较
来源：http://mf.shtwfgs.cn

Py:   s1 == s2; s1 != s2
来源：http://du.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jh.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ez.nszjky.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xt.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eh.jianghongdianzi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pm.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dy.hnjuh.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iv.lnxyls.cn

[A26] 类型转换总览
来源：http://dc.shtwfgs.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bv.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kk.nicolike.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zi.wgjwhj.cn

TS:   Number() String() Boolean() x as number
来源：http://id.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yo.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rc.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://im.shtwfgs.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gc.colortex.cn

================================================================================
来源：http://vi.asd995.cn

B. 流程控制
来源：http://de.chemitech.net.cn

================================================================================
来源：http://zd.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://mz.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ka.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lr.newstarts.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ox.muxihuayi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xh.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ei.shxzukj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jw.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hl.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dh.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://yg.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xx.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hl.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hq.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cj.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fv.haigaiapp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vm.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://us.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ef.huanxung.cn

[B03] switch / match / case
来源：http://qc.wgjwhj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nb.nicolike.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zc.gzmigu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gf.521024.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ei.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zr.gzmigu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jc.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tu.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rk.nszjky.cn

[B04] for 计数循环
来源：http://fm.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://yk.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://po.9csxet.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ss.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hi.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gg.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://py.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://aj.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yk.nicolike.cn

[B05] 遍历数组 / 列表
来源：http://ku.muxihuayi.cn

Py:   for item in arr: print(item)
来源：http://sw.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gs.jianghongdianzi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://px.nszjky.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://et.9csxet.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ts.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uv.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://mn.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zg.panjiajie.cn

[B06] 遍历字典 / 对象
来源：http://zg.nicolike.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bu.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zo.bjjhwx.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ct.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ns.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://me.yuexingan06.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ik.521024.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://id.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mk.chemitech.net.cn

[B07] while 循环
来源：http://xq.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://lp.jctech888.com.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lx.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://hm.nszjky.cn

TS:   while (i < 10) { i++; }
来源：http://bh.chemitech.net.cn

Java: while (i < 10) { i++; }
来源：http://dh.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tz.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://ij.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://pp.hahajie.cn

[B08] do-while（至少执行一次）
来源：http://mw.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://hp.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wu.nicolike.cn

JS:   do { i++; } while (i < 10);
来源：http://ys.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://fe.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://wc.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nf.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gk.huanxung.cn

C#:   do { i++; } while (i < 10);
来源：http://km.nicolike.cn

[B09] break 与 continue
来源：http://xu.nszjky.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rz.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xn.wgjwhj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ph.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xi.shxzskj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ip.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lo.lnxyls.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ih.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://or.szxytkj.cn

[B10] 遍历同时拿索引
来源：http://au.jianghongdianzi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ag.9csxet.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wx.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kr.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://us.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cq.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pj.jctech888.com.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dp.9csxet.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gz.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://no.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://hx.bjjhwx.cn

PHP:  range(0, 10, 2);
来源：http://he.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dx.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lr.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yk.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gl.521024.cn

Ruby: (0...10).step(2).to_a
来源：http://fs.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yq.jianghongdianzi.cn

[B12] 跳出多层循环
来源：http://la.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ve.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qk.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yh.shtwfgs.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oq.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gd.9csxet.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jd.wgjwhj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://um.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tj.shxzskj.cn

[B13] 判断是否为数字
来源：http://za.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://ku.9csxet.cn

PHP:  is_numeric($x)
来源：http://ut.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bv.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qs.wgjwhj.cn

Java: x instanceof Number
来源：http://pw.muxihuayi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ul.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://op.asd995.cn

C#:   x is int or double or decimal
来源：http://jx.colortex.cn

[B14] 判断值是否在集合内
来源：http://jo.jianghongdianzi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mv.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://if.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://fc.huanxung.cn

TS:   [1, 2, 3].includes(x)
来源：http://ob.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://km.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ih.nicolike.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bi.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yu.bjjhwx.cn

[B15] 布尔运算与取反
来源：http://uw.huanxung.cn

Py:   a and b or not c
来源：http://zs.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://ia.szxytkj.cn

JS:   a && b || !c
来源：http://xn.wgjwhj.cn

TS:   a && b || !c
来源：http://nq.asd995.cn

Java: a && b || !c
来源：http://cz.jianghongdianzi.cn


<!-- 参考信息 -->