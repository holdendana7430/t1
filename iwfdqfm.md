代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://pi.jctech888.com.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ze.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://vv.szxytkj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://re.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rr.hnjuh.cn

JS:   `Hello, ${name}!`
来源：http://ur.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://ip.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://hz.huixiangedu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rb.yuntaijiaju.cn

Ruby: "Hello, #{name}!"
来源：http://lj.bookmarksfly.cn

C#:   $"Hello, {name}!"
来源：http://wc.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://eu.chemitech.net.cn

Py:   "第一行\n第二行"
来源：http://bg.shtwfgs.cn

PHP:  "第一行\n第二行"
来源：http://tk.gzmigu.cn

JS:   "第一行\n第二行"
来源：http://ta.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://pb.nszjky.cn

Java: "第一行\n第二行"
来源：http://km.nicolike.cn

Go:   "第一行\n第二行"
来源：http://dg.bookmarksfly.cn

Ruby: "第一行\n第二行"
来源：http://ye.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://dv.colortex.cn

[A14] 注释写法
来源：http://nf.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vw.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ph.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://wm.haigaiapp.cn

TS:   // 单行；/* 多行 */
来源：http://oq.huanxung.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fv.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://pz.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tr.bjjhwx.cn

C#:   // 单行；/* 多行 */
来源：http://wn.asd995.cn

[A15] 空值判断与默认值
来源：http://uq.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://qh.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://br.asd995.cn

JS:   const value = data ?? "默认值";
来源：http://xp.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://oh.shxzukj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ku.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://ns.9csxet.cn

Ruby: value = data || "默认值"
来源：http://zv.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://zx.szxytkj.cn

[A16] 真假值判断规则
来源：http://ix.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xv.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ue.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ie.asd995.cn

TS:   if (!x) {}
来源：http://gh.jctech888.com.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gq.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xu.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://am.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://if.9csxet.cn

[A17] 位运算
来源：http://so.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xr.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rf.szxytkj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ou.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zo.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xu.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gi.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sq.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yx.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://hl.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://et.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://og.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zj.szxytkj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qc.newstarts.cn

Java: (int) 'A'; (char) 65
来源：http://pc.nszjky.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oi.lnxyls.cn

Ruby: "A".ord; 65.chr
来源：http://cm.hnjuh.cn

C#:   (int)'A'; (char)65
来源：http://uv.muxihuayi.cn

[A19] 交换两个变量
来源：http://sl.521024.cn

Py:   a, b = b, a
来源：http://yo.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ra.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://jz.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://tn.nicolike.cn

Java: int t = a; a = b; b = t;
来源：http://kp.shxzskj.cn

Go:   a, b = b, a
来源：http://io.lnxyls.cn

Ruby: a, b = b, a
来源：http://wq.newstarts.cn

C#:   (a, b) = (b, a);
来源：http://yh.9csxet.cn

[A20] 读取标准输入
来源：http://pl.yuntaijiaju.cn

Py:   name = input("请输入：")
来源：http://wu.wgjwhj.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kq.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gt.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://kt.yuntaijiaju.cn

Java: new Scanner(System.in).nextLine()
来源：http://oq.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vv.yuexingan06.cn

Ruby: gets.chomp
来源：http://du.haigaiapp.cn

C#:   Console.ReadLine();
来源：http://qe.haigaiapp.cn

[A21] 保留指定小数位输出
来源：http://xu.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://wk.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dx.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://zw.hahajie.cn

TS:   (3.14159).toFixed(2)
来源：http://qa.chemitech.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://ld.nicolike.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vo.muxihuayi.cn

Ruby: format("%.2f", 3.14159)
来源：http://qr.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://qw.colortex.cn

[A22] 获取字符串长度
来源：http://du.9csxet.cn

Py:   len(s)
来源：http://dp.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ud.yuntaijiaju.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zw.yuntaijiaju.cn

TS:   s.length
来源：http://zc.yuexingan06.cn

Java: s.length()
来源：http://uf.jianghongdianzi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ss.nszjky.cn

Ruby: s.length
来源：http://fg.jctech888.com.cn

C#:   s.Length
来源：http://jt.yuexingan06.cn

[A23] 大小写转换
来源：http://dx.huixinmuqiang.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ha.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ci.bookmarksfly.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vy.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yo.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hx.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wk.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rz.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cq.shxzukj.cn

[A24] 去除首尾空白
来源：http://xt.shtwfgs.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wr.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ea.szxytkj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yh.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pa.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fm.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://uy.gzmigu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cb.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://or.shtwfgs.cn

[A25] 字符串比较
来源：http://jh.huanxung.cn

Py:   s1 == s2; s1 != s2
来源：http://ys.bookmarksfly.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vs.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tk.huixiangedu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cy.szsharing.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rr.bookmarksfly.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mr.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fe.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zn.lnxyls.cn

[A26] 类型转换总览
来源：http://fb.hahajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://el.huanxung.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sq.jctech888.com.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ri.huixinmuqiang.cn

TS:   Number() String() Boolean() x as number
来源：http://at.szsharing.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ks.shtwfgs.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vn.shxzukj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jb.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ki.shtwfgs.cn

================================================================================
来源：http://ra.haigaiapp.cn

B. 流程控制
来源：http://gb.shxzukj.cn

================================================================================
来源：http://wz.jianghongdianzi.cn

