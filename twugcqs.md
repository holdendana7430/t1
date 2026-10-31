代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://wh.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://au.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://xf.shxzskj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rt.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jt.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ew.panjiajie.cn

[A12] 字符串插值 / 格式化
来源：http://oe.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://av.shtwfgs.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bf.yuntaijiaju.cn

JS:   `Hello, ${name}!`
来源：http://mh.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://ce.yuexingan06.cn

Java: "Hello, %s!".formatted(name)
来源：http://iw.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jx.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://ng.newstarts.cn

C#:   $"Hello, {name}!"
来源：http://nk.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://nm.huixiangedu.cn

Py:   "第一行\n第二行"
来源：http://ym.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://oi.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://pk.nszjky.cn

TS:   "第一行\n第二行"
来源：http://yf.bookmarksfly.cn

Java: "第一行\n第二行"
来源：http://zt.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://lh.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://os.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://vm.huixinmuqiang.cn

[A14] 注释写法
来源：http://ik.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ho.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rl.huixiangedu.cn

JS:   // 单行；/* 多行 */
来源：http://br.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://fz.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mm.huanxung.cn

Go:   // 单行；/* 多行 */
来源：http://hn.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ga.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://nz.hnjuh.cn

[A15] 空值判断与默认值
来源：http://hx.newstarts.cn

Py:   value = data or "默认值"
来源：http://gt.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://vv.panjiajie.cn

JS:   const value = data ?? "默认值";
来源：http://tp.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://ju.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mj.szxytkj.cn

Go:   if data == "" { data = "默认值" }
来源：http://jr.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://lf.huanxung.cn

C#:   var value = data ?? "默认值";
来源：http://cz.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://bv.wgjwhj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qw.haigaiapp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mk.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xe.szxytkj.cn

TS:   if (!x) {}
来源：http://wp.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zb.muxihuayi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eo.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qx.colortex.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dq.asd995.cn

[A17] 位运算
来源：http://jv.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eq.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hd.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qo.nszjky.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ma.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jt.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yd.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bn.gzmigu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pb.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://vh.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://xs.yuexingan06.cn

PHP:  ord("A"); chr(65)
来源：http://vk.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dt.asd995.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pu.jianghongdianzi.cn

Java: (int) 'A'; (char) 65
来源：http://xt.asd995.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gh.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://yi.colortex.cn

C#:   (int)'A'; (char)65
来源：http://cf.9csxet.cn

[A19] 交换两个变量
来源：http://oy.yuexingan06.cn

Py:   a, b = b, a
来源：http://qs.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fd.asd995.cn

JS:   [a, b] = [b, a];
来源：http://ff.lnxyls.cn

TS:   [a, b] = [b, a];
来源：http://ig.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://cm.wgjwhj.cn

Go:   a, b = b, a
来源：http://zh.gzmigu.cn

Ruby: a, b = b, a
来源：http://yp.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://zk.muxihuayi.cn

[A20] 读取标准输入
来源：http://gv.szsharing.cn

Py:   name = input("请输入：")
来源：http://js.huixinmuqiang.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qm.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nl.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://tg.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://ah.gzmigu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yj.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://wf.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://zq.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://ef.huixinmuqiang.cn

Py:   f"{3.14159:.2f}"
来源：http://ns.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://it.shxzukj.cn

JS:   (3.14159).toFixed(2)
来源：http://zi.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://wj.9csxet.cn

Java: String.format("%.2f", 3.14159)
来源：http://tf.shxzukj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xx.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://sb.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://ry.shxzukj.cn

[A22] 获取字符串长度
来源：http://yg.jctech888.com.cn

Py:   len(s)
来源：http://ks.bjjhwx.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kb.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://en.gzmigu.cn

TS:   s.length
来源：http://mi.muxihuayi.cn

Java: s.length()
来源：http://jc.panjiajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kg.gzmigu.cn

Ruby: s.length
来源：http://ij.nicolike.cn

C#:   s.Length
来源：http://yx.huixiangedu.cn

[A23] 大小写转换
来源：http://yl.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ys.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sd.haigaiapp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dz.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://en.newstarts.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://aa.gzmigu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ij.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yw.521024.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cb.szsharing.cn

[A24] 去除首尾空白
来源：http://rm.szxytkj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lz.huixinmuqiang.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ke.jianghongdianzi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jy.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dv.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vu.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://jg.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nf.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zk.huanxung.cn

[A25] 字符串比较
来源：http://tv.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://rg.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://za.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yc.gzmigu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ou.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jc.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ri.521024.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gl.chemitech.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://er.newstarts.cn

[A26] 类型转换总览
来源：http://yi.szsharing.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rb.shtwfgs.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://es.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lx.nicolike.cn

TS:   Number() String() Boolean() x as number
来源：http://jy.bjjhwx.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lx.szxytkj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rd.shxzskj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uj.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ge.huanxung.cn

================================================================================
来源：http://jh.shxzukj.cn

B. 流程控制
来源：http://ss.jianghongdianzi.cn

================================================================================
来源：http://vh.nszjky.cn

[B01] 条件判断 if / else
来源：http://hq.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ze.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eb.muxihuayi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rw.jianghongdianzi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dl.newstarts.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://td.huixinmuqiang.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yh.521024.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://il.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ju.muxihuayi.cn

