代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://nn.shxzskj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ri.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://lw.gzmigu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pp.hnjuh.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xv.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://si.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://rm.9csxet.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gp.nicolike.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://do.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://em.gzmigu.cn

TS:   `Hello, ${name}!`
来源：http://jq.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://kf.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fp.muxihuayi.cn

Ruby: "Hello, #{name}!"
来源：http://zy.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://vl.panjiajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cq.colortex.cn

Py:   "第一行\n第二行"
来源：http://eb.haigaiapp.cn

PHP:  "第一行\n第二行"
来源：http://ts.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://xg.521024.cn

TS:   "第一行\n第二行"
来源：http://jn.panjiajie.cn

Java: "第一行\n第二行"
来源：http://jv.panjiajie.cn

Go:   "第一行\n第二行"
来源：http://qt.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://mi.shxzukj.cn

C#:   "第一行\n第二行"
来源：http://zs.lnxyls.cn

[A14] 注释写法
来源：http://ap.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pp.bookmarksfly.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://cx.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://zw.nicolike.cn

TS:   // 单行；/* 多行 */
来源：http://rq.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dq.bjjhwx.cn

Go:   // 单行；/* 多行 */
来源：http://wd.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://we.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://nx.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://ht.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://lk.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://mt.521024.cn

JS:   const value = data ?? "默认值";
来源：http://ig.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://oc.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zx.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://zq.newstarts.cn

Ruby: value = data || "默认值"
来源：http://ew.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://nk.asd995.cn

[A16] 真假值判断规则
来源：http://mm.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ni.szxytkj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wo.shtwfgs.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ig.jctech888.com.cn

TS:   if (!x) {}
来源：http://pi.jctech888.com.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qy.haigaiapp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ck.bjjhwx.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pu.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ro.chemitech.net.cn

[A17] 位运算
来源：http://la.nicolike.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hr.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eo.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mb.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yq.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lg.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jw.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ik.yuexingan06.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xw.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://un.huixinmuqiang.cn

Py:   ord("A"); chr(65)
来源：http://dp.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://rw.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ow.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xw.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://sj.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yz.jianghongdianzi.cn

Ruby: "A".ord; 65.chr
来源：http://tz.yuexingan06.cn

C#:   (int)'A'; (char)65
来源：http://uh.chemitech.net.cn

[A19] 交换两个变量
来源：http://gl.hahajie.cn

Py:   a, b = b, a
来源：http://gd.gzmigu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://of.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://dl.hnjuh.cn

TS:   [a, b] = [b, a];
来源：http://jl.haigaiapp.cn

Java: int t = a; a = b; b = t;
来源：http://ff.colortex.cn

Go:   a, b = b, a
来源：http://ls.wgjwhj.cn

Ruby: a, b = b, a
来源：http://tu.jianghongdianzi.cn

C#:   (a, b) = (b, a);
来源：http://kn.wgjwhj.cn

[A20] 读取标准输入
来源：http://fq.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://xw.bjjhwx.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ke.asd995.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ij.9csxet.cn

TS:   // Node.js：readline 模块
来源：http://do.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://wv.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ma.bookmarksfly.cn

Ruby: gets.chomp
来源：http://fb.muxihuayi.cn

C#:   Console.ReadLine();
来源：http://wj.9csxet.cn

[A21] 保留指定小数位输出
来源：http://uy.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://fc.panjiajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://af.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://uy.chemitech.net.cn

TS:   (3.14159).toFixed(2)
来源：http://ba.jctech888.com.cn

Java: String.format("%.2f", 3.14159)
来源：http://wh.szsharing.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oe.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://ma.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://hk.huixiangedu.cn

[A22] 获取字符串长度
来源：http://ap.asd995.cn

Py:   len(s)
来源：http://xc.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xx.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wf.nszjky.cn

TS:   s.length
来源：http://kc.gzmigu.cn

Java: s.length()
来源：http://wx.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pe.yuntaijiaju.cn

Ruby: s.length
来源：http://dp.521024.cn

C#:   s.Length
来源：http://yv.nicolike.cn

[A23] 大小写转换
来源：http://hb.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rd.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mz.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rk.haigaiapp.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://by.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bx.huixinmuqiang.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://it.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ya.haigaiapp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wg.huixiangedu.cn

[A24] 去除首尾空白
来源：http://ki.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bp.huanxung.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ms.wgjwhj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uo.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://op.yuexingan06.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ih.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://jo.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sv.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yb.hahajie.cn

[A25] 字符串比较
来源：http://ji.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://tj.yuntaijiaju.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ob.shtwfgs.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tx.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qb.9csxet.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ma.colortex.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://if.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vg.muxihuayi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vv.shxzskj.cn

[A26] 类型转换总览
来源：http://ca.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ja.bookmarksfly.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hw.chemitech.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://to.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://ka.gzmigu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zb.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yy.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xy.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ev.521024.cn

================================================================================
来源：http://br.shxzskj.cn

B. 流程控制
来源：http://ub.hahajie.cn

================================================================================
来源：http://um.9csxet.cn

[B01] 条件判断 if / else
来源：http://tc.bjjhwx.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ca.muxihuayi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fa.panjiajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nj.nszjky.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ql.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ov.yuexingan06.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ru.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aj.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ae.szsharing.cn

