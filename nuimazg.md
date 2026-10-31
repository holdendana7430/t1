代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gc.asd995.cn

JS:   `Hello, ${name}!`
来源：http://wb.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://fj.asd995.cn

Java: "Hello, %s!".formatted(name)
来源：http://fo.shxzskj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zu.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://sq.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://kp.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://op.newstarts.cn

Py:   "第一行\n第二行"
来源：http://la.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://cw.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://ye.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://sh.lnxyls.cn

Java: "第一行\n第二行"
来源：http://xf.nicolike.cn

Go:   "第一行\n第二行"
来源：http://ct.shxzskj.cn

Ruby: "第一行\n第二行"
来源：http://cg.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://uy.yuexingan06.cn

[A14] 注释写法
来源：http://im.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yr.newstarts.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qp.lnxyls.cn

JS:   // 单行；/* 多行 */
来源：http://nf.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://uc.haigaiapp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dz.9csxet.cn

Go:   // 单行；/* 多行 */
来源：http://oa.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ia.521024.cn

C#:   // 单行；/* 多行 */
来源：http://rq.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://go.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://wt.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://jv.shxzukj.cn

JS:   const value = data ?? "默认值";
来源：http://he.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://kq.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gt.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://bu.szxytkj.cn

Ruby: value = data || "默认值"
来源：http://si.huixiangedu.cn

C#:   var value = data ?? "默认值";
来源：http://ly.haigaiapp.cn

[A16] 真假值判断规则
来源：http://ox.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pe.nicolike.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://iq.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pd.9csxet.cn

TS:   if (!x) {}
来源：http://wb.lnxyls.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ye.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ur.szsharing.cn

Ruby: unless x            # nil 与 false 为假
来源：http://et.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ky.nicolike.cn

[A17] 位运算
来源：http://dv.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iv.bjjhwx.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pz.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ic.szxytkj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://aa.szxytkj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xf.huanxung.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uw.shxzskj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zo.wgjwhj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mn.haigaiapp.cn

[A18] 字符与 ASCII 码互转
来源：http://za.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://xq.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://yd.shxzukj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yc.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fh.shxzukj.cn

Java: (int) 'A'; (char) 65
来源：http://fr.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bl.jctech888.com.cn

Ruby: "A".ord; 65.chr
来源：http://pr.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://ze.hahajie.cn

[A19] 交换两个变量
来源：http://jd.gzmigu.cn

Py:   a, b = b, a
来源：http://tj.szxytkj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vt.shxzskj.cn

JS:   [a, b] = [b, a];
来源：http://tv.haigaiapp.cn

TS:   [a, b] = [b, a];
来源：http://im.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://ms.colortex.cn

Go:   a, b = b, a
来源：http://rd.szxytkj.cn

Ruby: a, b = b, a
来源：http://fn.chemitech.net.cn

C#:   (a, b) = (b, a);
来源：http://xy.521024.cn

[A20] 读取标准输入
来源：http://sd.huixinmuqiang.cn

Py:   name = input("请输入：")
来源：http://hz.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wl.huanxung.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yv.yuntaijiaju.cn

TS:   // Node.js：readline 模块
来源：http://hb.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://sj.huanxung.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xv.huixiangedu.cn

Ruby: gets.chomp
来源：http://ij.huixinmuqiang.cn

C#:   Console.ReadLine();
来源：http://kh.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://jr.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://lg.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zo.jctech888.com.cn

JS:   (3.14159).toFixed(2)
来源：http://uu.nicolike.cn

TS:   (3.14159).toFixed(2)
来源：http://os.haigaiapp.cn

Java: String.format("%.2f", 3.14159)
来源：http://uk.jianghongdianzi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mh.nicolike.cn

Ruby: format("%.2f", 3.14159)
来源：http://wg.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://lo.jctech888.com.cn

[A22] 获取字符串长度
来源：http://ps.9csxet.cn

Py:   len(s)
来源：http://vv.panjiajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sj.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ha.gzmigu.cn

TS:   s.length
来源：http://qp.szxytkj.cn

Java: s.length()
来源：http://ss.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qr.wgjwhj.cn

Ruby: s.length
来源：http://qg.jianghongdianzi.cn

C#:   s.Length
来源：http://zt.shtwfgs.cn

[A23] 大小写转换
来源：http://us.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vp.hnjuh.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gf.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sd.colortex.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ns.yuexingan06.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wm.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kx.huanxung.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qj.asd995.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://mx.shxzukj.cn

[A24] 去除首尾空白
来源：http://la.huixinmuqiang.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ud.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iq.huixiangedu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ew.jctech888.com.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xx.haigaiapp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://aj.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://hz.hahajie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ak.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hr.bjjhwx.cn

[A25] 字符串比较
来源：http://ad.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://sx.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rz.shxzskj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qb.huixinmuqiang.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fa.huanxung.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://li.szxytkj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hm.yuexingan06.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tg.shxzukj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hx.9csxet.cn

[A26] 类型转换总览
来源：http://ll.huanxung.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ek.gzmigu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://et.muxihuayi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ep.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://bp.nicolike.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zd.nicolike.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://js.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gh.bookmarksfly.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://eu.9csxet.cn

================================================================================
来源：http://wo.shtwfgs.cn

B. 流程控制
来源：http://hq.muxihuayi.cn

================================================================================
来源：http://ii.hnjuh.cn

[B01] 条件判断 if / else
来源：http://yd.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yo.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fm.huixiangedu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nq.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ly.jianghongdianzi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ho.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bq.yuntaijiaju.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://in.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fq.bjjhwx.cn

