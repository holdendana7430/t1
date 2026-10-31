代发 wailian999

[A10] 生成随机数
来源：http://jj.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://kx.szsharing.cn

PHP:  random_int(1, 100);
来源：http://dk.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yn.hahajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fa.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://gj.shxzskj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bm.yuexingan06.cn

Ruby: rand(1..100)
来源：http://ko.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://br.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://tc.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://ge.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://mc.521024.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hy.521024.cn

TS:   x > 0 ? "yes" : "no"
来源：http://na.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://ug.yuntaijiaju.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://oj.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ze.hahajie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fv.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://ey.nicolike.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xn.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cg.nicolike.cn

JS:   `Hello, ${name}!`
来源：http://wz.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://ws.huixinmuqiang.cn

Java: "Hello, %s!".formatted(name)
来源：http://my.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lw.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://vp.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://kj.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bz.shxzskj.cn

Py:   "第一行\n第二行"
来源：http://np.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://dr.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://vf.jctech888.com.cn

TS:   "第一行\n第二行"
来源：http://yq.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://cz.521024.cn

Go:   "第一行\n第二行"
来源：http://bw.newstarts.cn

Ruby: "第一行\n第二行"
来源：http://ow.shtwfgs.cn

C#:   "第一行\n第二行"
来源：http://ul.shxzukj.cn

[A14] 注释写法
来源：http://kw.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://iv.wgjwhj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xv.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://zk.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://my.newstarts.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nj.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://lf.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://co.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://tm.bookmarksfly.cn

[A15] 空值判断与默认值
来源：http://xx.szxytkj.cn

Py:   value = data or "默认值"
来源：http://la.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://xd.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://wn.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://qm.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wo.huixinmuqiang.cn

Go:   if data == "" { data = "默认值" }
来源：http://wi.colortex.cn

Ruby: value = data || "默认值"
来源：http://qt.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://vy.yuexingan06.cn

[A16] 真假值判断规则
来源：http://aw.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bv.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uw.huixiangedu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gd.haigaiapp.cn

TS:   if (!x) {}
来源：http://xr.jctech888.com.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fv.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ta.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://td.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cd.bjjhwx.cn

[A17] 位运算
来源：http://sh.bjjhwx.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dl.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eo.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.panjiajie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wd.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bu.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ad.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sr.9csxet.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ul.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://tb.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://qx.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://da.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nf.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bs.huixinmuqiang.cn

Java: (int) 'A'; (char) 65
来源：http://pv.newstarts.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rm.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://yu.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://ra.bjjhwx.cn

[A19] 交换两个变量
来源：http://ip.shxzskj.cn

Py:   a, b = b, a
来源：http://zu.haigaiapp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ie.shtwfgs.cn

JS:   [a, b] = [b, a];
来源：http://kx.9csxet.cn

TS:   [a, b] = [b, a];
来源：http://tl.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://fb.haigaiapp.cn

Go:   a, b = b, a
来源：http://fq.szxytkj.cn

Ruby: a, b = b, a
来源：http://ik.colortex.cn

C#:   (a, b) = (b, a);
来源：http://wx.asd995.cn

[A20] 读取标准输入
来源：http://tx.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://wq.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ay.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wy.colortex.cn

TS:   // Node.js：readline 模块
来源：http://le.chemitech.net.cn

Java: new Scanner(System.in).nextLine()
来源：http://zn.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bu.newstarts.cn

Ruby: gets.chomp
来源：http://mx.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://tr.yuntaijiaju.cn

[A21] 保留指定小数位输出
来源：http://gx.shtwfgs.cn

Py:   f"{3.14159:.2f}"
来源：http://wn.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wj.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://cz.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://ur.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://hn.jctech888.com.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mo.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://xo.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://aq.haigaiapp.cn

[A22] 获取字符串长度
来源：http://us.gzmigu.cn

Py:   len(s)
来源：http://mi.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tz.521024.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yb.hnjuh.cn

TS:   s.length
来源：http://li.huanxung.cn

Java: s.length()
来源：http://bv.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uk.hnjuh.cn

Ruby: s.length
来源：http://ly.newstarts.cn

C#:   s.Length
来源：http://dc.yuexingan06.cn

[A23] 大小写转换
来源：http://nl.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pf.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://be.bjjhwx.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ut.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bf.huixinmuqiang.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xq.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zu.bjjhwx.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pv.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://nn.asd995.cn

[A24] 去除首尾空白
来源：http://qd.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mk.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mp.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ip.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://co.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jx.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://hh.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gd.yuexingan06.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gz.jianghongdianzi.cn

[A25] 字符串比较
来源：http://fy.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://cg.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zc.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jf.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pk.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gr.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pk.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xv.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cg.asd995.cn

