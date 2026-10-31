代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://al.nicolike.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qb.shtwfgs.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://de.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zq.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uh.wgjwhj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fh.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ap.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mr.521024.cn

[A10] 生成随机数
来源：http://zj.muxihuayi.cn

Py:   import random; random.randint(1, 100)
来源：http://kq.yuntaijiaju.cn

PHP:  random_int(1, 100);
来源：http://md.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kn.szxytkj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cg.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://rr.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fo.chemitech.net.cn

Ruby: rand(1..100)
来源：http://cf.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://ev.hahajie.cn

[A11] 条件表达式（三元）
来源：http://fa.521024.cn

Py:   "yes" if x > 0 else "no"
来源：http://ip.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://en.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hm.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cm.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://wh.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vs.bookmarksfly.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://uf.nszjky.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rx.panjiajie.cn

[A12] 字符串插值 / 格式化
来源：http://if.chemitech.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mx.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lt.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://pm.huixiangedu.cn

TS:   `Hello, ${name}!`
来源：http://ug.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://gm.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rs.hnjuh.cn

Ruby: "Hello, #{name}!"
来源：http://ct.chemitech.net.cn

C#:   $"Hello, {name}!"
来源：http://td.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ik.szxytkj.cn

Py:   "第一行\n第二行"
来源：http://wc.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://jo.colortex.cn

JS:   "第一行\n第二行"
来源：http://jf.hnjuh.cn

TS:   "第一行\n第二行"
来源：http://pt.colortex.cn

Java: "第一行\n第二行"
来源：http://vy.colortex.cn

Go:   "第一行\n第二行"
来源：http://vf.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://bk.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://hf.szxytkj.cn

[A14] 注释写法
来源：http://wi.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dy.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jj.lnxyls.cn

JS:   // 单行；/* 多行 */
来源：http://cn.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://ia.9csxet.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jt.jctech888.com.cn

Go:   // 单行；/* 多行 */
来源：http://it.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://on.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://mf.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://ef.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://hx.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://sz.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://lj.jianghongdianzi.cn

TS:   const value = data ?? "默认值";
来源：http://rn.9csxet.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pz.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://nh.hahajie.cn

Ruby: value = data || "默认值"
来源：http://jf.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://bs.wgjwhj.cn

[A16] 真假值判断规则
来源：http://fk.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fp.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ey.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kt.huixiangedu.cn

TS:   if (!x) {}
来源：http://tk.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fz.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zj.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://um.hnjuh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qs.hnjuh.cn

[A17] 位运算
来源：http://ro.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ab.nszjky.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fm.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ik.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://td.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ib.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yh.bookmarksfly.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zh.wgjwhj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cy.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://hh.bookmarksfly.cn

Py:   ord("A"); chr(65)
来源：http://bb.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://jl.bjjhwx.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://am.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rm.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://fu.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://os.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://sz.muxihuayi.cn

C#:   (int)'A'; (char)65
来源：http://xi.jianghongdianzi.cn

[A19] 交换两个变量
来源：http://tt.huixinmuqiang.cn

Py:   a, b = b, a
来源：http://st.bjjhwx.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://it.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://iw.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://ir.asd995.cn

Java: int t = a; a = b; b = t;
来源：http://jb.huixiangedu.cn

Go:   a, b = b, a
来源：http://uc.521024.cn

Ruby: a, b = b, a
来源：http://ek.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://eo.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://gw.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://zu.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://js.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qf.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://nx.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://lj.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fw.newstarts.cn

Ruby: gets.chomp
来源：http://ni.9csxet.cn

C#:   Console.ReadLine();
来源：http://im.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://ln.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://wf.521024.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ib.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://ew.newstarts.cn

TS:   (3.14159).toFixed(2)
来源：http://xr.shxzukj.cn

Java: String.format("%.2f", 3.14159)
来源：http://jt.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://au.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://qp.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://kt.bjjhwx.cn

[A22] 获取字符串长度
来源：http://rj.shtwfgs.cn

Py:   len(s)
来源：http://qw.nicolike.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ae.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wx.colortex.cn

TS:   s.length
来源：http://eh.szsharing.cn

Java: s.length()
来源：http://ci.shtwfgs.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ct.nicolike.cn

Ruby: s.length
来源：http://mb.panjiajie.cn

C#:   s.Length
来源：http://lp.521024.cn

[A23] 大小写转换
来源：http://fz.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vx.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yd.colortex.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qj.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lo.lnxyls.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bw.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kt.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hl.hnjuh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://re.hnjuh.cn