[B02] 多分支 else if / elif
来源：http://kl.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yn.szsharing.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vk.newstarts.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jy.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://at.asd995.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qd.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bk.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xt.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qd.jianghongdianzi.cn

[B03] switch / match / case
来源：http://wh.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ai.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gb.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zf.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qk.bjjhwx.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cr.muxihuayi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wh.nszjky.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ei.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rx.colortex.cn

[B04] for 计数循环
来源：http://xi.jianghongdianzi.cn

Py:   for i in range(10): print(i)
来源：http://ob.newstarts.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zz.colortex.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ku.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ah.muxihuayi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zm.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ok.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://jf.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://os.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://xt.bjjhwx.cn

Py:   for item in arr: print(item)
来源：http://to.gzmigu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fv.asd995.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jc.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://de.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://li.hnjuh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mo.521024.cn

Ruby: arr.each { |item| puts item }
来源：http://ah.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hx.asd995.cn

[B06] 遍历字典 / 对象
来源：http://ki.yuexingan06.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mo.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oe.shtwfgs.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zo.nicolike.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aw.yuexingan06.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pp.jianghongdianzi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ug.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.szxytkj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jy.panjiajie.cn

[B07] while 循环
来源：http://vy.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://ix.nicolike.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mb.wgjwhj.cn

JS:   while (i < 10) { i++; }
来源：http://iw.wgjwhj.cn

TS:   while (i < 10) { i++; }
来源：http://nt.521024.cn

Java: while (i < 10) { i++; }
来源：http://pk.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gu.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://cl.shxzskj.cn

C#:   while (i < 10) { i++; }
来源：http://eb.nszjky.cn

[B08] do-while（至少执行一次）
来源：http://ys.gzmigu.cn

Py:   # 无 do-while：用 while True + break
来源：http://wq.jianghongdianzi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pj.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://ic.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://th.lnxyls.cn

Java: do { i++; } while (i < 10);
来源：http://wl.lnxyls.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jr.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://el.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://xd.shxzukj.cn

[B09] break 与 continue
来源：http://sg.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zv.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://th.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dn.jctech888.com.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iv.huixiangedu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jj.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wa.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zk.shxzskj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://od.jianghongdianzi.cn

[B10] 遍历同时拿索引
来源：http://mh.szxytkj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fq.huixinmuqiang.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ap.hnjuh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pt.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lz.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zn.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zf.szxytkj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wd.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sq.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://eq.nszjky.cn

Py:   list(range(0, 10, 2))
来源：http://ez.muxihuayi.cn

PHP:  range(0, 10, 2);
来源：http://tp.colortex.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ny.huixinmuqiang.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yv.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ji.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lt.panjiajie.cn

Ruby: (0...10).step(2).to_a
来源：http://av.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eu.wgjwhj.cn

[B12] 跳出多层循环
来源：http://lw.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sn.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://en.yuntaijiaju.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://an.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://do.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dw.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zg.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mr.colortex.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pk.jctech888.com.cn

[B13] 判断是否为数字
来源：http://tg.jianghongdianzi.cn

Py:   isinstance(x, (int, float))
来源：http://wb.9csxet.cn

PHP:  is_numeric($x)
来源：http://dg.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yn.szsharing.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hq.lnxyls.cn

Java: x instanceof Number
来源：http://ad.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qo.asd995.cn

Ruby: x.is_a?(Numeric)
来源：http://uc.shxzukj.cn

C#:   x is int or double or decimal
来源：http://om.lnxyls.cn

[B14] 判断值是否在集合内
来源：http://ma.shtwfgs.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aa.colortex.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://at.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://qf.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://iy.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bv.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qv.muxihuayi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rx.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fb.nicolike.cn

[B15] 布尔运算与取反
来源：http://tn.shxzskj.cn

Py:   a and b or not c
来源：http://cp.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://fh.huixiangedu.cn

JS:   a && b || !c
来源：http://zf.szxytkj.cn

TS:   a && b || !c
来源：http://pn.nicolike.cn

Java: a && b || !c
来源：http://su.yuexingan06.cn

Go:   a && b || !c
来源：http://bw.hahajie.cn

Ruby: a && b || !c
来源：http://np.gzmigu.cn

C#:   a && b || !c
来源：http://jp.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bl.shxzskj.cn

Py:   if not data: return
来源：http://tu.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://da.shtwfgs.cn

JS:   if (!data) return;
来源：http://bm.chemitech.net.cn

TS:   if (!data) return;
来源：http://lp.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://ig.asd995.cn

Go:   if data == nil { return }
来源：http://hg.bjjhwx.cn

Ruby: return if data.nil?
来源：http://fg.jctech888.com.cn

C#:   if (data == null) return;
来源：http://qq.gzmigu.cn

================================================================================
来源：http://xb.yuntaijiaju.cn

C. 函数与作用域
来源：http://oj.bjjhwx.cn

================================================================================
来源：http://un.9csxet.cn

[C01] 定义函数
来源：http://wo.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://tj.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://je.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://eo.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nr.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://je.chemitech.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qz.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://ir.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lg.shtwfgs.cn


<!-- 参考信息 -->