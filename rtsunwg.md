代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://cj.shtwfgs.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ui.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://hh.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gn.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://ni.panjiajie.cn

[A15] 空值判断与默认值
来源：http://ii.521024.cn

Py:   value = data or "默认值"
来源：http://au.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://zo.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://vc.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://hi.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qd.nszjky.cn

Go:   if data == "" { data = "默认值" }
来源：http://ww.shxzukj.cn

Ruby: value = data || "默认值"
来源：http://ye.yuntaijiaju.cn

C#:   var value = data ?? "默认值";
来源：http://ea.yuexingan06.cn

[A16] 真假值判断规则
来源：http://te.wgjwhj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qa.shtwfgs.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pz.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vr.muxihuayi.cn

TS:   if (!x) {}
来源：http://pc.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qo.asd995.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qg.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hi.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xg.asd995.cn

[A17] 位运算
来源：http://yi.lnxyls.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hx.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tb.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yf.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://eo.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gf.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://he.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ap.hahajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hg.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://ly.9csxet.cn

Py:   ord("A"); chr(65)
来源：http://mq.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://lx.colortex.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fp.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ek.shxzskj.cn

Java: (int) 'A'; (char) 65
来源：http://zf.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lk.shxzukj.cn

Ruby: "A".ord; 65.chr
来源：http://mv.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://hm.haigaiapp.cn

[A19] 交换两个变量
来源：http://mv.521024.cn

Py:   a, b = b, a
来源：http://rr.huixinmuqiang.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hx.yuexingan06.cn

JS:   [a, b] = [b, a];
来源：http://wr.asd995.cn

TS:   [a, b] = [b, a];
来源：http://eu.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://gx.9csxet.cn

Go:   a, b = b, a
来源：http://tm.nicolike.cn

Ruby: a, b = b, a
来源：http://ic.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://qo.yuntaijiaju.cn

[A20] 读取标准输入
来源：http://eu.hnjuh.cn

Py:   name = input("请输入：")
来源：http://vx.asd995.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ms.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lj.szsharing.cn

TS:   // Node.js：readline 模块
来源：http://kq.haigaiapp.cn

Java: new Scanner(System.in).nextLine()
来源：http://ea.jctech888.com.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://me.hahajie.cn

Ruby: gets.chomp
来源：http://jd.huanxung.cn

C#:   Console.ReadLine();
来源：http://hf.colortex.cn

[A21] 保留指定小数位输出
来源：http://ar.huanxung.cn

Py:   f"{3.14159:.2f}"
来源：http://is.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kp.9csxet.cn

JS:   (3.14159).toFixed(2)
来源：http://aw.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://xo.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://hg.huanxung.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tw.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://nl.huixinmuqiang.cn

C#:   3.14159.ToString("F2")
来源：http://ok.nszjky.cn

[A22] 获取字符串长度
来源：http://vi.jianghongdianzi.cn

Py:   len(s)
来源：http://gk.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xf.bookmarksfly.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ba.yuntaijiaju.cn

TS:   s.length
来源：http://xq.yuntaijiaju.cn

Java: s.length()
来源：http://qr.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jl.muxihuayi.cn

Ruby: s.length
来源：http://lb.nszjky.cn

C#:   s.Length
来源：http://ju.haigaiapp.cn

[A23] 大小写转换
来源：http://pe.szsharing.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qu.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wd.chemitech.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bp.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ar.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kk.wgjwhj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dp.chemitech.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pw.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fx.bjjhwx.cn

[A24] 去除首尾空白
来源：http://zm.gzmigu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://or.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bj.gzmigu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ee.bjjhwx.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rg.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nb.wgjwhj.cn

Go:   strings.TrimSpace(s)
来源：http://pd.hnjuh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sp.521024.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rr.asd995.cn

[A25] 字符串比较
来源：http://by.shxzskj.cn

Py:   s1 == s2; s1 != s2
来源：http://wm.newstarts.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uw.szsharing.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gv.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cu.yuexingan06.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bp.shtwfgs.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ie.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://da.gzmigu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ku.panjiajie.cn

[A26] 类型转换总览
来源：http://pe.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kt.jianghongdianzi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lv.shxzukj.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kv.bjjhwx.cn

TS:   Number() String() Boolean() x as number
来源：http://fa.nszjky.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bh.muxihuayi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xq.9csxet.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cy.huixinmuqiang.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nb.nicolike.cn

================================================================================
来源：http://ox.szsharing.cn

B. 流程控制
来源：http://qb.haigaiapp.cn

================================================================================
来源：http://vy.521024.cn

[B01] 条件判断 if / else
来源：http://bk.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bx.huanxung.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cp.chemitech.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ra.shxzskj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ug.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vw.wgjwhj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oe.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pn.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xt.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://gm.huanxung.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pw.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nj.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dw.newstarts.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xx.huanxung.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xc.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ed.colortex.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://la.wgjwhj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vo.nicolike.cn

[B03] switch / match / case
来源：http://bj.chemitech.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uo.szxytkj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pa.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bm.asd995.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xx.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tu.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tl.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://op.jctech888.com.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tr.bookmarksfly.cn

[B04] for 计数循环
来源：http://uc.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://hr.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://av.shtwfgs.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fi.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://of.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ct.colortex.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://br.yuntaijiaju.cn

