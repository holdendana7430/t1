代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ut.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wb.hahajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xb.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gb.szsharing.cn

[A10] 生成随机数
来源：http://ra.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://tv.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://ez.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bo.nicolike.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kt.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://nv.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ot.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://ob.jctech888.com.cn

C#:   new Random().Next(1, 101)
来源：http://gq.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://kn.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://tg.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ga.colortex.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fg.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mn.muxihuayi.cn

Java: x > 0 ? "yes" : "no"
来源：http://ye.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kn.bookmarksfly.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://gz.asd995.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bj.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://zm.huanxung.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://op.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fm.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://jk.yuntaijiaju.cn

TS:   `Hello, ${name}!`
来源：http://th.huixinmuqiang.cn

Java: "Hello, %s!".formatted(name)
来源：http://cn.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rg.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://pg.colortex.cn

C#:   $"Hello, {name}!"
来源：http://sp.nicolike.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xj.asd995.cn

Py:   "第一行\n第二行"
来源：http://jr.chemitech.net.cn

PHP:  "第一行\n第二行"
来源：http://co.colortex.cn

JS:   "第一行\n第二行"
来源：http://ss.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://uz.hahajie.cn

Java: "第一行\n第二行"
来源：http://qi.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://rx.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://mt.szsharing.cn

C#:   "第一行\n第二行"
来源：http://xh.wgjwhj.cn

[A14] 注释写法
来源：http://bc.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mm.huixiangedu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mq.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://cg.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://qv.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xr.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://vt.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ah.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://ja.hnjuh.cn

[A15] 空值判断与默认值
来源：http://lc.521024.cn

Py:   value = data or "默认值"
来源：http://af.bookmarksfly.cn

PHP:  $value = $data ?? "默认值";
来源：http://gi.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://oh.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://mu.muxihuayi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ao.muxihuayi.cn

Go:   if data == "" { data = "默认值" }
来源：http://fh.newstarts.cn

Ruby: value = data || "默认值"
来源：http://hs.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://xc.nszjky.cn

[A16] 真假值判断规则
来源：http://tw.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tl.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://en.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uw.gzmigu.cn

TS:   if (!x) {}
来源：http://za.muxihuayi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nj.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://od.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gy.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qo.hnjuh.cn

[A17] 位运算
来源：http://dc.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jh.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qv.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mr.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qx.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dh.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xs.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ms.colortex.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tv.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://sc.wgjwhj.cn

Py:   ord("A"); chr(65)
来源：http://ko.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://fl.panjiajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pu.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://it.bookmarksfly.cn

Java: (int) 'A'; (char) 65
来源：http://hf.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zq.asd995.cn

Ruby: "A".ord; 65.chr
来源：http://mm.wgjwhj.cn

C#:   (int)'A'; (char)65
来源：http://cd.yuntaijiaju.cn

[A19] 交换两个变量
来源：http://bm.hnjuh.cn

Py:   a, b = b, a
来源：http://xb.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fm.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://zy.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://kg.bjjhwx.cn

Java: int t = a; a = b; b = t;
来源：http://ml.muxihuayi.cn

Go:   a, b = b, a
来源：http://oq.shxzukj.cn

Ruby: a, b = b, a
来源：http://au.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://mq.huanxung.cn

[A20] 读取标准输入
来源：http://kx.newstarts.cn

Py:   name = input("请输入：")
来源：http://kg.521024.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jg.muxihuayi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tk.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://mq.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://dz.jianghongdianzi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bq.shxzskj.cn

Ruby: gets.chomp
来源：http://em.nszjky.cn

C#:   Console.ReadLine();
来源：http://cs.muxihuayi.cn

[A21] 保留指定小数位输出
来源：http://wd.haigaiapp.cn

Py:   f"{3.14159:.2f}"
来源：http://qd.huixinmuqiang.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rs.gzmigu.cn

JS:   (3.14159).toFixed(2)
来源：http://nc.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://vn.szxytkj.cn

Java: String.format("%.2f", 3.14159)
来源：http://ri.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oq.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://uy.hahajie.cn

C#:   3.14159.ToString("F2")
来源：http://ae.shxzskj.cn

[A22] 获取字符串长度
来源：http://tz.huixiangedu.cn

Py:   len(s)
来源：http://fc.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xd.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nq.jctech888.com.cn

TS:   s.length
来源：http://cs.muxihuayi.cn

Java: s.length()
来源：http://ij.nicolike.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yv.huanxung.cn

Ruby: s.length
来源：http://wo.yuntaijiaju.cn

C#:   s.Length
来源：http://mq.jctech888.com.cn

[A23] 大小写转换
来源：http://nf.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://de.huixiangedu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qa.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yq.huanxung.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cj.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://au.shxzukj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sv.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dj.9csxet.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://em.shtwfgs.cn

[A24] 去除首尾空白
来源：http://jl.chemitech.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uj.jianghongdianzi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cs.hahajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://av.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ij.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mv.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://mo.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ic.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xg.newstarts.cn