[B02] 多分支 else if / elif
来源：http://qf.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jl.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pw.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zx.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pd.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://df.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hl.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vi.521024.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://po.muxihuayi.cn

[B03] switch / match / case
来源：http://en.nicolike.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zc.yuntaijiaju.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ij.panjiajie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mj.muxihuayi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sp.yuntaijiaju.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://km.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mw.yuexingan06.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gd.chemitech.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yy.shxzskj.cn

[B04] for 计数循环
来源：http://bl.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://ja.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bh.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mp.bjjhwx.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cc.shxzukj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jl.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ck.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://td.szxytkj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pi.asd995.cn

[B05] 遍历数组 / 列表
来源：http://lk.newstarts.cn

Py:   for item in arr: print(item)
来源：http://ir.yuexingan06.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zk.huanxung.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cx.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oa.lnxyls.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pu.szxytkj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rx.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://hy.haigaiapp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vt.bjjhwx.cn

[B06] 遍历字典 / 对象
来源：http://cj.yuntaijiaju.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ru.yuntaijiaju.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yk.huixiangedu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zw.chemitech.net.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wo.nicolike.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kj.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cq.nszjky.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dg.muxihuayi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ey.panjiajie.cn

[B07] while 循环
来源：http://xt.yuntaijiaju.cn

Py:   while i < 10: i += 1
来源：http://do.huanxung.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rt.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://gk.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://tf.huixiangedu.cn

Java: while (i < 10) { i++; }
来源：http://io.9csxet.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ag.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://yz.521024.cn

C#:   while (i < 10) { i++; }
来源：http://nn.shxzskj.cn

[B08] do-while（至少执行一次）
来源：http://ru.shtwfgs.cn

Py:   # 无 do-while：用 while True + break
来源：http://ag.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ai.nszjky.cn

JS:   do { i++; } while (i < 10);
来源：http://ma.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://wx.huixinmuqiang.cn

Java: do { i++; } while (i < 10);
来源：http://ka.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://eq.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nf.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://qx.huanxung.cn

[B09] break 与 continue
来源：http://vd.huixiangedu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://oy.9csxet.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cb.huixinmuqiang.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ka.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://he.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ib.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cc.panjiajie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://py.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qz.newstarts.cn

[B10] 遍历同时拿索引
来源：http://pa.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xk.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ob.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kq.szsharing.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://aq.huanxung.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cn.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fg.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oo.nszjky.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cs.huixinmuqiang.cn

[B11] 生成数字序列 / 区间
来源：http://ke.bookmarksfly.cn

Py:   list(range(0, 10, 2))
来源：http://tu.panjiajie.cn

PHP:  range(0, 10, 2);
来源：http://ba.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hf.huixiangedu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nc.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cf.szsharing.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jm.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://wn.haigaiapp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ug.szxytkj.cn

[B12] 跳出多层循环
来源：http://tp.asd995.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qz.jianghongdianzi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ef.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yx.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vr.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zy.panjiajie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://db.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ky.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bj.haigaiapp.cn

[B13] 判断是否为数字
来源：http://su.bookmarksfly.cn

Py:   isinstance(x, (int, float))
来源：http://fv.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://at.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ks.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nl.jianghongdianzi.cn

Java: x instanceof Number
来源：http://bp.hnjuh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ds.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://jj.shxzukj.cn

C#:   x is int or double or decimal
来源：http://nz.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://vd.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fl.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ro.lnxyls.cn

JS:   [1, 2, 3].includes(x)
来源：http://ij.521024.cn

TS:   [1, 2, 3].includes(x)
来源：http://ai.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qm.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vk.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xx.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://he.gzmigu.cn

[B15] 布尔运算与取反
来源：http://uo.jianghongdianzi.cn

Py:   a and b or not c
来源：http://xm.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://rg.yuexingan06.cn

JS:   a && b || !c
来源：http://bk.huixinmuqiang.cn

TS:   a && b || !c
来源：http://hi.szxytkj.cn

Java: a && b || !c
来源：http://fi.newstarts.cn

Go:   a && b || !c
来源：http://uc.gzmigu.cn

Ruby: a && b || !c
来源：http://pr.szsharing.cn

C#:   a && b || !c
来源：http://no.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cw.shtwfgs.cn

Py:   if not data: return
来源：http://mx.521024.cn

PHP:  if (!$data) { return; }
来源：http://hs.nszjky.cn

JS:   if (!data) return;
来源：http://tq.muxihuayi.cn

TS:   if (!data) return;
来源：http://fk.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://kt.lnxyls.cn

Go:   if data == nil { return }
来源：http://gw.chemitech.net.cn

Ruby: return if data.nil?
来源：http://sw.colortex.cn

C#:   if (data == null) return;
来源：http://jo.wgjwhj.cn

================================================================================
来源：http://al.wgjwhj.cn

C. 函数与作用域
来源：http://nq.huixinmuqiang.cn

================================================================================
来源：http://ru.yuexingan06.cn

[C01] 定义函数
来源：http://al.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://se.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ri.wgjwhj.cn

JS:   function add(a, b) { return a + b; }
来源：http://lh.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wa.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zq.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kw.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://mm.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cn.wgjwhj.cn


<!-- 参考信息 -->