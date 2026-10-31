代发 wailian999

Java: "第一行\n第二行"
来源：http://pl.nszjky.cn

Go:   "第一行\n第二行"
来源：http://vt.asd995.cn

Ruby: "第一行\n第二行"
来源：http://ub.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://gx.wgjwhj.cn

[A14] 注释写法
来源：http://vp.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gq.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dv.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://wb.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://kd.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gq.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://rj.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://av.newstarts.cn

C#:   // 单行；/* 多行 */
来源：http://eo.shxzskj.cn

[A15] 空值判断与默认值
来源：http://zt.asd995.cn

Py:   value = data or "默认值"
来源：http://sg.shxzukj.cn

PHP:  $value = $data ?? "默认值";
来源：http://ue.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://yv.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://cv.shtwfgs.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gq.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://rl.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://bn.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://ko.newstarts.cn

[A16] 真假值判断规则
来源：http://xb.wgjwhj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ph.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oi.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zx.9csxet.cn

TS:   if (!x) {}
来源：http://es.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mr.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xb.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ek.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://or.szxytkj.cn

[A17] 位运算
来源：http://pv.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://el.gzmigu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pc.huixinmuqiang.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ez.wgjwhj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jz.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sw.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://oj.huanxung.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zp.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://up.colortex.cn

[A18] 字符与 ASCII 码互转
来源：http://my.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://lc.yuntaijiaju.cn

PHP:  ord("A"); chr(65)
来源：http://ne.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gu.szsharing.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gm.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://mk.shxzskj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://aa.521024.cn

Ruby: "A".ord; 65.chr
来源：http://el.jctech888.com.cn

C#:   (int)'A'; (char)65
来源：http://ik.yuntaijiaju.cn

[A19] 交换两个变量
来源：http://od.huixiangedu.cn

Py:   a, b = b, a
来源：http://ww.muxihuayi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ss.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://gf.huixinmuqiang.cn

TS:   [a, b] = [b, a];
来源：http://bn.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://dt.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://ww.gzmigu.cn

Ruby: a, b = b, a
来源：http://pa.bookmarksfly.cn

C#:   (a, b) = (b, a);
来源：http://tc.gzmigu.cn

[A20] 读取标准输入
来源：http://km.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://ru.szsharing.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mb.shtwfgs.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xl.bookmarksfly.cn

TS:   // Node.js：readline 模块
来源：http://hm.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://uj.muxihuayi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://iq.huixiangedu.cn

Ruby: gets.chomp
来源：http://pg.shxzskj.cn

C#:   Console.ReadLine();
来源：http://pn.asd995.cn

[A21] 保留指定小数位输出
来源：http://ua.nicolike.cn

Py:   f"{3.14159:.2f}"
来源：http://fe.yuexingan06.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cf.shxzskj.cn

JS:   (3.14159).toFixed(2)
来源：http://sv.521024.cn

TS:   (3.14159).toFixed(2)
来源：http://yy.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://vc.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zn.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://eg.colortex.cn

C#:   3.14159.ToString("F2")
来源：http://zz.asd995.cn

[A22] 获取字符串长度
来源：http://xc.newstarts.cn

Py:   len(s)
来源：http://zp.hahajie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://un.hnjuh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://op.lnxyls.cn

TS:   s.length
来源：http://vx.newstarts.cn

Java: s.length()
来源：http://fg.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fo.wgjwhj.cn

Ruby: s.length
来源：http://jo.newstarts.cn

C#:   s.Length
来源：http://am.huanxung.cn

[A23] 大小写转换
来源：http://ft.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lg.hahajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://di.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cy.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sa.jctech888.com.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://da.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tr.jctech888.com.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nj.wgjwhj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yr.gzmigu.cn

[A24] 去除首尾空白
来源：http://tb.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yp.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oj.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hi.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://si.chemitech.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cx.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://kt.chemitech.net.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wa.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fx.muxihuayi.cn

[A25] 字符串比较
来源：http://ah.huixinmuqiang.cn

Py:   s1 == s2; s1 != s2
来源：http://db.yuexingan06.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ur.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lb.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ze.yuntaijiaju.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qk.huanxung.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bm.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ci.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ub.lnxyls.cn

[A26] 类型转换总览
来源：http://eu.shxzskj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nq.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fa.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oi.hnjuh.cn

TS:   Number() String() Boolean() x as number
来源：http://ez.huanxung.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hw.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fq.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lr.521024.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://be.jctech888.com.cn

================================================================================
来源：http://wp.bookmarksfly.cn

B. 流程控制
来源：http://tb.szxytkj.cn

================================================================================
来源：http://hn.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://mr.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hf.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tc.shxzskj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zi.521024.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://un.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gy.521024.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rr.lnxyls.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lc.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ou.newstarts.cn

[B02] 多分支 else if / elif
来源：http://ao.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hf.huixiangedu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ru.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zx.shxzukj.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ln.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fe.szxytkj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ws.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mw.hahajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://df.chemitech.net.cn

[B03] switch / match / case
来源：http://wz.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wm.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rt.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oa.szxytkj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tq.haigaiapp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mr.jianghongdianzi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yy.shxzskj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hn.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zn.shxzskj.cn

[B04] for 计数循环
来源：http://kg.bookmarksfly.cn

Py:   for i in range(10): print(i)
来源：http://tn.bookmarksfly.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://od.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jm.szsharing.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ph.hnjuh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fa.jianghongdianzi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sl.chemitech.net.cn

