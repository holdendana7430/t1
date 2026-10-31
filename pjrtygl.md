代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://nb.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://ow.hahajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://xi.chemitech.net.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ku.gzmigu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xd.hahajie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fk.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://hd.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wl.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rr.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vn.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://fw.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gh.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gc.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://rt.huanxung.cn

TS:   `Hello, ${name}!`
来源：http://dt.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://uv.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bg.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://fu.shxzukj.cn

C#:   $"Hello, {name}!"
来源：http://py.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jg.hnjuh.cn

Py:   "第一行\n第二行"
来源：http://ts.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://zh.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://ts.lnxyls.cn

TS:   "第一行\n第二行"
来源：http://my.huixinmuqiang.cn

Java: "第一行\n第二行"
来源：http://ml.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://du.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://jg.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://yn.panjiajie.cn

[A14] 注释写法
来源：http://sy.nszjky.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gr.huixiangedu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vd.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://bb.szsharing.cn

TS:   // 单行；/* 多行 */
来源：http://sc.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gc.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://ij.gzmigu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://te.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://rh.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://nz.asd995.cn

Py:   value = data or "默认值"
来源：http://sp.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://wu.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://vj.huixiangedu.cn

TS:   const value = data ?? "默认值";
来源：http://ot.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uj.nszjky.cn

Go:   if data == "" { data = "默认值" }
来源：http://pr.hahajie.cn

Ruby: value = data || "默认值"
来源：http://vq.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://nc.muxihuayi.cn

[A16] 真假值判断规则
来源：http://sq.szxytkj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vg.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qs.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vy.panjiajie.cn

TS:   if (!x) {}
来源：http://ob.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zp.9csxet.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pi.9csxet.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oj.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://el.gzmigu.cn

[A17] 位运算
来源：http://xu.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://il.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ys.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zb.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xf.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fi.muxihuayi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ph.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://et.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rg.wgjwhj.cn

[A18] 字符与 ASCII 码互转
来源：http://xf.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://le.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://mm.szxytkj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ro.hahajie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ey.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://ne.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jo.colortex.cn

Ruby: "A".ord; 65.chr
来源：http://gx.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://po.hahajie.cn

[A19] 交换两个变量
来源：http://lt.9csxet.cn

Py:   a, b = b, a
来源：http://te.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ac.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://ig.chemitech.net.cn

TS:   [a, b] = [b, a];
来源：http://xc.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://wq.yuexingan06.cn

Go:   a, b = b, a
来源：http://yg.shxzukj.cn

Ruby: a, b = b, a
来源：http://pc.bookmarksfly.cn

C#:   (a, b) = (b, a);
来源：http://ny.gzmigu.cn

[A20] 读取标准输入
来源：http://as.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://pt.lnxyls.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zj.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fn.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://ni.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://lq.lnxyls.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jq.shxzukj.cn

Ruby: gets.chomp
来源：http://cy.nicolike.cn

C#:   Console.ReadLine();
来源：http://fc.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://it.wgjwhj.cn

Py:   f"{3.14159:.2f}"
来源：http://ir.nszjky.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hi.panjiajie.cn

JS:   (3.14159).toFixed(2)
来源：http://vm.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://td.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://mb.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hm.hnjuh.cn

Ruby: format("%.2f", 3.14159)
来源：http://ef.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://wm.newstarts.cn

[A22] 获取字符串长度
来源：http://py.hnjuh.cn

Py:   len(s)
来源：http://ay.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gi.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oe.lnxyls.cn

TS:   s.length
来源：http://vo.huixinmuqiang.cn

Java: s.length()
来源：http://nc.jctech888.com.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cv.szsharing.cn

Ruby: s.length
来源：http://th.shxzskj.cn

C#:   s.Length
来源：http://mo.shxzukj.cn

[A23] 大小写转换
来源：http://qd.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ie.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ol.newstarts.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bt.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xt.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://he.hnjuh.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://py.9csxet.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kd.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tn.jctech888.com.cn

[A24] 去除首尾空白
来源：http://ur.hahajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oq.bjjhwx.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xu.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fh.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://at.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pr.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://hr.muxihuayi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fn.shxzskj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uf.yuexingan06.cn

[A25] 字符串比较
来源：http://jj.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://jf.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xx.nszjky.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qb.hahajie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xi.shtwfgs.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mq.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xz.newstarts.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nb.9csxet.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fe.nicolike.cn

[A26] 类型转换总览
来源：http://zc.hnjuh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://iu.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pv.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tg.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://sz.yuntaijiaju.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://og.bookmarksfly.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yj.panjiajie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dt.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ti.yuntaijiaju.cn

================================================================================
来源：http://ec.yuexingan06.cn

B. 流程控制
来源：http://xv.shxzskj.cn

================================================================================
来源：http://ms.panjiajie.cn

[B01] 条件判断 if / else
来源：http://nq.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ju.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pn.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iw.panjiajie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mo.colortex.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rz.jianghongdianzi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fh.shxzukj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hk.yuntaijiaju.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vz.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://sa.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kc.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fk.nszjky.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yu.shxzskj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://re.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://la.huixiangedu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ty.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ee.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://em.lnxyls.cn

