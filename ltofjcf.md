代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uk.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://ht.jctech888.com.cn

TS:   `Hello, ${name}!`
来源：http://jv.huanxung.cn

Java: "Hello, %s!".formatted(name)
来源：http://as.shxzukj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cv.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://xc.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://rn.muxihuayi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://up.asd995.cn

Py:   "第一行\n第二行"
来源：http://lo.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://uk.nicolike.cn

JS:   "第一行\n第二行"
来源：http://en.haigaiapp.cn

TS:   "第一行\n第二行"
来源：http://gs.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://ns.asd995.cn

Go:   "第一行\n第二行"
来源：http://mm.nszjky.cn

Ruby: "第一行\n第二行"
来源：http://lz.colortex.cn

C#:   "第一行\n第二行"
来源：http://dm.huixinmuqiang.cn

[A14] 注释写法
来源：http://zk.nszjky.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://oi.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rh.asd995.cn

JS:   // 单行；/* 多行 */
来源：http://rx.yuexingan06.cn

TS:   // 单行；/* 多行 */
来源：http://mq.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ot.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://dd.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pr.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://cz.colortex.cn

[A15] 空值判断与默认值
来源：http://ql.hahajie.cn

Py:   value = data or "默认值"
来源：http://uu.chemitech.net.cn

PHP:  $value = $data ?? "默认值";
来源：http://de.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://oc.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://cn.asd995.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dq.hahajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://yr.nicolike.cn

Ruby: value = data || "默认值"
来源：http://vp.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://nz.wgjwhj.cn

[A16] 真假值判断规则
来源：http://xs.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hf.9csxet.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lv.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://eo.newstarts.cn

TS:   if (!x) {}
来源：http://kg.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hm.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ii.chemitech.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gn.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ql.bjjhwx.cn

[A17] 位运算
来源：http://ga.wgjwhj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://un.chemitech.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tg.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eh.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zt.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ah.szsharing.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rl.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ts.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uo.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://hr.nicolike.cn

Py:   ord("A"); chr(65)
来源：http://vf.bjjhwx.cn

PHP:  ord("A"); chr(65)
来源：http://wt.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wd.asd995.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vi.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://kk.9csxet.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ne.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://kv.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://os.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://me.huanxung.cn

Py:   a, b = b, a
来源：http://fg.yuntaijiaju.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qv.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://wg.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://fv.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://ce.newstarts.cn

Go:   a, b = b, a
来源：http://hq.wgjwhj.cn

Ruby: a, b = b, a
来源：http://ti.muxihuayi.cn

C#:   (a, b) = (b, a);
来源：http://yn.hahajie.cn

[A20] 读取标准输入
来源：http://rg.jianghongdianzi.cn

Py:   name = input("请输入：")
来源：http://be.haigaiapp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ll.521024.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dx.521024.cn

TS:   // Node.js：readline 模块
来源：http://vc.jctech888.com.cn

Java: new Scanner(System.in).nextLine()
来源：http://em.nszjky.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ui.hahajie.cn

Ruby: gets.chomp
来源：http://db.panjiajie.cn

C#:   Console.ReadLine();
来源：http://mo.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://ta.shxzskj.cn

Py:   f"{3.14159:.2f}"
来源：http://ye.wgjwhj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://la.colortex.cn

JS:   (3.14159).toFixed(2)
来源：http://jd.shxzskj.cn

TS:   (3.14159).toFixed(2)
来源：http://gr.colortex.cn

Java: String.format("%.2f", 3.14159)
来源：http://yb.chemitech.net.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gy.lnxyls.cn

Ruby: format("%.2f", 3.14159)
来源：http://zm.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://kb.521024.cn

[A22] 获取字符串长度
来源：http://bw.szxytkj.cn

Py:   len(s)
来源：http://sk.shxzukj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tz.asd995.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://al.colortex.cn

TS:   s.length
来源：http://rb.shxzskj.cn

Java: s.length()
来源：http://mn.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hl.wgjwhj.cn

Ruby: s.length
来源：http://op.521024.cn

C#:   s.Length
来源：http://tb.colortex.cn

[A23] 大小写转换
来源：http://pc.shxzukj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ed.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ph.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zq.gzmigu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ed.szsharing.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vf.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://od.shxzukj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zz.panjiajie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hn.chemitech.net.cn

[A24] 去除首尾空白
来源：http://kt.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zr.panjiajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dx.521024.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ev.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zk.shtwfgs.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hf.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://pi.asd995.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oc.bookmarksfly.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://re.chemitech.net.cn

[A25] 字符串比较
来源：http://nm.nicolike.cn

Py:   s1 == s2; s1 != s2
来源：http://qi.huanxung.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pe.521024.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://by.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qr.gzmigu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lx.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vx.shxzskj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qq.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lc.huixiangedu.cn

[A26] 类型转换总览
来源：http://mb.shxzukj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ja.shxzukj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mt.gzmigu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uy.muxihuayi.cn

TS:   Number() String() Boolean() x as number
来源：http://rw.521024.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ly.huanxung.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://le.bookmarksfly.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mx.wgjwhj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wt.shtwfgs.cn

================================================================================
来源：http://zs.newstarts.cn

B. 流程控制
来源：http://fc.hnjuh.cn

================================================================================
来源：http://kt.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://dp.shtwfgs.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gr.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://am.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://th.hnjuh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nu.gzmigu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zk.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rn.bookmarksfly.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xy.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ww.nicolike.cn

[B02] 多分支 else if / elif
来源：http://bb.muxihuayi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xy.colortex.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pu.nicolike.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ee.chemitech.net.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bw.huixiangedu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ir.lnxyls.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tr.yuexingan06.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://em.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ya.gzmigu.cn

