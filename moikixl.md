代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ca.gzmigu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cy.asd995.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jp.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jj.chemitech.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hf.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://at.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yq.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://qi.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wx.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dr.hnjuh.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xb.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tu.panjiajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bd.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xd.jianghongdianzi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://aa.yuexingan06.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mj.shxzskj.cn

[A10] 生成随机数
来源：http://wc.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://wj.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://zf.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bv.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fe.muxihuayi.cn

Java: new Random().nextInt(100) + 1
来源：http://gn.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zq.haigaiapp.cn

Ruby: rand(1..100)
来源：http://vk.shtwfgs.cn

C#:   new Random().Next(1, 101)
来源：http://cp.nicolike.cn

[A11] 条件表达式（三元）
来源：http://ic.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://mw.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fd.panjiajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://os.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mh.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://gu.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nb.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tv.hnjuh.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vh.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://xl.chemitech.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tp.gzmigu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cg.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://zd.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://ko.muxihuayi.cn

Java: "Hello, %s!".formatted(name)
来源：http://kz.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vv.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://aa.bookmarksfly.cn

C#:   $"Hello, {name}!"
来源：http://uq.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hq.panjiajie.cn

Py:   "第一行\n第二行"
来源：http://xw.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://hj.nszjky.cn

JS:   "第一行\n第二行"
来源：http://tt.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://hf.newstarts.cn

Java: "第一行\n第二行"
来源：http://kp.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://sw.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://hr.shxzukj.cn

C#:   "第一行\n第二行"
来源：http://jk.szsharing.cn

[A14] 注释写法
来源：http://fy.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vl.shxzukj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nm.haigaiapp.cn

JS:   // 单行；/* 多行 */
来源：http://uo.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://mo.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ha.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://ul.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xl.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://az.nicolike.cn

[A15] 空值判断与默认值
来源：http://il.jctech888.com.cn

Py:   value = data or "默认值"
来源：http://qq.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://em.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://eo.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://lf.nicolike.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ls.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://pf.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://eq.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://zb.shxzskj.cn

[A16] 真假值判断规则
来源：http://vy.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dn.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mq.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sz.jctech888.com.cn

TS:   if (!x) {}
来源：http://fw.521024.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oj.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gs.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ku.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jg.colortex.cn

[A17] 位运算
来源：http://mr.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://re.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qs.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ut.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jp.gzmigu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jy.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vd.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jf.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cl.hnjuh.cn

[A18] 字符与 ASCII 码互转
来源：http://hw.521024.cn

Py:   ord("A"); chr(65)
来源：http://un.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://ht.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://go.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://us.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://tc.huixinmuqiang.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qq.hahajie.cn

Ruby: "A".ord; 65.chr
来源：http://xm.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://lw.nicolike.cn

[A19] 交换两个变量
来源：http://ip.521024.cn

Py:   a, b = b, a
来源：http://fm.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ic.9csxet.cn

JS:   [a, b] = [b, a];
来源：http://kb.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://nv.colortex.cn

Java: int t = a; a = b; b = t;
来源：http://om.huixiangedu.cn

Go:   a, b = b, a
来源：http://ja.chemitech.net.cn

Ruby: a, b = b, a
来源：http://nd.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://sr.gzmigu.cn

[A20] 读取标准输入
来源：http://pe.521024.cn

Py:   name = input("请输入：")
来源：http://tp.shxzukj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ez.9csxet.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lm.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://om.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://nk.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fi.521024.cn

Ruby: gets.chomp
来源：http://ly.bookmarksfly.cn

C#:   Console.ReadLine();
来源：http://sq.szsharing.cn

[A21] 保留指定小数位输出
来源：http://kj.muxihuayi.cn

Py:   f"{3.14159:.2f}"
来源：http://ao.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qe.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://ms.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://mj.huixiangedu.cn

Java: String.format("%.2f", 3.14159)
来源：http://rb.panjiajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gm.shxzskj.cn

Ruby: format("%.2f", 3.14159)
来源：http://xf.huanxung.cn

C#:   3.14159.ToString("F2")
来源：http://ve.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://rz.lnxyls.cn

Py:   len(s)
来源：http://iq.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xt.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pz.haigaiapp.cn

TS:   s.length
来源：http://gg.huanxung.cn

Java: s.length()
来源：http://na.yuexingan06.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gq.newstarts.cn

Ruby: s.length
来源：http://ei.huixiangedu.cn

