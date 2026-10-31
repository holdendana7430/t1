代发 wailian999

Java: "第一行\n第二行"
来源：http://ex.yuntaijiaju.cn

Go:   "第一行\n第二行"
来源：http://da.nicolike.cn

Ruby: "第一行\n第二行"
来源：http://mn.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://jx.shxzukj.cn

[A14] 注释写法
来源：http://qp.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fy.asd995.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tl.panjiajie.cn

JS:   // 单行；/* 多行 */
来源：http://tp.bjjhwx.cn

TS:   // 单行；/* 多行 */
来源：http://fu.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sj.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://uy.asd995.cn

Ruby: # 单行；=begin 多行 =end
来源：http://cx.jctech888.com.cn

C#:   // 单行；/* 多行 */
来源：http://mk.9csxet.cn

[A15] 空值判断与默认值
来源：http://ep.521024.cn

Py:   value = data or "默认值"
来源：http://ya.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://mp.yuntaijiaju.cn

JS:   const value = data ?? "默认值";
来源：http://zl.shxzskj.cn

TS:   const value = data ?? "默认值";
来源：http://ut.yuntaijiaju.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nn.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://oz.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://ri.bookmarksfly.cn

C#:   var value = data ?? "默认值";
来源：http://fw.newstarts.cn

[A16] 真假值判断规则
来源：http://jf.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nf.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ig.panjiajie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rs.huixinmuqiang.cn

TS:   if (!x) {}
来源：http://wx.colortex.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xp.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ht.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cn.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://md.hahajie.cn

[A17] 位运算
来源：http://sk.szsharing.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wt.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pl.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ji.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lz.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hi.colortex.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://az.chemitech.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yh.wgjwhj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jj.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://hz.hnjuh.cn

Py:   ord("A"); chr(65)
来源：http://br.bookmarksfly.cn

PHP:  ord("A"); chr(65)
来源：http://pa.bookmarksfly.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cy.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://da.shtwfgs.cn

Java: (int) 'A'; (char) 65
来源：http://vv.shxzukj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cl.szsharing.cn

Ruby: "A".ord; 65.chr
来源：http://np.hahajie.cn

C#:   (int)'A'; (char)65
来源：http://cu.jctech888.com.cn

[A19] 交换两个变量
来源：http://rx.shxzukj.cn

Py:   a, b = b, a
来源：http://tx.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mu.nszjky.cn

JS:   [a, b] = [b, a];
来源：http://ea.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://yx.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://tz.wgjwhj.cn

Go:   a, b = b, a
来源：http://zw.hnjuh.cn

Ruby: a, b = b, a
来源：http://xx.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://hh.hnjuh.cn

[A20] 读取标准输入
来源：http://ji.wgjwhj.cn

Py:   name = input("请输入：")
来源：http://ga.gzmigu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ei.bookmarksfly.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bz.panjiajie.cn

TS:   // Node.js：readline 模块
来源：http://fe.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://dx.521024.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ny.panjiajie.cn

Ruby: gets.chomp
来源：http://jp.jianghongdianzi.cn

C#:   Console.ReadLine();
来源：http://sm.nszjky.cn

[A21] 保留指定小数位输出
来源：http://aw.bookmarksfly.cn

Py:   f"{3.14159:.2f}"
来源：http://vd.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://se.bjjhwx.cn

JS:   (3.14159).toFixed(2)
来源：http://hm.9csxet.cn

TS:   (3.14159).toFixed(2)
来源：http://ii.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://pe.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lj.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://bc.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://rc.chemitech.net.cn

[A22] 获取字符串长度
来源：http://ax.wgjwhj.cn

Py:   len(s)
来源：http://xb.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qt.nszjky.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rq.haigaiapp.cn

TS:   s.length
来源：http://ww.asd995.cn

Java: s.length()
来源：http://qu.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sd.jianghongdianzi.cn

Ruby: s.length
来源：http://rz.huixinmuqiang.cn

C#:   s.Length
来源：http://qm.colortex.cn

[A23] 大小写转换
来源：http://gp.asd995.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hu.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sb.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uz.shxzskj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tu.hahajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iu.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ia.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ha.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jl.gzmigu.cn

[A24] 去除首尾空白
来源：http://lx.shxzskj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bn.chemitech.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sj.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://be.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lu.huixinmuqiang.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uh.newstarts.cn

Go:   strings.TrimSpace(s)
来源：http://ib.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vl.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xv.huanxung.cn

[A25] 字符串比较
来源：http://ht.bookmarksfly.cn

Py:   s1 == s2; s1 != s2
来源：http://xj.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cr.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lg.colortex.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xj.huixiangedu.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tx.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gw.jianghongdianzi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ew.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pl.chemitech.net.cn

[A26] 类型转换总览
来源：http://qi.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ku.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zr.asd995.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://re.haigaiapp.cn

TS:   Number() String() Boolean() x as number
来源：http://te.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hr.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://et.nszjky.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qa.hnjuh.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wq.gzmigu.cn

================================================================================
来源：http://he.bookmarksfly.cn

B. 流程控制
来源：http://ze.shxzukj.cn

================================================================================
来源：http://gq.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://ce.yuexingan06.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yy.bjjhwx.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fh.colortex.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ha.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wr.shxzukj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://hv.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bm.chemitech.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://og.hahajie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ht.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://ux.shtwfgs.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qh.gzmigu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://le.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pq.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gp.hahajie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jj.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://le.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lp.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ra.wgjwhj.cn

