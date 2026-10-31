代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kb.haigaiapp.cn

Java: new Random().nextInt(100) + 1
来源：http://qb.9csxet.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jk.chemitech.net.cn

Ruby: rand(1..100)
来源：http://ae.asd995.cn

C#:   new Random().Next(1, 101)
来源：http://zu.nicolike.cn

[A11] 条件表达式（三元）
来源：http://fq.lnxyls.cn

Py:   "yes" if x > 0 else "no"
来源：http://dj.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vu.9csxet.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vn.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kh.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://kg.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hv.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jy.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pz.jctech888.com.cn

[A12] 字符串插值 / 格式化
来源：http://bx.shxzukj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ny.wgjwhj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hw.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://sf.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://jd.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://nm.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mg.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://mk.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://hk.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kt.colortex.cn

Py:   "第一行\n第二行"
来源：http://mw.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://jt.szsharing.cn

JS:   "第一行\n第二行"
来源：http://eu.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://eu.nicolike.cn

Java: "第一行\n第二行"
来源：http://po.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://da.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://pp.szxytkj.cn

C#:   "第一行\n第二行"
来源：http://xp.panjiajie.cn

[A14] 注释写法
来源：http://yz.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dq.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rn.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://ag.9csxet.cn

TS:   // 单行；/* 多行 */
来源：http://zd.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jr.hahajie.cn

Go:   // 单行；/* 多行 */
来源：http://xv.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wr.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://bl.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://gw.szsharing.cn

Py:   value = data or "默认值"
来源：http://zu.huixiangedu.cn

PHP:  $value = $data ?? "默认值";
来源：http://mz.panjiajie.cn

JS:   const value = data ?? "默认值";
来源：http://ka.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://fi.shxzskj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wn.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://zt.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://ic.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://ou.wgjwhj.cn

[A16] 真假值判断规则
来源：http://du.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hu.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wd.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bz.nszjky.cn

TS:   if (!x) {}
来源：http://iw.shxzskj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qa.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rs.muxihuayi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tp.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qu.muxihuayi.cn

[A17] 位运算
来源：http://zl.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gv.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cs.hnjuh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mz.asd995.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rs.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rb.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yr.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://og.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qg.asd995.cn

[A18] 字符与 ASCII 码互转
来源：http://yk.shtwfgs.cn

Py:   ord("A"); chr(65)
来源：http://ei.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://du.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xx.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://al.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://zv.nicolike.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xu.521024.cn

Ruby: "A".ord; 65.chr
来源：http://rh.yuntaijiaju.cn

C#:   (int)'A'; (char)65
来源：http://sj.newstarts.cn

[A19] 交换两个变量
来源：http://pi.haigaiapp.cn

Py:   a, b = b, a
来源：http://ch.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nw.521024.cn

JS:   [a, b] = [b, a];
来源：http://qo.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://sw.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://th.shxzukj.cn

Go:   a, b = b, a
来源：http://np.huanxung.cn

Ruby: a, b = b, a
来源：http://kh.jctech888.com.cn

C#:   (a, b) = (b, a);
来源：http://sl.shxzukj.cn

[A20] 读取标准输入
来源：http://mi.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://bg.jianghongdianzi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jn.jctech888.com.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uw.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://yb.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://fw.haigaiapp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qf.nszjky.cn

Ruby: gets.chomp
来源：http://ce.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://rp.nszjky.cn

[A21] 保留指定小数位输出
来源：http://ib.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://jn.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ep.bookmarksfly.cn

JS:   (3.14159).toFixed(2)
来源：http://gu.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://ry.yuexingan06.cn

Java: String.format("%.2f", 3.14159)
来源：http://tf.yuntaijiaju.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://av.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://ly.asd995.cn

C#:   3.14159.ToString("F2")
来源：http://ha.hnjuh.cn

[A22] 获取字符串长度
来源：http://oi.panjiajie.cn

Py:   len(s)
来源：http://rc.yuexingan06.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nt.9csxet.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lk.jianghongdianzi.cn

TS:   s.length
来源：http://uq.nszjky.cn

Java: s.length()
来源：http://kp.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ta.jianghongdianzi.cn

Ruby: s.length
来源：http://hl.szsharing.cn

C#:   s.Length
来源：http://gd.lnxyls.cn

[A23] 大小写转换
来源：http://yj.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wv.jianghongdianzi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://is.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gu.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sc.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://is.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xi.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vy.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wx.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://fg.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rw.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ds.yuntaijiaju.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wi.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aq.muxihuayi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yw.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://rv.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pp.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jn.bjjhwx.cn

