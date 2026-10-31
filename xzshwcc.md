代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ei.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://cz.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hh.newstarts.cn

Ruby: rand(1..100)
来源：http://ak.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://hs.shtwfgs.cn

[A11] 条件表达式（三元）
来源：http://qe.jctech888.com.cn

Py:   "yes" if x > 0 else "no"
来源：http://zb.szxytkj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://us.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bu.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rk.newstarts.cn

Java: x > 0 ? "yes" : "no"
来源：http://fb.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://eq.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sb.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ec.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://zk.muxihuayi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dt.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://it.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://jb.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://gk.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://tw.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fz.gzmigu.cn

Ruby: "Hello, #{name}!"
来源：http://xc.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://pv.muxihuayi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hl.nszjky.cn

Py:   "第一行\n第二行"
来源：http://sw.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://by.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://ka.9csxet.cn

TS:   "第一行\n第二行"
来源：http://xm.nszjky.cn

Java: "第一行\n第二行"
来源：http://jc.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://km.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://nw.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://vj.huixiangedu.cn

[A14] 注释写法
来源：http://go.shxzukj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nh.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zf.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://jn.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://xt.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tl.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://ae.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://st.hahajie.cn

C#:   // 单行；/* 多行 */
来源：http://sz.nszjky.cn

[A15] 空值判断与默认值
来源：http://hp.huanxung.cn

Py:   value = data or "默认值"
来源：http://en.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://lt.huanxung.cn

JS:   const value = data ?? "默认值";
来源：http://ya.521024.cn

TS:   const value = data ?? "默认值";
来源：http://nb.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ab.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://jb.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://ye.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://br.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://kb.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cw.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mm.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wg.hahajie.cn

TS:   if (!x) {}
来源：http://cx.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://er.chemitech.net.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qf.panjiajie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://se.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tl.jianghongdianzi.cn

[A17] 位运算
来源：http://ai.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cw.newstarts.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ll.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xv.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gh.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oz.huixiangedu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bv.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zt.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://go.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://bg.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://gi.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://ij.shxzukj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ju.hnjuh.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://un.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://jq.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lg.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://qt.lnxyls.cn

C#:   (int)'A'; (char)65
来源：http://cy.bjjhwx.cn

[A19] 交换两个变量
来源：http://ko.jctech888.com.cn

Py:   a, b = b, a
来源：http://uz.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kr.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://mh.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://gy.huixiangedu.cn

Java: int t = a; a = b; b = t;
来源：http://xq.9csxet.cn

Go:   a, b = b, a
来源：http://op.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://ah.colortex.cn

C#:   (a, b) = (b, a);
来源：http://ie.bjjhwx.cn

[A20] 读取标准输入
来源：http://si.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://fv.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rv.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lu.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://bj.asd995.cn

Java: new Scanner(System.in).nextLine()
来源：http://pi.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hl.muxihuayi.cn

Ruby: gets.chomp
来源：http://we.lnxyls.cn

C#:   Console.ReadLine();
来源：http://st.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://as.colortex.cn

Py:   f"{3.14159:.2f}"
来源：http://xi.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uk.521024.cn

JS:   (3.14159).toFixed(2)
来源：http://fd.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://nt.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://mc.shtwfgs.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ra.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://ds.521024.cn

C#:   3.14159.ToString("F2")
来源：http://nv.szxytkj.cn

[A22] 获取字符串长度
来源：http://zu.bjjhwx.cn

Py:   len(s)
来源：http://fg.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cd.shxzskj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hi.huixiangedu.cn

TS:   s.length
来源：http://pe.lnxyls.cn

Java: s.length()
来源：http://ll.huanxung.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nf.haigaiapp.cn

Ruby: s.length
来源：http://tu.shxzskj.cn

C#:   s.Length
来源：http://gc.9csxet.cn

[A23] 大小写转换
来源：http://pu.panjiajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hl.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jw.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sd.lnxyls.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ei.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qv.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ky.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xq.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://aw.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://jj.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ot.gzmigu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mr.nicolike.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rx.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nr.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xu.jctech888.com.cn

Go:   strings.TrimSpace(s)
来源：http://zo.bookmarksfly.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fl.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ps.huixinmuqiang.cn

[A25] 字符串比较
来源：http://yv.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://ij.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ou.bjjhwx.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ee.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ee.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://al.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ri.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://za.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rc.wgjwhj.cn

[A26] 类型转换总览
来源：http://yc.huixiangedu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cx.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xz.9csxet.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mm.shxzukj.cn

TS:   Number() String() Boolean() x as number
来源：http://hv.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yv.szsharing.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fu.colortex.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ut.chemitech.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xn.gzmigu.cn

================================================================================
来源：http://qq.nicolike.cn

B. 流程控制
来源：http://jv.jianghongdianzi.cn

================================================================================
来源：http://at.szsharing.cn