[B03] switch / match / case
来源：http://ck.yuexingan06.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ma.hahajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://um.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qb.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yy.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://be.lnxyls.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ai.hahajie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xe.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gg.wgjwhj.cn

[B04] for 计数循环
来源：http://ii.huixiangedu.cn

Py:   for i in range(10): print(i)
来源：http://lu.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nf.huixinmuqiang.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://on.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sr.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kh.haigaiapp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://im.panjiajie.cn

Ruby: 10.times { |i| puts i }
来源：http://hm.9csxet.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ym.szxytkj.cn

[B05] 遍历数组 / 列表
来源：http://yy.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://sd.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zz.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sr.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bu.shxzukj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ht.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pb.newstarts.cn

Ruby: arr.each { |item| puts item }
来源：http://ok.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ze.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://mp.asd995.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qb.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kw.shxzukj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ru.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://im.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aa.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xv.jctech888.com.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oo.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ll.nicolike.cn

[B07] while 循环
来源：http://gz.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://fn.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://px.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://uv.jctech888.com.cn

TS:   while (i < 10) { i++; }
来源：http://zg.newstarts.cn

Java: while (i < 10) { i++; }
来源：http://ka.muxihuayi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://di.gzmigu.cn

Ruby: while i < 10; i += 1; end
来源：http://cd.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://qx.asd995.cn

[B08] do-while（至少执行一次）
来源：http://hv.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://sy.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xj.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://ma.lnxyls.cn

TS:   do { i++; } while (i < 10);
来源：http://ng.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://im.jctech888.com.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fw.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ah.gzmigu.cn

C#:   do { i++; } while (i < 10);
来源：http://rb.shtwfgs.cn

[B09] break 与 continue
来源：http://ba.lnxyls.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yn.nszjky.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gr.huanxung.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iy.nicolike.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://id.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ot.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bc.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sa.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uf.panjiajie.cn

[B10] 遍历同时拿索引
来源：http://ix.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hh.asd995.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xr.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mf.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://do.chemitech.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gm.haigaiapp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xq.szsharing.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wj.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tn.jctech888.com.cn

[B11] 生成数字序列 / 区间
来源：http://wk.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://gy.hnjuh.cn

PHP:  range(0, 10, 2);
来源：http://by.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ib.shxzskj.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bi.shxzukj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cf.huixiangedu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ca.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://jz.chemitech.net.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jm.nicolike.cn

[B12] 跳出多层循环
来源：http://qd.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://aj.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jt.jianghongdianzi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pk.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ia.gzmigu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ht.jianghongdianzi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ce.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qe.asd995.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://et.asd995.cn

[B13] 判断是否为数字
来源：http://na.yuexingan06.cn

Py:   isinstance(x, (int, float))
来源：http://cs.hahajie.cn

PHP:  is_numeric($x)
来源：http://th.nszjky.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wk.yuntaijiaju.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rw.521024.cn

Java: x instanceof Number
来源：http://zt.jctech888.com.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fz.wgjwhj.cn

Ruby: x.is_a?(Numeric)
来源：http://ru.lnxyls.cn

C#:   x is int or double or decimal
来源：http://lv.521024.cn

[B14] 判断值是否在集合内
来源：http://bk.hnjuh.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ax.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vs.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://ex.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://zw.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lt.yuexingan06.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zw.9csxet.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sq.jianghongdianzi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fd.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://zy.bookmarksfly.cn

Py:   a and b or not c
来源：http://sm.szsharing.cn

PHP:  $a && $b || !$c
来源：http://yz.bookmarksfly.cn

JS:   a && b || !c
来源：http://vq.huixiangedu.cn

TS:   a && b || !c
来源：http://cc.colortex.cn

Java: a && b || !c
来源：http://uu.asd995.cn

Go:   a && b || !c
来源：http://vu.lnxyls.cn

Ruby: a && b || !c
来源：http://mi.colortex.cn

C#:   a && b || !c
来源：http://ll.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://py.bjjhwx.cn

Py:   if not data: return
来源：http://dn.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://em.nszjky.cn

JS:   if (!data) return;
来源：http://xr.chemitech.net.cn

TS:   if (!data) return;
来源：http://sw.huanxung.cn

Java: if (data == null) return;
来源：http://km.huixiangedu.cn

Go:   if data == nil { return }
来源：http://nw.szsharing.cn

Ruby: return if data.nil?
来源：http://fg.huixinmuqiang.cn

C#:   if (data == null) return;
来源：http://zw.hahajie.cn

================================================================================
来源：http://hb.chemitech.net.cn

C. 函数与作用域
来源：http://eq.asd995.cn

================================================================================
来源：http://il.wgjwhj.cn

[C01] 定义函数
来源：http://ff.lnxyls.cn

Py:   def add(a, b): return a + b
来源：http://cs.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://im.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://ng.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pz.wgjwhj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ju.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bo.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://hz.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nf.hahajie.cn

[C02] 默认参数
来源：http://ys.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://pd.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uj.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://qq.hahajie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lw.nszjky.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ua.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://be.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://uo.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://zu.muxihuayi.cn

[C03] 可变参数
来源：http://gc.yuntaijiaju.cn

Py:   def total(*args): return sum(args)
来源：http://fy.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ke.colortex.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xf.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fn.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xu.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pk.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pp.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://er.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://kq.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hh.bjjhwx.cn


<!-- 参考信息 -->