C#:   s.Length
来源：http://at.nicolike.cn

[A23] 大小写转换
来源：http://wu.gzmigu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lm.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tu.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bw.yuntaijiaju.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bn.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fx.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ym.bookmarksfly.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ni.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bm.szxytkj.cn

[A24] 去除首尾空白
来源：http://ki.bjjhwx.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ub.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dm.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ek.asd995.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yq.jctech888.com.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cw.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://ng.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mj.jctech888.com.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kh.chemitech.net.cn

[A25] 字符串比较
来源：http://ch.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://us.shxzukj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bc.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xt.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ca.wgjwhj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wx.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hw.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nc.newstarts.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gl.szsharing.cn

[A26] 类型转换总览
来源：http://cg.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rl.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ta.haigaiapp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hc.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://ye.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kr.lnxyls.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xs.nicolike.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hn.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ri.lnxyls.cn

================================================================================
来源：http://rg.hnjuh.cn

B. 流程控制
来源：http://aw.shxzukj.cn

================================================================================
来源：http://bs.szsharing.cn

[B01] 条件判断 if / else
来源：http://hq.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jt.wgjwhj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tt.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ri.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ff.nicolike.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://na.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dp.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://of.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kj.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://wq.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uh.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zk.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pd.huixiangedu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://as.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xt.yuntaijiaju.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vi.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bd.huixiangedu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tx.hnjuh.cn

[B03] switch / match / case
来源：http://ee.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uf.jianghongdianzi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ub.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pd.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ji.jctech888.com.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jt.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ot.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fu.gzmigu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cw.colortex.cn

[B04] for 计数循环
来源：http://tc.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://py.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rl.jianghongdianzi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jd.bookmarksfly.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rg.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wd.lnxyls.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ke.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://bm.wgjwhj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tm.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://od.jianghongdianzi.cn

Py:   for item in arr: print(item)
来源：http://db.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ls.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ka.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cc.szsharing.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jn.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qe.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://hg.huanxung.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://np.huanxung.cn

[B06] 遍历字典 / 对象
来源：http://sn.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bo.muxihuayi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://na.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yj.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fd.521024.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ej.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://be.asd995.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mz.huixinmuqiang.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wd.gzmigu.cn

[B07] while 循环
来源：http://fu.521024.cn

Py:   while i < 10: i += 1
来源：http://vd.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://is.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://hw.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://al.colortex.cn

Java: while (i < 10) { i++; }
来源：http://jx.haigaiapp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ze.lnxyls.cn

Ruby: while i < 10; i += 1; end
来源：http://ax.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://mh.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://bg.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://ap.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ka.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://sx.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://fm.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://pg.huixinmuqiang.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://py.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zy.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://qv.szxytkj.cn

[B09] break 与 continue
来源：http://ug.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hy.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dd.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pt.newstarts.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gh.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yb.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bz.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wx.bjjhwx.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wc.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://wy.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://el.nszjky.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wb.jianghongdianzi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sg.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pd.muxihuayi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lc.jianghongdianzi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jy.muxihuayi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://by.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tl.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://vg.521024.cn

Py:   list(range(0, 10, 2))
来源：http://ng.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://jd.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mv.muxihuayi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tv.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://og.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sj.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://tk.szxytkj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oe.asd995.cn

[B12] 跳出多层循环
来源：http://dq.shxzskj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xm.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yc.szxytkj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zb.muxihuayi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zi.nicolike.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kl.newstarts.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fy.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ee.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hi.colortex.cn

[B13] 判断是否为数字
来源：http://io.asd995.cn

Py:   isinstance(x, (int, float))
来源：http://tk.hnjuh.cn

PHP:  is_numeric($x)
来源：http://jq.bookmarksfly.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pw.hahajie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rb.szsharing.cn

Java: x instanceof Number
来源：http://wp.lnxyls.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yn.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://nn.szsharing.cn

C#:   x is int or double or decimal
来源：http://yg.hahajie.cn

[B14] 判断值是否在集合内
来源：http://ox.huixiangedu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yo.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xc.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://um.szxytkj.cn

TS:   [1, 2, 3].includes(x)
来源：http://ro.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ji.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://py.colortex.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qf.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bs.nicolike.cn

[B15] 布尔运算与取反
来源：http://ug.jctech888.com.cn

Py:   a and b or not c
来源：http://zr.huixinmuqiang.cn


<!-- 参考信息 -->