[A25] 字符串比较
来源：http://zn.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://ju.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://td.jctech888.com.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yx.szxytkj.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zd.haigaiapp.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vs.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zf.panjiajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rt.jianghongdianzi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pz.nszjky.cn

[A26] 类型转换总览
来源：http://dp.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tz.asd995.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jn.shxzskj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rg.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://ns.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yv.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vo.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fp.shxzskj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mh.hahajie.cn

================================================================================
来源：http://qd.nicolike.cn

B. 流程控制
来源：http://le.hnjuh.cn

================================================================================
来源：http://uu.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://xa.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hh.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bk.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ff.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lm.hnjuh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ah.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jd.asd995.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sd.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fz.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://uv.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ue.huanxung.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tk.lnxyls.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tc.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zc.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ev.huixinmuqiang.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yf.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kt.szxytkj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qg.colortex.cn

[B03] switch / match / case
来源：http://zd.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xe.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xt.newstarts.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qb.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ft.9csxet.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oo.521024.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lj.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bz.9csxet.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fi.szxytkj.cn

[B04] for 计数循环
来源：http://ys.huanxung.cn

Py:   for i in range(10): print(i)
来源：http://bu.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://um.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rl.huixinmuqiang.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oa.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vj.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zo.haigaiapp.cn

Ruby: 10.times { |i| puts i }
来源：http://ds.hnjuh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qd.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://lg.yuexingan06.cn

Py:   for item in arr: print(item)
来源：http://le.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nf.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yv.wgjwhj.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zg.newstarts.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pf.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cd.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://vj.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ds.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://iv.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kx.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xd.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vh.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vg.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sf.hahajie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rb.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bv.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dp.asd995.cn

[B07] while 循环
来源：http://eh.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://mw.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://el.521024.cn

JS:   while (i < 10) { i++; }
来源：http://mm.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://rt.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://pw.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qi.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://qq.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://uc.shxzukj.cn

[B08] do-while（至少执行一次）
来源：http://ri.521024.cn

Py:   # 无 do-while：用 while True + break
来源：http://bu.haigaiapp.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://an.szxytkj.cn

JS:   do { i++; } while (i < 10);
来源：http://mw.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://yw.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://eg.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yh.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lu.lnxyls.cn

C#:   do { i++; } while (i < 10);
来源：http://yi.yuntaijiaju.cn

[B09] break 与 continue
来源：http://uf.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zv.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://aj.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ao.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lj.lnxyls.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://li.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://um.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://km.chemitech.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zc.newstarts.cn

[B10] 遍历同时拿索引
来源：http://ji.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ci.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pt.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zv.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tn.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hw.shxzskj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xo.9csxet.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ze.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gb.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://uz.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://fq.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://wb.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mh.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ht.haigaiapp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tq.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zp.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://bn.nicolike.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fq.nszjky.cn

[B12] 跳出多层循环
来源：http://nv.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rh.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://up.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ku.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sy.shtwfgs.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://py.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://me.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sn.wgjwhj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dp.hnjuh.cn

[B13] 判断是否为数字
来源：http://bk.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://uj.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://my.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hd.521024.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ps.hahajie.cn

Java: x instanceof Number
来源：http://pb.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dv.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://ic.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://mu.colortex.cn

[B14] 判断值是否在集合内
来源：http://zu.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ih.nszjky.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yg.shxzukj.cn

JS:   [1, 2, 3].includes(x)
来源：http://vx.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://fu.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ow.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fp.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vn.huixiangedu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oh.asd995.cn

[B15] 布尔运算与取反
来源：http://sw.wgjwhj.cn

Py:   a and b or not c
来源：http://bu.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://fy.9csxet.cn

JS:   a && b || !c
来源：http://pn.nicolike.cn

TS:   a && b || !c
来源：http://io.nszjky.cn

Java: a && b || !c
来源：http://dp.jianghongdianzi.cn

Go:   a && b || !c
来源：http://op.haigaiapp.cn

Ruby: a && b || !c
来源：http://xo.huanxung.cn

C#:   a && b || !c
来源：http://lm.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://po.521024.cn

Py:   if not data: return
来源：http://bp.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://jv.wgjwhj.cn

JS:   if (!data) return;
来源：http://jp.jctech888.com.cn

TS:   if (!data) return;
来源：http://cs.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://ay.yuntaijiaju.cn

Go:   if data == nil { return }
来源：http://sh.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://pp.shtwfgs.cn

C#:   if (data == null) return;
来源：http://qn.huanxung.cn

================================================================================
来源：http://wm.9csxet.cn

C. 函数与作用域
来源：http://yv.shtwfgs.cn

================================================================================
来源：http://su.asd995.cn

[C01] 定义函数
来源：http://pz.shtwfgs.cn


<!-- 参考信息 -->