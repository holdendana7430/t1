代发 wailian999

[A14] 注释写法
来源：http://gw.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qp.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yl.muxihuayi.cn

JS:   // 单行；/* 多行 */
来源：http://um.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://or.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ld.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://fn.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://za.lnxyls.cn

C#:   // 单行；/* 多行 */
来源：http://xf.huixiangedu.cn

[A15] 空值判断与默认值
来源：http://qk.yuntaijiaju.cn

Py:   value = data or "默认值"
来源：http://um.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://nz.szsharing.cn

JS:   const value = data ?? "默认值";
来源：http://je.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://cf.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zf.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://zi.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://ba.szxytkj.cn

C#:   var value = data ?? "默认值";
来源：http://db.shxzukj.cn

[A16] 真假值判断规则
来源：http://pd.bookmarksfly.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ul.haigaiapp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fa.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sk.yuntaijiaju.cn

TS:   if (!x) {}
来源：http://ye.gzmigu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tl.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uo.wgjwhj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jn.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cf.huixiangedu.cn

[A17] 位运算
来源：http://qg.huixinmuqiang.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://br.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qr.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ou.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xn.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ol.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tr.shxzukj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://in.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pz.bjjhwx.cn

[A18] 字符与 ASCII 码互转
来源：http://wx.yuntaijiaju.cn

Py:   ord("A"); chr(65)
来源：http://mc.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://hh.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iz.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://da.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://aw.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hx.hnjuh.cn

Ruby: "A".ord; 65.chr
来源：http://sv.bookmarksfly.cn

C#:   (int)'A'; (char)65
来源：http://to.jctech888.com.cn

[A19] 交换两个变量
来源：http://ch.chemitech.net.cn

Py:   a, b = b, a
来源：http://eq.jctech888.com.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vg.colortex.cn

JS:   [a, b] = [b, a];
来源：http://zo.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://vk.szsharing.cn

Java: int t = a; a = b; b = t;
来源：http://uq.gzmigu.cn

Go:   a, b = b, a
来源：http://yx.bjjhwx.cn

Ruby: a, b = b, a
来源：http://yt.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://ce.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://ah.hnjuh.cn

Py:   name = input("请输入：")
来源：http://ak.panjiajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dc.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sm.jianghongdianzi.cn

TS:   // Node.js：readline 模块
来源：http://dr.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://mv.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mg.asd995.cn

Ruby: gets.chomp
来源：http://by.shtwfgs.cn

C#:   Console.ReadLine();
来源：http://jn.hnjuh.cn

[A21] 保留指定小数位输出
来源：http://ma.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://ls.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iy.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://xv.shtwfgs.cn

TS:   (3.14159).toFixed(2)
来源：http://jd.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://va.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ev.chemitech.net.cn

Ruby: format("%.2f", 3.14159)
来源：http://gp.chemitech.net.cn

C#:   3.14159.ToString("F2")
来源：http://zk.szxytkj.cn

[A22] 获取字符串长度
来源：http://bh.lnxyls.cn

Py:   len(s)
来源：http://ju.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ci.wgjwhj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ak.huixiangedu.cn

TS:   s.length
来源：http://qh.nszjky.cn

Java: s.length()
来源：http://wj.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zu.bjjhwx.cn

Ruby: s.length
来源：http://dc.bookmarksfly.cn

C#:   s.Length
来源：http://sg.hahajie.cn

[A23] 大小写转换
来源：http://cl.yuexingan06.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ir.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ir.hahajie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wz.muxihuayi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fz.shtwfgs.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fb.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nn.nszjky.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tx.newstarts.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zk.shxzskj.cn

[A24] 去除首尾空白
来源：http://yi.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mk.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ot.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kw.bookmarksfly.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://me.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gn.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://vc.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rk.shxzukj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yc.newstarts.cn

[A25] 字符串比较
来源：http://bt.asd995.cn

Py:   s1 == s2; s1 != s2
来源：http://ku.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sz.hnjuh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vv.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fa.nicolike.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bo.nszjky.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sz.jctech888.com.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xv.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pg.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://hr.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://yd.panjiajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://za.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://db.huixiangedu.cn

TS:   Number() String() Boolean() x as number
来源：http://gf.hahajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kz.yuexingan06.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ua.haigaiapp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jm.newstarts.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dl.panjiajie.cn

================================================================================
来源：http://na.szxytkj.cn

B. 流程控制
来源：http://lf.huixiangedu.cn

================================================================================
来源：http://oz.colortex.cn

[B01] 条件判断 if / else
来源：http://di.9csxet.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ep.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pj.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ws.wgjwhj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ec.nszjky.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vi.asd995.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hh.9csxet.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pr.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nu.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://lq.chemitech.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://et.wgjwhj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fn.jctech888.com.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pe.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rv.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://td.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dh.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ws.yuexingan06.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ka.yuexingan06.cn

[B03] switch / match / case
来源：http://tl.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gw.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sz.521024.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rf.gzmigu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cu.lnxyls.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fv.asd995.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ct.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wf.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gc.asd995.cn

[B04] for 计数循环
来源：http://fe.haigaiapp.cn

Py:   for i in range(10): print(i)
来源：http://mf.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nx.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ji.jctech888.com.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qo.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pn.wgjwhj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rh.jianghongdianzi.cn