[A25] 字符串比较
来源：http://ba.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://nc.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xi.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hf.bookmarksfly.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zu.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://on.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ss.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://kq.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gi.lnxyls.cn

[A26] 类型转换总览
来源：http://vf.huixinmuqiang.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kk.muxihuayi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://da.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ov.shtwfgs.cn

TS:   Number() String() Boolean() x as number
来源：http://as.jctech888.com.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://av.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xk.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ik.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://at.shtwfgs.cn

================================================================================
来源：http://mr.yuntaijiaju.cn

B. 流程控制
来源：http://mu.huanxung.cn

================================================================================
来源：http://bx.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://fq.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://uo.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jc.lnxyls.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jb.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nv.9csxet.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qu.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ik.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://re.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hi.nszjky.cn

[B02] 多分支 else if / elif
来源：http://tl.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xv.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gt.gzmigu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xt.hahajie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dp.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uo.colortex.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nv.hnjuh.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ku.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mq.gzmigu.cn

[B03] switch / match / case
来源：http://fw.muxihuayi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xn.yuexingan06.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hl.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nj.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wv.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gy.jctech888.com.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qd.jctech888.com.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://im.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kt.shxzukj.cn

[B04] for 计数循环
来源：http://yn.521024.cn

Py:   for i in range(10): print(i)
来源：http://wv.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hq.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fl.shtwfgs.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ro.haigaiapp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wg.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://le.9csxet.cn

Ruby: 10.times { |i| puts i }
来源：http://zw.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ke.colortex.cn

[B05] 遍历数组 / 列表
来源：http://bh.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://io.haigaiapp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ev.lnxyls.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mh.shxzukj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rx.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://as.bjjhwx.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eo.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://mz.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dq.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://gb.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cc.asd995.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sh.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kb.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jm.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ta.asd995.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://go.szsharing.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xl.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pe.colortex.cn

[B07] while 循环
来源：http://fg.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://om.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kc.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://jb.huixinmuqiang.cn

TS:   while (i < 10) { i++; }
来源：http://su.asd995.cn

Java: while (i < 10) { i++; }
来源：http://hv.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bs.yuexingan06.cn

Ruby: while i < 10; i += 1; end
来源：http://ii.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://dn.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://tk.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://to.nicolike.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eq.szsharing.cn

JS:   do { i++; } while (i < 10);
来源：http://ga.jianghongdianzi.cn

TS:   do { i++; } while (i < 10);
来源：http://wf.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://ej.bjjhwx.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ir.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nr.chemitech.net.cn

C#:   do { i++; } while (i < 10);
来源：http://sh.panjiajie.cn

[B09] break 与 continue
来源：http://kh.huanxung.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sl.haigaiapp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yx.yuntaijiaju.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://om.bookmarksfly.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rf.chemitech.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://au.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lv.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fn.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jg.nszjky.cn

[B10] 遍历同时拿索引
来源：http://jc.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ea.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lg.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ux.yuntaijiaju.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://at.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yj.shxzukj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ny.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xq.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qj.521024.cn

[B11] 生成数字序列 / 区间
来源：http://yp.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://ke.szsharing.cn

PHP:  range(0, 10, 2);
来源：http://xr.yuntaijiaju.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ro.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ia.nicolike.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ij.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eg.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://hl.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hx.shtwfgs.cn

[B12] 跳出多层循环
来源：http://wx.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zp.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://oj.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sw.panjiajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wc.shxzskj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://it.haigaiapp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bf.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mr.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vu.hahajie.cn

[B13] 判断是否为数字
来源：http://zz.hnjuh.cn

Py:   isinstance(x, (int, float))
来源：http://ur.bookmarksfly.cn

PHP:  is_numeric($x)
来源：http://zh.shxzskj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gl.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mv.shtwfgs.cn

Java: x instanceof Number
来源：http://ya.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ac.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://il.huanxung.cn

C#:   x is int or double or decimal
来源：http://bn.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://ml.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pw.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zg.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://vs.nicolike.cn

TS:   [1, 2, 3].includes(x)
来源：http://qz.nszjky.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jp.nicolike.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fr.wgjwhj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kc.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://en.huanxung.cn

[B15] 布尔运算与取反
来源：http://co.muxihuayi.cn

Py:   a and b or not c
来源：http://ry.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://fu.bjjhwx.cn

JS:   a && b || !c
来源：http://xa.shxzukj.cn

TS:   a && b || !c
来源：http://re.muxihuayi.cn

Java: a && b || !c
来源：http://cs.bjjhwx.cn

Go:   a && b || !c
来源：http://qk.nicolike.cn

Ruby: a && b || !c
来源：http://fy.gzmigu.cn

C#:   a && b || !c
来源：http://qy.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fe.bjjhwx.cn

Py:   if not data: return
来源：http://ov.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://cj.szxytkj.cn

JS:   if (!data) return;
来源：http://zs.shtwfgs.cn

TS:   if (!data) return;
来源：http://nc.shxzskj.cn


<!-- 参考信息 -->