Ruby: 10.times { |i| puts i }
来源：http://kg.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ut.bookmarksfly.cn

[B05] 遍历数组 / 列表
来源：http://er.szsharing.cn

Py:   for item in arr: print(item)
来源：http://nt.jianghongdianzi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gk.bjjhwx.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://id.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lm.jianghongdianzi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nn.shtwfgs.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iu.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://th.yuexingan06.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ub.muxihuayi.cn

[B06] 遍历字典 / 对象
来源：http://ib.shxzskj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vq.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://db.wgjwhj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://px.shxzukj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ed.szsharing.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gx.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://at.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cm.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ty.szxytkj.cn

[B07] while 循环
来源：http://wr.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://dd.lnxyls.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bl.chemitech.net.cn

JS:   while (i < 10) { i++; }
来源：http://yf.newstarts.cn

TS:   while (i < 10) { i++; }
来源：http://ne.huanxung.cn

Java: while (i < 10) { i++; }
来源：http://fk.shxzukj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nv.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://fz.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://cc.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://tg.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://ka.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bw.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://lo.huixiangedu.cn

TS:   do { i++; } while (i < 10);
来源：http://hs.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://od.huixiangedu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://id.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ra.shtwfgs.cn

C#:   do { i++; } while (i < 10);
来源：http://yt.jctech888.com.cn

[B09] break 与 continue
来源：http://wd.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tk.colortex.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zt.nicolike.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://og.lnxyls.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://im.asd995.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pv.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ny.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ej.shxzukj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ak.huixinmuqiang.cn

[B10] 遍历同时拿索引
来源：http://wx.bookmarksfly.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ne.shxzskj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kp.hahajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yr.shtwfgs.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ij.szxytkj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ax.panjiajie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://md.gzmigu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vw.colortex.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sm.szxytkj.cn

[B11] 生成数字序列 / 区间
来源：http://ck.huixiangedu.cn

Py:   list(range(0, 10, 2))
来源：http://qt.jianghongdianzi.cn

PHP:  range(0, 10, 2);
来源：http://ve.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://np.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cj.huixinmuqiang.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cs.newstarts.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yt.szsharing.cn

Ruby: (0...10).step(2).to_a
来源：http://fc.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wx.colortex.cn

[B12] 跳出多层循环
来源：http://mm.panjiajie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dm.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://iv.nszjky.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ww.bookmarksfly.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://na.bjjhwx.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ik.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hu.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rf.gzmigu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yt.hnjuh.cn

[B13] 判断是否为数字
来源：http://lv.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://gw.nicolike.cn

PHP:  is_numeric($x)
来源：http://ch.newstarts.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iw.gzmigu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://er.newstarts.cn

Java: x instanceof Number
来源：http://ny.colortex.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yl.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://vc.hnjuh.cn

C#:   x is int or double or decimal
来源：http://mu.hnjuh.cn

[B14] 判断值是否在集合内
来源：http://lx.bjjhwx.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://we.panjiajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eu.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://dw.yuntaijiaju.cn

TS:   [1, 2, 3].includes(x)
来源：http://us.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qq.huixinmuqiang.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ls.asd995.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pg.9csxet.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ey.nszjky.cn

[B15] 布尔运算与取反
来源：http://ey.jianghongdianzi.cn

Py:   a and b or not c
来源：http://hm.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://mv.colortex.cn

JS:   a && b || !c
来源：http://wy.bookmarksfly.cn

TS:   a && b || !c
来源：http://fa.9csxet.cn

Java: a && b || !c
来源：http://na.hahajie.cn

Go:   a && b || !c
来源：http://xm.wgjwhj.cn

Ruby: a && b || !c
来源：http://mj.szxytkj.cn

C#:   a && b || !c
来源：http://mq.newstarts.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ls.jianghongdianzi.cn

Py:   if not data: return
来源：http://wp.szxytkj.cn

PHP:  if (!$data) { return; }
来源：http://fz.521024.cn

JS:   if (!data) return;
来源：http://sb.asd995.cn

TS:   if (!data) return;
来源：http://ry.hnjuh.cn

Java: if (data == null) return;
来源：http://jp.shxzukj.cn

Go:   if data == nil { return }
来源：http://sk.newstarts.cn

Ruby: return if data.nil?
来源：http://vq.newstarts.cn

C#:   if (data == null) return;
来源：http://qz.jianghongdianzi.cn

================================================================================
来源：http://vh.9csxet.cn

C. 函数与作用域
来源：http://fd.huixinmuqiang.cn

================================================================================
来源：http://jt.jctech888.com.cn

[C01] 定义函数
来源：http://tb.9csxet.cn

Py:   def add(a, b): return a + b
来源：http://ex.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lg.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://vw.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yq.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hs.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vi.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://nv.yuexingan06.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lx.nicolike.cn

[C02] 默认参数
来源：http://mi.muxihuayi.cn

Py:   def greet(name="World"): return name
来源：http://jj.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jl.bookmarksfly.cn

JS:   function greet(name = "World") { return name; }
来源：http://tg.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oh.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ub.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dz.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://mo.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://hk.yuntaijiaju.cn

[C03] 可变参数
来源：http://tv.521024.cn

Py:   def total(*args): return sum(args)
来源：http://sv.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oj.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vo.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lr.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qm.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://en.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jm.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qv.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://zy.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cc.huanxung.cn


<!-- 参考信息 -->