Ruby: 10.times { |i| puts i }
来源：http://cj.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ix.gzmigu.cn

[B05] 遍历数组 / 列表
来源：http://vi.szxytkj.cn

Py:   for item in arr: print(item)
来源：http://ko.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ga.gzmigu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pp.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://zx.szxytkj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ra.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bl.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://of.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://il.yuexingan06.cn

[B06] 遍历字典 / 对象
来源：http://fo.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dn.nicolike.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xk.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nq.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://en.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sn.szxytkj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yt.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fu.yuexingan06.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mm.jctech888.com.cn

[B07] while 循环
来源：http://va.panjiajie.cn

Py:   while i < 10: i += 1
来源：http://gn.muxihuayi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zy.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://hw.muxihuayi.cn

TS:   while (i < 10) { i++; }
来源：http://ea.szxytkj.cn

Java: while (i < 10) { i++; }
来源：http://mu.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bq.asd995.cn

Ruby: while i < 10; i += 1; end
来源：http://ua.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://vi.haigaiapp.cn

[B08] do-while（至少执行一次）
来源：http://ao.colortex.cn

Py:   # 无 do-while：用 while True + break
来源：http://lg.muxihuayi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ba.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://hj.yuexingan06.cn

TS:   do { i++; } while (i < 10);
来源：http://nx.bookmarksfly.cn

Java: do { i++; } while (i < 10);
来源：http://sz.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://jb.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kw.haigaiapp.cn

C#:   do { i++; } while (i < 10);
来源：http://cp.muxihuayi.cn

[B09] break 与 continue
来源：http://fo.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qh.huanxung.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dn.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://az.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dh.haigaiapp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://id.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gg.jctech888.com.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dt.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mu.gzmigu.cn

[B10] 遍历同时拿索引
来源：http://xl.shxzukj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jx.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oe.newstarts.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ku.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sm.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cr.yuntaijiaju.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lf.yuexingan06.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aw.bookmarksfly.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zq.hnjuh.cn

[B11] 生成数字序列 / 区间
来源：http://fi.yuntaijiaju.cn

Py:   list(range(0, 10, 2))
来源：http://za.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://rp.lnxyls.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dk.nszjky.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uk.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hq.wgjwhj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tr.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://px.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fy.gzmigu.cn

[B12] 跳出多层循环
来源：http://dz.hnjuh.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cr.bjjhwx.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gt.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hp.hnjuh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pr.lnxyls.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ej.szsharing.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pc.szxytkj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vm.shxzskj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aw.bookmarksfly.cn

[B13] 判断是否为数字
来源：http://cm.panjiajie.cn

Py:   isinstance(x, (int, float))
来源：http://ao.muxihuayi.cn

PHP:  is_numeric($x)
来源：http://pd.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mz.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kb.521024.cn

Java: x instanceof Number
来源：http://vt.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ci.muxihuayi.cn

Ruby: x.is_a?(Numeric)
来源：http://ib.9csxet.cn

C#:   x is int or double or decimal
来源：http://mq.hahajie.cn

[B14] 判断值是否在集合内
来源：http://fx.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jk.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://te.muxihuayi.cn

JS:   [1, 2, 3].includes(x)
来源：http://dx.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://nr.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wr.szsharing.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ef.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kj.yuexingan06.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ev.huixiangedu.cn

[B15] 布尔运算与取反
来源：http://wz.gzmigu.cn

Py:   a and b or not c
来源：http://gy.colortex.cn

PHP:  $a && $b || !$c
来源：http://hz.panjiajie.cn

JS:   a && b || !c
来源：http://fu.haigaiapp.cn

TS:   a && b || !c
来源：http://eq.colortex.cn

Java: a && b || !c
来源：http://yt.bookmarksfly.cn

Go:   a && b || !c
来源：http://iq.huanxung.cn

Ruby: a && b || !c
来源：http://ol.shxzukj.cn

C#:   a && b || !c
来源：http://el.jctech888.com.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cy.yuntaijiaju.cn

Py:   if not data: return
来源：http://oc.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://gv.colortex.cn

JS:   if (!data) return;
来源：http://xj.shxzukj.cn

TS:   if (!data) return;
来源：http://zz.huanxung.cn

Java: if (data == null) return;
来源：http://sv.muxihuayi.cn

Go:   if data == nil { return }
来源：http://uk.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://cq.nicolike.cn

C#:   if (data == null) return;
来源：http://jy.hahajie.cn

================================================================================
来源：http://ls.shxzskj.cn

C. 函数与作用域
来源：http://ds.nszjky.cn

================================================================================
来源：http://sv.521024.cn

[C01] 定义函数
来源：http://rs.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://yc.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://do.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://lk.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pu.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://qc.lnxyls.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gg.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://kg.newstarts.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bk.asd995.cn

[C02] 默认参数
来源：http://oe.521024.cn

Py:   def greet(name="World"): return name
来源：http://pi.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xc.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://yr.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xb.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wh.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ka.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://dk.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://me.hnjuh.cn

[C03] 可变参数
来源：http://fu.panjiajie.cn

Py:   def total(*args): return sum(args)
来源：http://ui.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cv.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hy.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yt.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ba.shxzskj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tm.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gl.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wd.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://tk.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dw.jianghongdianzi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ub.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hv.wgjwhj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gn.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://id.gzmigu.cn


<!-- 参考信息 -->