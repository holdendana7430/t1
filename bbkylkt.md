代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://qv.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qm.huanxung.cn

[A12] 字符串插值 / 格式化
来源：http://zl.colortex.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gf.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hk.lnxyls.cn

JS:   `Hello, ${name}!`
来源：http://rk.colortex.cn

TS:   `Hello, ${name}!`
来源：http://rv.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://cn.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mm.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://nd.newstarts.cn

C#:   $"Hello, {name}!"
来源：http://qq.bookmarksfly.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oy.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://xl.hnjuh.cn

PHP:  "第一行\n第二行"
来源：http://yo.hahajie.cn

JS:   "第一行\n第二行"
来源：http://on.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://jr.huixiangedu.cn

Java: "第一行\n第二行"
来源：http://uw.nszjky.cn

Go:   "第一行\n第二行"
来源：http://kn.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://sz.haigaiapp.cn

C#:   "第一行\n第二行"
来源：http://ow.huanxung.cn

[A14] 注释写法
来源：http://mn.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dk.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://nk.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://lq.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://uq.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ez.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://vh.shxzskj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rw.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://sz.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://aw.newstarts.cn

Py:   value = data or "默认值"
来源：http://je.chemitech.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://dl.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://hs.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://ik.jianghongdianzi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vy.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://ae.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://nv.jctech888.com.cn

C#:   var value = data ?? "默认值";
来源：http://hy.szsharing.cn

[A16] 真假值判断规则
来源：http://cj.gzmigu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wu.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vf.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ii.haigaiapp.cn

TS:   if (!x) {}
来源：http://cm.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fy.yuntaijiaju.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fi.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ju.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rb.nicolike.cn

[A17] 位运算
来源：http://cm.hnjuh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ao.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ru.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hm.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lo.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nu.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uf.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jg.newstarts.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sp.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://wn.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://gv.lnxyls.cn

PHP:  ord("A"); chr(65)
来源：http://rr.hahajie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ir.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qz.yuexingan06.cn

Java: (int) 'A'; (char) 65
来源：http://ye.hahajie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tq.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://xr.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://fg.colortex.cn

[A19] 交换两个变量
来源：http://qh.wgjwhj.cn

Py:   a, b = b, a
来源：http://ch.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://th.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://aa.bjjhwx.cn

TS:   [a, b] = [b, a];
来源：http://aj.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://az.gzmigu.cn

Go:   a, b = b, a
来源：http://ns.chemitech.net.cn

Ruby: a, b = b, a
来源：http://yu.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://ms.muxihuayi.cn

[A20] 读取标准输入
来源：http://tl.asd995.cn

Py:   name = input("请输入：")
来源：http://ew.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kp.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ui.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://sk.jianghongdianzi.cn

Java: new Scanner(System.in).nextLine()
来源：http://mh.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cy.szxytkj.cn

Ruby: gets.chomp
来源：http://ud.hnjuh.cn

C#:   Console.ReadLine();
来源：http://ym.521024.cn

[A21] 保留指定小数位输出
来源：http://mb.jianghongdianzi.cn

Py:   f"{3.14159:.2f}"
来源：http://gz.yuntaijiaju.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nt.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://pn.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://cx.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://pw.huixiangedu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zl.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://mn.shxzskj.cn

C#:   3.14159.ToString("F2")
来源：http://jy.haigaiapp.cn

[A22] 获取字符串长度
来源：http://fy.shxzukj.cn

Py:   len(s)
来源：http://oi.gzmigu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vm.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://br.szxytkj.cn

TS:   s.length
来源：http://ax.wgjwhj.cn

Java: s.length()
来源：http://ij.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pi.chemitech.net.cn

Ruby: s.length
来源：http://mx.colortex.cn

C#:   s.Length
来源：http://fy.asd995.cn

[A23] 大小写转换
来源：http://gv.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zx.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kl.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rs.huixinmuqiang.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ri.asd995.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ea.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ws.huixinmuqiang.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mw.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://az.asd995.cn

[A24] 去除首尾空白
来源：http://my.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sw.colortex.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cp.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oq.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://us.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mw.bookmarksfly.cn

Go:   strings.TrimSpace(s)
来源：http://rz.lnxyls.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://op.huanxung.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sw.asd995.cn

[A25] 字符串比较
来源：http://ci.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://pq.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sh.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ix.521024.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nw.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jd.huixiangedu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://td.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dk.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gu.huixiangedu.cn

[A26] 类型转换总览
来源：http://yx.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gd.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jx.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rv.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://ek.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jo.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pw.jianghongdianzi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qf.jianghongdianzi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sa.yuntaijiaju.cn

================================================================================
来源：http://rw.nicolike.cn

B. 流程控制
来源：http://rm.huixinmuqiang.cn