[A24] 去除首尾空白
来源：http://zx.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ne.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fx.asd995.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ko.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mm.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pf.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://kj.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ik.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://px.hahajie.cn

[A25] 字符串比较
来源：http://pa.bjjhwx.cn

Py:   s1 == s2; s1 != s2
来源：http://cu.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wl.gzmigu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rh.asd995.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xj.521024.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ii.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xx.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://by.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rw.muxihuayi.cn

[A26] 类型转换总览
来源：http://cr.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cp.chemitech.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eg.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oz.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://sz.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nx.huixiangedu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mr.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://js.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ep.wgjwhj.cn

================================================================================
来源：http://qn.haigaiapp.cn

B. 流程控制
来源：http://yf.bookmarksfly.cn

================================================================================
来源：http://ew.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://wk.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fr.yuexingan06.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lf.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://at.nicolike.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nu.hahajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ls.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kg.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aw.szxytkj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://me.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://ly.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://he.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sz.shxzskj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zf.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aj.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zo.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eb.hahajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vc.colortex.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cp.hnjuh.cn

[B03] switch / match / case
来源：http://ci.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bp.chemitech.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ur.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rk.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://un.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vr.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tz.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sz.colortex.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vk.panjiajie.cn

[B04] for 计数循环
来源：http://lv.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://ju.jianghongdianzi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://py.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rp.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://db.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ga.szxytkj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://py.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://ou.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nn.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://qb.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://br.jctech888.com.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mu.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yo.hahajie.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dk.yuntaijiaju.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lt.521024.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hi.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://jx.huixinmuqiang.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mf.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://vb.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pn.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oi.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vr.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jk.bjjhwx.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ja.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dj.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cr.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dj.hnjuh.cn

[B07] while 循环
来源：http://rt.wgjwhj.cn

Py:   while i < 10: i += 1
来源：http://ug.colortex.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ow.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://yu.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://ft.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://sh.hahajie.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pd.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://gj.colortex.cn

C#:   while (i < 10) { i++; }
来源：http://ea.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://ge.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://cq.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://mc.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://ky.muxihuayi.cn

TS:   do { i++; } while (i < 10);
来源：http://ij.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://aq.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fq.jctech888.com.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qh.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://xg.wgjwhj.cn

[B09] break 与 continue
来源：http://sh.shxzukj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://al.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ob.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pf.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ey.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kx.bookmarksfly.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vv.nszjky.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pq.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rv.9csxet.cn

[B10] 遍历同时拿索引
来源：http://ay.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nh.chemitech.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ox.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rn.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mb.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ce.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qb.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ag.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jq.haigaiapp.cn

[B11] 生成数字序列 / 区间
来源：http://ry.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://ys.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://sp.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wd.lnxyls.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tv.shtwfgs.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ki.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lr.yuntaijiaju.cn

Ruby: (0...10).step(2).to_a
来源：http://bb.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://un.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://ss.newstarts.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nl.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rm.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uf.huixinmuqiang.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tw.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://so.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dt.yuexingan06.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mr.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://et.muxihuayi.cn

[B13] 判断是否为数字
来源：http://nq.chemitech.net.cn

Py:   isinstance(x, (int, float))
来源：http://gh.huixinmuqiang.cn

PHP:  is_numeric($x)
来源：http://de.panjiajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sq.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ok.gzmigu.cn

Java: x instanceof Number
来源：http://lg.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gq.shxzskj.cn

Ruby: x.is_a?(Numeric)
来源：http://zo.bjjhwx.cn

C#:   x is int or double or decimal
来源：http://av.asd995.cn

[B14] 判断值是否在集合内
来源：http://rs.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oj.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gh.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://co.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://rr.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ny.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ht.gzmigu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lt.shxzskj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vj.huixinmuqiang.cn

[B15] 布尔运算与取反
来源：http://tr.jctech888.com.cn

Py:   a and b or not c
来源：http://po.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://yq.muxihuayi.cn

JS:   a && b || !c
来源：http://yh.szsharing.cn

TS:   a && b || !c
来源：http://ub.szsharing.cn

Java: a && b || !c
来源：http://rx.szsharing.cn

Go:   a && b || !c
来源：http://qe.panjiajie.cn

Ruby: a && b || !c
来源：http://ll.wgjwhj.cn

C#:   a && b || !c
来源：http://wi.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mx.panjiajie.cn


<!-- 参考信息 -->