[B01] 条件判断 if / else
来源：http://re.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oq.bookmarksfly.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rj.yuntaijiaju.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zc.bjjhwx.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yn.panjiajie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tw.bjjhwx.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kr.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ze.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wg.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://di.yuntaijiaju.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oh.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dg.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kp.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vr.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ei.shxzskj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mx.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://af.gzmigu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qd.521024.cn

[B03] switch / match / case
来源：http://vf.shtwfgs.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hw.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ob.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://le.hnjuh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xa.hahajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cy.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zx.hnjuh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qw.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gv.huixiangedu.cn

[B04] for 计数循环
来源：http://nh.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://ua.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hh.panjiajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eq.lnxyls.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dh.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zx.521024.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rg.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://dy.nszjky.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bn.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://lb.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://tf.nszjky.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gx.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ok.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qv.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://db.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qf.jianghongdianzi.cn

Ruby: arr.each { |item| puts item }
来源：http://nt.nicolike.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pj.521024.cn

[B06] 遍历字典 / 对象
来源：http://qg.huixinmuqiang.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ou.bookmarksfly.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fk.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mu.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lf.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vo.haigaiapp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yl.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cb.asd995.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hp.shtwfgs.cn

[B07] while 循环
来源：http://in.nszjky.cn

Py:   while i < 10: i += 1
来源：http://xi.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jw.521024.cn

JS:   while (i < 10) { i++; }
来源：http://tw.lnxyls.cn

TS:   while (i < 10) { i++; }
来源：http://zg.shxzskj.cn

Java: while (i < 10) { i++; }
来源：http://jt.yuexingan06.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ym.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://jc.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://fs.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://ah.szsharing.cn

Py:   # 无 do-while：用 while True + break
来源：http://yf.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ji.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://dw.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://pe.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://my.newstarts.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gh.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://co.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://di.haigaiapp.cn

[B09] break 与 continue
来源：http://cx.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hl.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ts.muxihuayi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://et.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ub.huixinmuqiang.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zc.wgjwhj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ys.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sl.hahajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vw.hahajie.cn

[B10] 遍历同时拿索引
来源：http://en.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://io.yuntaijiaju.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sa.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lr.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aw.jianghongdianzi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ox.muxihuayi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bw.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tu.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ln.shxzukj.cn

[B11] 生成数字序列 / 区间
来源：http://hy.muxihuayi.cn

Py:   list(range(0, 10, 2))
来源：http://lt.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://fh.bjjhwx.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://af.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mv.yuntaijiaju.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pk.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ml.nszjky.cn

Ruby: (0...10).step(2).to_a
来源：http://tf.521024.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dl.huixiangedu.cn

[B12] 跳出多层循环
来源：http://ei.521024.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gf.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://za.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wm.9csxet.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://la.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hk.yuntaijiaju.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zv.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tj.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xp.bjjhwx.cn

[B13] 判断是否为数字
来源：http://se.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://hw.colortex.cn

PHP:  is_numeric($x)
来源：http://ue.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pm.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xg.yuexingan06.cn

Java: x instanceof Number
来源：http://dl.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gx.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://tu.hnjuh.cn

C#:   x is int or double or decimal
来源：http://vm.bookmarksfly.cn

[B14] 判断值是否在集合内
来源：http://wb.wgjwhj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ez.bookmarksfly.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://km.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://jg.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://cz.chemitech.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rl.szxytkj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rv.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cb.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ib.bookmarksfly.cn

[B15] 布尔运算与取反
来源：http://eh.yuntaijiaju.cn

Py:   a and b or not c
来源：http://bu.nicolike.cn

PHP:  $a && $b || !$c
来源：http://ms.huixiangedu.cn

JS:   a && b || !c
来源：http://hh.jctech888.com.cn

TS:   a && b || !c
来源：http://em.newstarts.cn

Java: a && b || !c
来源：http://fi.colortex.cn

Go:   a && b || !c
来源：http://nd.nszjky.cn

Ruby: a && b || !c
来源：http://yt.bookmarksfly.cn

C#:   a && b || !c
来源：http://dw.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ku.szsharing.cn

Py:   if not data: return
来源：http://ih.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://yn.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://cr.szsharing.cn

TS:   if (!data) return;
来源：http://fj.haigaiapp.cn

Java: if (data == null) return;
来源：http://ob.muxihuayi.cn

Go:   if data == nil { return }
来源：http://hd.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://nk.521024.cn

C#:   if (data == null) return;
来源：http://zd.huixiangedu.cn

================================================================================
来源：http://yh.jianghongdianzi.cn

C. 函数与作用域
来源：http://xc.huixinmuqiang.cn

================================================================================
来源：http://im.bookmarksfly.cn

[C01] 定义函数
来源：http://ol.shxzukj.cn


<!-- 参考信息 -->