================================================================================
来源：http://in.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://sy.nicolike.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hj.hahajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oh.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ym.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://op.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ei.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yq.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rf.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qe.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://wu.jctech888.com.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ac.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hh.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jn.yuexingan06.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ij.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://an.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://td.haigaiapp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tj.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yx.wgjwhj.cn

[B03] switch / match / case
来源：http://jt.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ts.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zu.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gq.shtwfgs.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bm.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hw.szsharing.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://af.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://za.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xv.yuntaijiaju.cn

[B04] for 计数循环
来源：http://gp.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://mu.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tr.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hf.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rx.wgjwhj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hh.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gt.521024.cn

Ruby: 10.times { |i| puts i }
来源：http://uo.szsharing.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wu.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://ky.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://am.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tz.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bt.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://az.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://iz.haigaiapp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xx.gzmigu.cn

Ruby: arr.each { |item| puts item }
来源：http://lt.shxzukj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wn.shxzskj.cn

[B06] 遍历字典 / 对象
来源：http://ut.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zl.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rf.colortex.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yo.bjjhwx.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wd.huixiangedu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://da.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yb.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nz.bjjhwx.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sk.panjiajie.cn

[B07] while 循环
来源：http://ck.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://pa.newstarts.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rh.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://rn.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://dk.haigaiapp.cn

Java: while (i < 10) { i++; }
来源：http://am.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vx.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://gf.bookmarksfly.cn

C#:   while (i < 10) { i++; }
来源：http://jp.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://za.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://ac.shxzskj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oj.colortex.cn

JS:   do { i++; } while (i < 10);
来源：http://wc.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://sg.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://ru.colortex.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://br.9csxet.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mc.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://ok.hahajie.cn

[B09] break 与 continue
来源：http://oy.hahajie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lk.panjiajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cv.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tm.huanxung.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pi.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pu.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ie.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ua.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xi.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://hb.lnxyls.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://be.colortex.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hj.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://be.szxytkj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vk.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wt.bookmarksfly.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eo.jianghongdianzi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xt.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sy.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://jr.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://nt.nicolike.cn

PHP:  range(0, 10, 2);
来源：http://om.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xg.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bu.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vw.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eh.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://ja.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ib.wgjwhj.cn

[B12] 跳出多层循环
来源：http://vp.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hc.lnxyls.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://sx.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vh.gzmigu.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cr.shxzukj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mn.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mc.gzmigu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lo.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vi.bjjhwx.cn

[B13] 判断是否为数字
来源：http://nb.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://rm.nicolike.cn

PHP:  is_numeric($x)
来源：http://fc.szxytkj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://th.yuexingan06.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yk.haigaiapp.cn

Java: x instanceof Number
来源：http://zs.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hf.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://df.panjiajie.cn

C#:   x is int or double or decimal
来源：http://lz.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://ye.newstarts.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zc.9csxet.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xr.huixinmuqiang.cn

JS:   [1, 2, 3].includes(x)
来源：http://qm.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://ht.shtwfgs.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pq.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ye.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vk.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wf.gzmigu.cn

[B15] 布尔运算与取反
来源：http://sn.yuexingan06.cn

Py:   a and b or not c
来源：http://km.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://wn.newstarts.cn

JS:   a && b || !c
来源：http://ug.shtwfgs.cn

TS:   a && b || !c
来源：http://xd.bookmarksfly.cn

Java: a && b || !c
来源：http://qm.huixiangedu.cn

Go:   a && b || !c
来源：http://ad.szxytkj.cn

Ruby: a && b || !c
来源：http://zq.shxzskj.cn

C#:   a && b || !c
来源：http://zj.yuexingan06.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pp.nicolike.cn

Py:   if not data: return
来源：http://ky.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://fy.newstarts.cn

JS:   if (!data) return;
来源：http://pb.chemitech.net.cn

TS:   if (!data) return;
来源：http://fm.haigaiapp.cn

Java: if (data == null) return;
来源：http://tn.shtwfgs.cn

Go:   if data == nil { return }
来源：http://fz.panjiajie.cn

Ruby: return if data.nil?
来源：http://lj.szsharing.cn

C#:   if (data == null) return;
来源：http://zd.szsharing.cn

================================================================================
来源：http://bb.lnxyls.cn

C. 函数与作用域
来源：http://or.lnxyls.cn

================================================================================
来源：http://jq.asd995.cn

[C01] 定义函数
来源：http://kz.newstarts.cn

Py:   def add(a, b): return a + b
来源：http://ms.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dd.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ix.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nn.szsharing.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ov.jianghongdianzi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dn.asd995.cn

Ruby: def add(a, b); a + b; end
来源：http://fe.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zi.chemitech.net.cn

[C02] 默认参数
来源：http://sy.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://sd.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bm.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://bq.nicolike.cn


<!-- 参考信息 -->