[A26] 类型转换总览
来源：http://ia.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tv.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ls.nszjky.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eo.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://cz.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tq.huixinmuqiang.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zk.hahajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vv.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hm.newstarts.cn

================================================================================
来源：http://mi.huixinmuqiang.cn

B. 流程控制
来源：http://ct.jianghongdianzi.cn

================================================================================
来源：http://ht.jctech888.com.cn

[B01] 条件判断 if / else
来源：http://cg.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rh.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ja.521024.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ld.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://df.haigaiapp.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tm.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hi.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tb.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ik.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://tl.hahajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gx.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sp.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xf.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kl.yuntaijiaju.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wz.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qv.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rp.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hc.shxzskj.cn

[B03] switch / match / case
来源：http://ue.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ve.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lg.hahajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dm.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aw.huanxung.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hi.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vz.szxytkj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bz.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bz.hnjuh.cn

[B04] for 计数循环
来源：http://qq.huixinmuqiang.cn

Py:   for i in range(10): print(i)
来源：http://cp.haigaiapp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mq.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://at.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zn.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ld.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jx.gzmigu.cn

Ruby: 10.times { |i| puts i }
来源：http://ss.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qe.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://qg.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://to.yuntaijiaju.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wy.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ic.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sn.bookmarksfly.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://fa.shxzukj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://re.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://uz.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pd.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://mq.bookmarksfly.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xc.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mt.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lf.newstarts.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ee.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yx.521024.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qa.yuexingan06.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wu.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bs.huixinmuqiang.cn

[B07] while 循环
来源：http://aw.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://eb.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ux.yuexingan06.cn

JS:   while (i < 10) { i++; }
来源：http://om.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://pe.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://vp.huixiangedu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fl.szsharing.cn

Ruby: while i < 10; i += 1; end
来源：http://nz.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://nr.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://fx.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://ni.9csxet.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wh.shxzskj.cn

JS:   do { i++; } while (i < 10);
来源：http://dv.shxzskj.cn

TS:   do { i++; } while (i < 10);
来源：http://gk.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://tv.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cz.jianghongdianzi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qo.shxzukj.cn

C#:   do { i++; } while (i < 10);
来源：http://yx.nicolike.cn

[B09] break 与 continue
来源：http://za.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zf.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://al.shxzskj.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bw.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rj.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mj.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://du.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zv.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sm.huanxung.cn

[B10] 遍历同时拿索引
来源：http://rv.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bo.haigaiapp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://js.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ko.hahajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://az.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cd.huanxung.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wm.colortex.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sk.wgjwhj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zj.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://qj.huanxung.cn

Py:   list(range(0, 10, 2))
来源：http://rn.hahajie.cn

PHP:  range(0, 10, 2);
来源：http://rl.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ct.521024.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ni.hnjuh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fh.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fs.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://jb.9csxet.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://be.panjiajie.cn

[B12] 跳出多层循环
来源：http://iq.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xz.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tk.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jh.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jn.bookmarksfly.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bf.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mr.yuntaijiaju.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ce.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xv.yuexingan06.cn

[B13] 判断是否为数字
来源：http://rt.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://pi.jctech888.com.cn

PHP:  is_numeric($x)
来源：http://jh.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fj.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ko.muxihuayi.cn

Java: x instanceof Number
来源：http://lu.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ip.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://dr.yuntaijiaju.cn

C#:   x is int or double or decimal
来源：http://dl.9csxet.cn

[B14] 判断值是否在集合内
来源：http://tm.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ur.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mg.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://al.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://ox.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xx.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fr.szxytkj.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kr.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xm.nszjky.cn

[B15] 布尔运算与取反
来源：http://nt.yuexingan06.cn

Py:   a and b or not c
来源：http://wx.yuexingan06.cn

PHP:  $a && $b || !$c
来源：http://ts.muxihuayi.cn

JS:   a && b || !c
来源：http://hp.colortex.cn

TS:   a && b || !c
来源：http://ol.gzmigu.cn

Java: a && b || !c
来源：http://kn.newstarts.cn

Go:   a && b || !c
来源：http://us.jianghongdianzi.cn

Ruby: a && b || !c
来源：http://rf.huixinmuqiang.cn

C#:   a && b || !c
来源：http://gt.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kw.9csxet.cn

Py:   if not data: return
来源：http://ub.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://ld.jctech888.com.cn

JS:   if (!data) return;
来源：http://hh.huixiangedu.cn

TS:   if (!data) return;
来源：http://gq.colortex.cn

Java: if (data == null) return;
来源：http://fy.asd995.cn

Go:   if data == nil { return }
来源：http://ro.huanxung.cn

Ruby: return if data.nil?
来源：http://du.asd995.cn

C#:   if (data == null) return;
来源：http://ke.hahajie.cn


<!-- 参考信息 -->