Ruby: 10.times { |i| puts i }
来源：http://ap.huixinmuqiang.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rg.yuntaijiaju.cn

[B05] 遍历数组 / 列表
来源：http://js.szsharing.cn

Py:   for item in arr: print(item)
来源：http://wp.bjjhwx.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://od.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kc.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xu.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lf.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://by.9csxet.cn

Ruby: arr.each { |item| puts item }
来源：http://rm.hnjuh.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ru.huixiangedu.cn

[B06] 遍历字典 / 对象
来源：http://aq.colortex.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mg.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://si.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uz.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dz.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zn.huixiangedu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dn.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://am.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cz.newstarts.cn

[B07] while 循环
来源：http://cr.hahajie.cn

Py:   while i < 10: i += 1
来源：http://jn.gzmigu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zg.lnxyls.cn

JS:   while (i < 10) { i++; }
来源：http://zf.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://tb.shxzukj.cn

Java: while (i < 10) { i++; }
来源：http://xz.jianghongdianzi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wg.huixiangedu.cn

Ruby: while i < 10; i += 1; end
来源：http://er.shxzukj.cn

C#:   while (i < 10) { i++; }
来源：http://su.panjiajie.cn

[B08] do-while（至少执行一次）
来源：http://zq.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://ip.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ar.gzmigu.cn

JS:   do { i++; } while (i < 10);
来源：http://ir.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://zu.chemitech.net.cn

Java: do { i++; } while (i < 10);
来源：http://cp.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oq.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ok.szxytkj.cn

C#:   do { i++; } while (i < 10);
来源：http://ti.muxihuayi.cn

[B09] break 与 continue
来源：http://sd.szsharing.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mv.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hi.newstarts.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fy.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oj.9csxet.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ay.panjiajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fp.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qb.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ua.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://dd.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hl.hnjuh.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dj.yuntaijiaju.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sd.nszjky.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wl.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://do.hahajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qa.asd995.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xm.lnxyls.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ss.chemitech.net.cn

[B11] 生成数字序列 / 区间
来源：http://ud.huixinmuqiang.cn

Py:   list(range(0, 10, 2))
来源：http://bx.gzmigu.cn

PHP:  range(0, 10, 2);
来源：http://ry.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wh.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yz.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tg.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wo.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://zp.jctech888.com.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ss.hnjuh.cn

[B12] 跳出多层循环
来源：http://ri.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://li.yuntaijiaju.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zl.huanxung.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rv.nszjky.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sx.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dc.chemitech.net.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ov.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://db.hahajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tz.bjjhwx.cn

[B13] 判断是否为数字
来源：http://vc.bjjhwx.cn

Py:   isinstance(x, (int, float))
来源：http://of.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://fy.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wj.szxytkj.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vm.nicolike.cn

Java: x instanceof Number
来源：http://ot.newstarts.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rb.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://ma.huixiangedu.cn

C#:   x is int or double or decimal
来源：http://ii.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://hd.shxzskj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ft.wgjwhj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wa.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://tp.nszjky.cn

TS:   [1, 2, 3].includes(x)
来源：http://xm.bjjhwx.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kg.huanxung.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://se.yuntaijiaju.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qy.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wc.hnjuh.cn

[B15] 布尔运算与取反
来源：http://ff.asd995.cn

Py:   a and b or not c
来源：http://tv.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://zz.jianghongdianzi.cn

JS:   a && b || !c
来源：http://tv.shxzskj.cn

TS:   a && b || !c
来源：http://ze.hnjuh.cn

Java: a && b || !c
来源：http://cb.shxzskj.cn

Go:   a && b || !c
来源：http://so.lnxyls.cn

Ruby: a && b || !c
来源：http://zl.nszjky.cn

C#:   a && b || !c
来源：http://id.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mc.colortex.cn

Py:   if not data: return
来源：http://mv.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://zg.haigaiapp.cn

JS:   if (!data) return;
来源：http://vv.huixinmuqiang.cn

TS:   if (!data) return;
来源：http://bs.huixinmuqiang.cn

Java: if (data == null) return;
来源：http://hu.muxihuayi.cn

Go:   if data == nil { return }
来源：http://fb.521024.cn

Ruby: return if data.nil?
来源：http://cz.hnjuh.cn

C#:   if (data == null) return;
来源：http://fu.521024.cn

================================================================================
来源：http://ju.lnxyls.cn

C. 函数与作用域
来源：http://tu.huanxung.cn

================================================================================
来源：http://bc.panjiajie.cn

[C01] 定义函数
来源：http://fx.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://ro.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fu.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://bz.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xf.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ks.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fw.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://dr.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://la.hnjuh.cn

[C02] 默认参数
来源：http://zi.bjjhwx.cn

Py:   def greet(name="World"): return name
来源：http://fk.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://du.colortex.cn

JS:   function greet(name = "World") { return name; }
来源：http://jw.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vs.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dd.chemitech.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bq.jctech888.com.cn

Ruby: def greet(name = "World") = name
来源：http://ve.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://hy.nicolike.cn

[C03] 可变参数
来源：http://fz.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://ls.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dm.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iw.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ch.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fd.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kp.9csxet.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lq.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hy.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://cn.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eh.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ie.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zh.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://es.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://kp.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://rw.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://bf.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://vf.asd995.cn

[C05] 返回多个值
来源：http://pu.szxytkj.cn


<!-- 参考信息 -->