[B02] 多分支 else if / elif
来源：http://pm.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wy.jctech888.com.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nx.jianghongdianzi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lu.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qn.shtwfgs.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ca.521024.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sq.asd995.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zy.huanxung.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ha.huanxung.cn

[B03] switch / match / case
来源：http://bn.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ow.521024.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ta.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wy.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lt.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lp.newstarts.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oe.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qq.shxzskj.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zi.bjjhwx.cn

[B04] for 计数循环
来源：http://zx.shxzukj.cn

Py:   for i in range(10): print(i)
来源：http://mf.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ij.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vq.muxihuayi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bc.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zu.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jl.szxytkj.cn

Ruby: 10.times { |i| puts i }
来源：http://mw.jianghongdianzi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://na.szsharing.cn

[B05] 遍历数组 / 列表
来源：http://jv.shxzukj.cn

Py:   for item in arr: print(item)
来源：http://jz.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://is.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://uw.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pz.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jc.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lz.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://ux.hahajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tx.jctech888.com.cn

[B06] 遍历字典 / 对象
来源：http://en.shtwfgs.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://st.9csxet.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xy.newstarts.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oy.shtwfgs.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ka.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hl.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bw.shxzukj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ql.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ea.asd995.cn

[B07] while 循环
来源：http://nu.gzmigu.cn

Py:   while i < 10: i += 1
来源：http://pg.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ce.shxzskj.cn

JS:   while (i < 10) { i++; }
来源：http://ci.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://fh.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://fp.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vy.huanxung.cn

Ruby: while i < 10; i += 1; end
来源：http://yv.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://ww.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://fx.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://xv.colortex.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://di.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://sl.colortex.cn

TS:   do { i++; } while (i < 10);
来源：http://md.wgjwhj.cn

Java: do { i++; } while (i < 10);
来源：http://lu.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://aq.szxytkj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mw.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://le.shxzukj.cn

[B09] break 与 continue
来源：http://zx.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ov.newstarts.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wl.hnjuh.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wv.9csxet.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eh.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yw.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ry.newstarts.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xf.asd995.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yy.521024.cn

[B10] 遍历同时拿索引
来源：http://bc.newstarts.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fr.jctech888.com.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nn.yuexingan06.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yv.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ob.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cw.wgjwhj.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://id.lnxyls.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gr.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dw.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://fo.newstarts.cn

Py:   list(range(0, 10, 2))
来源：http://nm.newstarts.cn

PHP:  range(0, 10, 2);
来源：http://mq.chemitech.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://im.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xx.muxihuayi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mz.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xz.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://sk.shtwfgs.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ec.shtwfgs.cn

[B12] 跳出多层循环
来源：http://qv.bookmarksfly.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hv.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://np.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qo.shxzukj.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://az.yuntaijiaju.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pv.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ue.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nt.szsharing.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lv.huanxung.cn

[B13] 判断是否为数字
来源：http://de.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://kv.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://zk.shxzukj.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ka.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ge.gzmigu.cn

Java: x instanceof Number
来源：http://wb.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ym.huixinmuqiang.cn

Ruby: x.is_a?(Numeric)
来源：http://ct.lnxyls.cn

C#:   x is int or double or decimal
来源：http://db.asd995.cn

[B14] 判断值是否在集合内
来源：http://wu.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ht.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kt.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://yg.szsharing.cn

TS:   [1, 2, 3].includes(x)
来源：http://ls.gzmigu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ym.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sf.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fb.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bv.newstarts.cn

[B15] 布尔运算与取反
来源：http://bu.huixinmuqiang.cn

Py:   a and b or not c
来源：http://sg.huixinmuqiang.cn

PHP:  $a && $b || !$c
来源：http://mp.chemitech.net.cn

JS:   a && b || !c
来源：http://np.shxzukj.cn

TS:   a && b || !c
来源：http://qs.asd995.cn

Java: a && b || !c
来源：http://bt.hnjuh.cn

Go:   a && b || !c
来源：http://ux.szsharing.cn

Ruby: a && b || !c
来源：http://gy.521024.cn

C#:   a && b || !c
来源：http://pl.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gf.hnjuh.cn

Py:   if not data: return
来源：http://xq.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://ae.hnjuh.cn

JS:   if (!data) return;
来源：http://yv.bookmarksfly.cn

TS:   if (!data) return;
来源：http://jj.hnjuh.cn

Java: if (data == null) return;
来源：http://we.521024.cn

Go:   if data == nil { return }
来源：http://kz.newstarts.cn

Ruby: return if data.nil?
来源：http://br.panjiajie.cn

C#:   if (data == null) return;
来源：http://oc.haigaiapp.cn

================================================================================
来源：http://tw.bookmarksfly.cn

C. 函数与作用域
来源：http://xs.yuexingan06.cn

================================================================================
来源：http://ox.muxihuayi.cn

[C01] 定义函数
来源：http://ri.521024.cn

Py:   def add(a, b): return a + b
来源：http://jj.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jx.jianghongdianzi.cn

JS:   function add(a, b) { return a + b; }
来源：http://ft.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yx.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yu.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ic.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://hu.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://us.huanxung.cn

[C02] 默认参数
来源：http://ho.nicolike.cn

Py:   def greet(name="World"): return name
来源：http://vt.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vb.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://hy.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bk.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rj.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xp.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://lt.yuntaijiaju.cn


<!-- 参考信息 -->