[B03] switch / match / case
来源：http://oe.nszjky.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://px.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rm.chemitech.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rs.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ru.szsharing.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mj.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bp.haigaiapp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ls.shtwfgs.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.gzmigu.cn

[B04] for 计数循环
来源：http://jw.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://tj.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mt.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yr.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wz.asd995.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qs.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gz.jctech888.com.cn

Ruby: 10.times { |i| puts i }
来源：http://pt.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yg.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://gz.chemitech.net.cn

Py:   for item in arr: print(item)
来源：http://ig.szsharing.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gi.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mt.lnxyls.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cx.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pw.newstarts.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uz.yuntaijiaju.cn

Ruby: arr.each { |item| puts item }
来源：http://im.9csxet.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yu.shtwfgs.cn

[B06] 遍历字典 / 对象
来源：http://qd.lnxyls.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://de.huixinmuqiang.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hl.yuexingan06.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hr.huixinmuqiang.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cr.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ls.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zd.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ar.9csxet.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kn.szsharing.cn

[B07] while 循环
来源：http://fy.nszjky.cn

Py:   while i < 10: i += 1
来源：http://sq.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fz.haigaiapp.cn

JS:   while (i < 10) { i++; }
来源：http://jq.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://bi.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://hm.bjjhwx.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ul.jctech888.com.cn

Ruby: while i < 10; i += 1; end
来源：http://ok.asd995.cn

C#:   while (i < 10) { i++; }
来源：http://ud.huixiangedu.cn

[B08] do-while（至少执行一次）
来源：http://ns.asd995.cn

Py:   # 无 do-while：用 while True + break
来源：http://vs.szxytkj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jk.huanxung.cn

JS:   do { i++; } while (i < 10);
来源：http://em.jctech888.com.cn

TS:   do { i++; } while (i < 10);
来源：http://yc.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://ju.szsharing.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://on.shtwfgs.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xc.newstarts.cn

C#:   do { i++; } while (i < 10);
来源：http://fk.521024.cn

[B09] break 与 continue
来源：http://lb.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ht.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wo.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fk.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jb.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hw.yuntaijiaju.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wi.huixiangedu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jy.colortex.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gu.521024.cn

[B10] 遍历同时拿索引
来源：http://oo.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xy.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zy.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pr.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jw.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://db.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ce.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xd.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qt.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://ji.nicolike.cn

Py:   list(range(0, 10, 2))
来源：http://wm.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://xs.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pv.wgjwhj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hc.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sa.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hl.jianghongdianzi.cn

Ruby: (0...10).step(2).to_a
来源：http://zj.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uq.shtwfgs.cn

[B12] 跳出多层循环
来源：http://nn.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yy.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tr.wgjwhj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ss.hahajie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bs.9csxet.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nz.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lw.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dy.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hw.shxzskj.cn

[B13] 判断是否为数字
来源：http://ls.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://lv.nszjky.cn

PHP:  is_numeric($x)
来源：http://kd.9csxet.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vd.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ot.yuexingan06.cn

Java: x instanceof Number
来源：http://ag.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eu.haigaiapp.cn

Ruby: x.is_a?(Numeric)
来源：http://ci.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://kw.newstarts.cn

[B14] 判断值是否在集合内
来源：http://ou.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ep.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jf.shtwfgs.cn

JS:   [1, 2, 3].includes(x)
来源：http://ia.hahajie.cn

TS:   [1, 2, 3].includes(x)
来源：http://qt.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jq.yuntaijiaju.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zw.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://go.szxytkj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ma.gzmigu.cn

[B15] 布尔运算与取反
来源：http://aq.hahajie.cn

Py:   a and b or not c
来源：http://zu.jctech888.com.cn

PHP:  $a && $b || !$c
来源：http://ke.huixinmuqiang.cn

JS:   a && b || !c
来源：http://gk.szsharing.cn

TS:   a && b || !c
来源：http://wk.muxihuayi.cn

Java: a && b || !c
来源：http://yc.shxzukj.cn

Go:   a && b || !c
来源：http://ah.huixinmuqiang.cn

Ruby: a && b || !c
来源：http://ux.haigaiapp.cn

C#:   a && b || !c
来源：http://pv.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vl.nicolike.cn

Py:   if not data: return
来源：http://ni.huixiangedu.cn

PHP:  if (!$data) { return; }
来源：http://fn.nicolike.cn

JS:   if (!data) return;
来源：http://ud.newstarts.cn

TS:   if (!data) return;
来源：http://lx.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://pt.chemitech.net.cn

Go:   if data == nil { return }
来源：http://jp.huixiangedu.cn

Ruby: return if data.nil?
来源：http://qe.szsharing.cn

C#:   if (data == null) return;
来源：http://ie.jianghongdianzi.cn

================================================================================
来源：http://il.hahajie.cn

C. 函数与作用域
来源：http://sb.bookmarksfly.cn

================================================================================
来源：http://dw.yuexingan06.cn

[C01] 定义函数
来源：http://ix.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://ot.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://td.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://ny.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hy.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://or.nszjky.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ry.hahajie.cn

Ruby: def add(a, b); a + b; end
来源：http://ru.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jb.jianghongdianzi.cn

[C02] 默认参数
来源：http://vv.yuexingan06.cn

Py:   def greet(name="World"): return name
来源：http://gp.huanxung.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uk.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://vo.hnjuh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uq.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kl.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fv.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://ub.haigaiapp.cn


<!-- 参考信息 -->