[B01] 条件判断 if / else
来源：http://ph.newstarts.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://er.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nn.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wu.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tn.asd995.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kr.newstarts.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://md.szxytkj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://js.muxihuayi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bq.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://ow.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nv.hnjuh.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ne.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pz.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jy.521024.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sc.nicolike.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bf.gzmigu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ke.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jc.huixiangedu.cn

[B03] switch / match / case
来源：http://xk.szxytkj.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://po.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cf.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ss.bookmarksfly.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vo.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cy.colortex.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eo.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uc.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cb.hahajie.cn

[B04] for 计数循环
来源：http://dy.jctech888.com.cn

Py:   for i in range(10): print(i)
来源：http://ty.nicolike.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bt.szxytkj.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lk.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bm.colortex.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yw.hnjuh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ny.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://od.shxzskj.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mt.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://eo.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://ft.shtwfgs.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tc.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oy.colortex.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nj.shtwfgs.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zh.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pe.szxytkj.cn

Ruby: arr.each { |item| puts item }
来源：http://un.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ha.nszjky.cn

[B06] 遍历字典 / 对象
来源：http://fr.szsharing.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hr.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oj.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mf.muxihuayi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eo.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://je.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lo.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://al.yuntaijiaju.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ky.newstarts.cn

[B07] while 循环
来源：http://ug.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://ac.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://do.nszjky.cn

JS:   while (i < 10) { i++; }
来源：http://ay.hahajie.cn

TS:   while (i < 10) { i++; }
来源：http://mj.szsharing.cn

Java: while (i < 10) { i++; }
来源：http://ih.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oc.bookmarksfly.cn

Ruby: while i < 10; i += 1; end
来源：http://kz.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://xx.chemitech.net.cn

[B08] do-while（至少执行一次）
来源：http://kc.chemitech.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://fr.521024.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://of.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://rk.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://do.yuntaijiaju.cn

Java: do { i++; } while (i < 10);
来源：http://be.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pw.colortex.cn

Ruby: begin; i += 1; end while i < 10
来源：http://sx.yuexingan06.cn

C#:   do { i++; } while (i < 10);
来源：http://om.gzmigu.cn

[B09] break 与 continue
来源：http://tq.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hc.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xj.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oo.jianghongdianzi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jc.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nj.newstarts.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uo.muxihuayi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jc.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nw.bookmarksfly.cn

[B10] 遍历同时拿索引
来源：http://ha.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xl.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ob.huanxung.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wj.huanxung.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oh.nszjky.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jq.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ac.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hk.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ah.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://ko.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://kz.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://ru.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ic.szxytkj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nc.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yn.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bp.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://xn.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rq.huixiangedu.cn

[B12] 跳出多层循环
来源：http://pg.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ax.bookmarksfly.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vt.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yr.wgjwhj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ru.huixinmuqiang.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ua.nszjky.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vm.huanxung.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nw.huanxung.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://to.huixiangedu.cn

[B13] 判断是否为数字
来源：http://ih.9csxet.cn

Py:   isinstance(x, (int, float))
来源：http://ka.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://zf.colortex.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yr.shtwfgs.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gq.bjjhwx.cn

Java: x instanceof Number
来源：http://do.shxzskj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fp.yuexingan06.cn

Ruby: x.is_a?(Numeric)
来源：http://gf.colortex.cn

C#:   x is int or double or decimal
来源：http://nr.newstarts.cn

[B14] 判断值是否在集合内
来源：http://lw.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cc.asd995.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yu.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://sj.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://na.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mj.asd995.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://as.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dm.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bz.colortex.cn

[B15] 布尔运算与取反
来源：http://mm.newstarts.cn

Py:   a and b or not c
来源：http://li.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://zr.nicolike.cn

JS:   a && b || !c
来源：http://sh.wgjwhj.cn

TS:   a && b || !c
来源：http://px.asd995.cn

Java: a && b || !c
来源：http://ex.yuexingan06.cn

Go:   a && b || !c
来源：http://tj.wgjwhj.cn

Ruby: a && b || !c
来源：http://tw.nicolike.cn

C#:   a && b || !c
来源：http://ac.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yd.haigaiapp.cn

Py:   if not data: return
来源：http://dl.nicolike.cn

PHP:  if (!$data) { return; }
来源：http://wg.bjjhwx.cn

JS:   if (!data) return;
来源：http://lx.hahajie.cn

TS:   if (!data) return;
来源：http://jq.gzmigu.cn

Java: if (data == null) return;
来源：http://bl.nicolike.cn

Go:   if data == nil { return }
来源：http://gj.jctech888.com.cn

Ruby: return if data.nil?
来源：http://gz.hahajie.cn

C#:   if (data == null) return;
来源：http://rw.szxytkj.cn

================================================================================
来源：http://nx.jctech888.com.cn

C. 函数与作用域
来源：http://ju.bookmarksfly.cn

================================================================================
来源：http://fs.9csxet.cn

[C01] 定义函数
来源：http://or.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://dt.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nr.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://vd.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gt.huixiangedu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ui.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://si.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://yo.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dp.jianghongdianzi.cn

[C02] 默认参数
来源：http://qs.huixiangedu.cn

Py:   def greet(name="World"): return name
来源：http://yc.hnjuh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uz.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://lh.jianghongdianzi.cn


<!-- 参考信息 -->