[B03] switch / match / case
来源：http://nw.shxzskj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nv.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xb.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sm.colortex.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gw.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fz.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yg.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uw.szxytkj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zy.shxzukj.cn

[B04] for 计数循环
来源：http://mu.wgjwhj.cn

Py:   for i in range(10): print(i)
来源：http://rw.asd995.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dt.bjjhwx.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://he.shxzskj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ht.yuntaijiaju.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hm.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zd.colortex.cn

Ruby: 10.times { |i| puts i }
来源：http://gj.newstarts.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://go.jianghongdianzi.cn

[B05] 遍历数组 / 列表
来源：http://kd.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://dv.shxzukj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jj.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zg.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zl.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tw.yuntaijiaju.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ot.muxihuayi.cn

Ruby: arr.each { |item| puts item }
来源：http://oo.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lx.nicolike.cn

[B06] 遍历字典 / 对象
来源：http://iq.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ua.shxzukj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://el.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rk.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qc.panjiajie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ox.nszjky.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vg.hahajie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wb.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gn.521024.cn

[B07] while 循环
来源：http://gv.hnjuh.cn

Py:   while i < 10: i += 1
来源：http://ma.asd995.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hz.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://be.yuexingan06.cn

TS:   while (i < 10) { i++; }
来源：http://do.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://de.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eh.521024.cn

Ruby: while i < 10; i += 1; end
来源：http://cn.newstarts.cn

C#:   while (i < 10) { i++; }
来源：http://yh.szxytkj.cn

[B08] do-while（至少执行一次）
来源：http://rd.haigaiapp.cn

Py:   # 无 do-while：用 while True + break
来源：http://op.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eq.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://bc.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://nq.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://bl.jianghongdianzi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uj.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xb.hnjuh.cn

C#:   do { i++; } while (i < 10);
来源：http://ht.shtwfgs.cn

[B09] break 与 continue
来源：http://pl.bjjhwx.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://er.yuntaijiaju.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dc.jianghongdianzi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vo.shtwfgs.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fp.yuntaijiaju.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sa.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wj.szxytkj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vj.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jj.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://ll.panjiajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rh.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mc.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ig.shxzskj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qm.bjjhwx.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://az.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sb.huanxung.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sz.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gm.yuexingan06.cn

[B11] 生成数字序列 / 区间
来源：http://hp.wgjwhj.cn

Py:   list(range(0, 10, 2))
来源：http://wf.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://ru.szsharing.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zh.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jg.wgjwhj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://et.nicolike.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gw.gzmigu.cn

Ruby: (0...10).step(2).to_a
来源：http://rn.yuntaijiaju.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ag.bookmarksfly.cn

[B12] 跳出多层循环
来源：http://du.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ab.asd995.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://rm.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tb.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nn.colortex.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bu.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mr.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hs.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bo.gzmigu.cn

[B13] 判断是否为数字
来源：http://eq.521024.cn

Py:   isinstance(x, (int, float))
来源：http://fa.szsharing.cn

PHP:  is_numeric($x)
来源：http://hq.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ba.nszjky.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pg.chemitech.net.cn

Java: x instanceof Number
来源：http://zr.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mu.hahajie.cn

Ruby: x.is_a?(Numeric)
来源：http://vx.muxihuayi.cn

C#:   x is int or double or decimal
来源：http://zd.huanxung.cn

[B14] 判断值是否在集合内
来源：http://mt.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sx.shxzukj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zr.colortex.cn

JS:   [1, 2, 3].includes(x)
来源：http://gn.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://pk.wgjwhj.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ym.haigaiapp.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ri.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qm.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nh.shxzskj.cn

[B15] 布尔运算与取反
来源：http://id.szsharing.cn

Py:   a and b or not c
来源：http://pe.shxzskj.cn

PHP:  $a && $b || !$c
来源：http://ym.panjiajie.cn

JS:   a && b || !c
来源：http://zn.yuntaijiaju.cn

TS:   a && b || !c
来源：http://ys.muxihuayi.cn

Java: a && b || !c
来源：http://oc.muxihuayi.cn

Go:   a && b || !c
来源：http://ej.wgjwhj.cn

Ruby: a && b || !c
来源：http://tq.szsharing.cn

C#:   a && b || !c
来源：http://nk.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ow.chemitech.net.cn

Py:   if not data: return
来源：http://la.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://zz.9csxet.cn

JS:   if (!data) return;
来源：http://qs.newstarts.cn

TS:   if (!data) return;
来源：http://bv.shxzukj.cn

Java: if (data == null) return;
来源：http://qe.haigaiapp.cn

Go:   if data == nil { return }
来源：http://wa.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://kn.yuexingan06.cn

C#:   if (data == null) return;
来源：http://mg.yuexingan06.cn

================================================================================
来源：http://xa.yuntaijiaju.cn

C. 函数与作用域
来源：http://bh.szsharing.cn

================================================================================
来源：http://iz.hnjuh.cn

[C01] 定义函数
来源：http://aw.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://yj.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tw.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://rk.shxzukj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ye.bjjhwx.cn


<!-- 参考信息 -->