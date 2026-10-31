代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://lk.yuntaijiaju.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tv.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://gc.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tu.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://eb.huanxung.cn

JS:   `Hello, ${name}!`
来源：http://qd.haigaiapp.cn

TS:   `Hello, ${name}!`
来源：http://lu.bjjhwx.cn

Java: "Hello, %s!".formatted(name)
来源：http://zf.bookmarksfly.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yb.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://gu.hahajie.cn

C#:   $"Hello, {name}!"
来源：http://us.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lj.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://ii.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://ti.shtwfgs.cn

JS:   "第一行\n第二行"
来源：http://mc.newstarts.cn

TS:   "第一行\n第二行"
来源：http://am.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://wl.panjiajie.cn

Go:   "第一行\n第二行"
来源：http://iu.gzmigu.cn

Ruby: "第一行\n第二行"
来源：http://fi.newstarts.cn

C#:   "第一行\n第二行"
来源：http://qs.shxzskj.cn

[A14] 注释写法
来源：http://zi.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vo.huixiangedu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://br.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://pn.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://gh.nszjky.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rz.panjiajie.cn

Go:   // 单行；/* 多行 */
来源：http://hn.szxytkj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ha.yuexingan06.cn

C#:   // 单行；/* 多行 */
来源：http://yv.szsharing.cn

[A15] 空值判断与默认值
来源：http://ax.asd995.cn

Py:   value = data or "默认值"
来源：http://fh.jctech888.com.cn

PHP:  $value = $data ?? "默认值";
来源：http://wk.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://cy.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://tw.panjiajie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ra.nszjky.cn

Go:   if data == "" { data = "默认值" }
来源：http://rf.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://ks.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://wo.shxzukj.cn

[A16] 真假值判断规则
来源：http://la.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lg.bookmarksfly.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oq.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sy.szsharing.cn

TS:   if (!x) {}
来源：http://ug.shxzskj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oc.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hm.jianghongdianzi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bw.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yk.lnxyls.cn

[A17] 位运算
来源：http://ah.nszjky.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bf.nicolike.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ti.szsharing.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hr.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hv.jianghongdianzi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sl.yuexingan06.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nm.jianghongdianzi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hi.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ro.shxzskj.cn

[A18] 字符与 ASCII 码互转
来源：http://kh.szxytkj.cn

Py:   ord("A"); chr(65)
来源：http://yw.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://tq.asd995.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://se.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ma.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://km.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://in.szxytkj.cn

Ruby: "A".ord; 65.chr
来源：http://pc.chemitech.net.cn

C#:   (int)'A'; (char)65
来源：http://nn.huanxung.cn

[A19] 交换两个变量
来源：http://ea.nszjky.cn

Py:   a, b = b, a
来源：http://kr.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qx.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://aa.asd995.cn

TS:   [a, b] = [b, a];
来源：http://xm.shxzskj.cn

Java: int t = a; a = b; b = t;
来源：http://qn.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://vr.521024.cn

Ruby: a, b = b, a
来源：http://sb.panjiajie.cn

C#:   (a, b) = (b, a);
来源：http://ry.shxzskj.cn

[A20] 读取标准输入
来源：http://ok.jctech888.com.cn

Py:   name = input("请输入：")
来源：http://cl.hnjuh.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bl.haigaiapp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fu.huixinmuqiang.cn

TS:   // Node.js：readline 模块
来源：http://uc.szxytkj.cn

Java: new Scanner(System.in).nextLine()
来源：http://gw.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dj.asd995.cn

Ruby: gets.chomp
来源：http://rs.lnxyls.cn

C#:   Console.ReadLine();
来源：http://no.szxytkj.cn

[A21] 保留指定小数位输出
来源：http://vf.newstarts.cn

Py:   f"{3.14159:.2f}"
来源：http://tv.jctech888.com.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wy.szsharing.cn

JS:   (3.14159).toFixed(2)
来源：http://mi.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://xl.yuntaijiaju.cn

Java: String.format("%.2f", 3.14159)
来源：http://hx.yuexingan06.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hw.bjjhwx.cn

Ruby: format("%.2f", 3.14159)
来源：http://uw.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://ns.bookmarksfly.cn

[A22] 获取字符串长度
来源：http://yj.yuntaijiaju.cn

Py:   len(s)
来源：http://us.szxytkj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eh.chemitech.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bp.bookmarksfly.cn

TS:   s.length
来源：http://jw.shtwfgs.cn

Java: s.length()
来源：http://ia.szsharing.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bp.huixiangedu.cn

Ruby: s.length
来源：http://qn.shxzskj.cn

C#:   s.Length
来源：http://ov.shtwfgs.cn

[A23] 大小写转换
来源：http://lp.521024.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ab.colortex.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uh.521024.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pm.shtwfgs.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tn.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zf.jctech888.com.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xt.nicolike.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yx.shtwfgs.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jz.yuexingan06.cn

[A24] 去除首尾空白
来源：http://xl.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jk.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qa.bjjhwx.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mj.nszjky.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lm.wgjwhj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rv.hnjuh.cn

Go:   strings.TrimSpace(s)
来源：http://ph.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ab.9csxet.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gh.huanxung.cn

[A25] 字符串比较
来源：http://td.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://qx.shxzskj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://je.szxytkj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xz.huanxung.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ie.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bf.521024.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mu.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nn.huixiangedu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nw.asd995.cn

[A26] 类型转换总览
来源：http://xr.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ns.nszjky.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oe.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ef.newstarts.cn

TS:   Number() String() Boolean() x as number
来源：http://hd.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pp.gzmigu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qq.lnxyls.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hg.gzmigu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://je.huanxung.cn

================================================================================
来源：http://zl.hnjuh.cn

B. 流程控制
来源：http://dd.hnjuh.cn

================================================================================
来源：http://sf.yuntaijiaju.cn

[B01] 条件判断 if / else
来源：http://lq.colortex.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pa.lnxyls.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cv.jctech888.com.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pd.bookmarksfly.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sn.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gt.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://us.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sh.521024.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aa.jctech888.com.cn

[B02] 多分支 else if / elif
来源：http://fh.panjiajie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ij.huixinmuqiang.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hv.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rp.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uv.bjjhwx.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sw.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ib.huixinmuqiang.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rc.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rc.lnxyls.cn

[B03] switch / match / case
来源：http://yz.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rq.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://be.szsharing.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zg.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lg.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qv.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ar.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sy.hnjuh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mf.shxzukj.cn

[B04] for 计数循环
来源：http://mi.newstarts.cn

Py:   for i in range(10): print(i)
来源：http://re.jctech888.com.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ii.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ys.huixiangedu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://be.lnxyls.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cb.bjjhwx.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tn.szsharing.cn

Ruby: 10.times { |i| puts i }
来源：http://nq.521024.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gd.asd995.cn

[B05] 遍历数组 / 列表
来源：http://tu.newstarts.cn

Py:   for item in arr: print(item)
来源：http://pj.muxihuayi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yk.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lv.haigaiapp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mv.panjiajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ae.wgjwhj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ph.panjiajie.cn

Ruby: arr.each { |item| puts item }
来源：http://jo.gzmigu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rg.bookmarksfly.cn

[B06] 遍历字典 / 对象
来源：http://ci.panjiajie.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mm.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hj.9csxet.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pe.yuexingan06.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vh.gzmigu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dz.shtwfgs.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uy.wgjwhj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fd.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bl.bookmarksfly.cn

[B07] while 循环
来源：http://uf.lnxyls.cn

Py:   while i < 10: i += 1
来源：http://aq.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pd.jianghongdianzi.cn

JS:   while (i < 10) { i++; }
来源：http://yr.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://lb.colortex.cn

Java: while (i < 10) { i++; }
来源：http://ir.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iq.9csxet.cn

Ruby: while i < 10; i += 1; end
来源：http://ff.bjjhwx.cn

C#:   while (i < 10) { i++; }
来源：http://ep.wgjwhj.cn

[B08] do-while（至少执行一次）
来源：http://ca.jctech888.com.cn

Py:   # 无 do-while：用 while True + break
来源：http://af.bookmarksfly.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fm.newstarts.cn

JS:   do { i++; } while (i < 10);
来源：http://tp.521024.cn

TS:   do { i++; } while (i < 10);
来源：http://te.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://lt.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oi.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ml.panjiajie.cn

C#:   do { i++; } while (i < 10);
来源：http://xc.9csxet.cn

[B09] break 与 continue
来源：http://lh.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mq.asd995.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eu.521024.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sp.huixinmuqiang.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gm.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xe.haigaiapp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yi.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qx.haigaiapp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://su.newstarts.cn

[B10] 遍历同时拿索引
来源：http://lh.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wh.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bt.shtwfgs.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ng.panjiajie.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jc.haigaiapp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://am.lnxyls.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yd.wgjwhj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xd.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fx.newstarts.cn

[B11] 生成数字序列 / 区间
来源：http://bl.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://iy.shxzskj.cn

PHP:  range(0, 10, 2);
来源：http://vn.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fk.chemitech.net.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vi.huixiangedu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bj.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jz.newstarts.cn

Ruby: (0...10).step(2).to_a
来源：http://ij.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zq.hnjuh.cn

[B12] 跳出多层循环
来源：http://wv.gzmigu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zr.panjiajie.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://on.bookmarksfly.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wc.yuexingan06.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://di.yuexingan06.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://th.shxzskj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vn.lnxyls.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rg.bjjhwx.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pm.shxzukj.cn

[B13] 判断是否为数字
来源：http://hh.lnxyls.cn

Py:   isinstance(x, (int, float))
来源：http://so.hahajie.cn

PHP:  is_numeric($x)
来源：http://nu.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ko.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wa.huanxung.cn

Java: x instanceof Number
来源：http://oy.521024.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mg.newstarts.cn

Ruby: x.is_a?(Numeric)
来源：http://dl.yuexingan06.cn

C#:   x is int or double or decimal
来源：http://yh.yuexingan06.cn

[B14] 判断值是否在集合内
来源：http://te.huanxung.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hq.jctech888.com.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://el.yuexingan06.cn

JS:   [1, 2, 3].includes(x)
来源：http://rt.shtwfgs.cn

TS:   [1, 2, 3].includes(x)
来源：http://gn.panjiajie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jx.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bi.jianghongdianzi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ht.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ve.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://yh.haigaiapp.cn

Py:   a and b or not c
来源：http://bn.yuntaijiaju.cn

PHP:  $a && $b || !$c
来源：http://yb.bjjhwx.cn

JS:   a && b || !c
来源：http://rx.gzmigu.cn

TS:   a && b || !c
来源：http://xr.shtwfgs.cn

Java: a && b || !c
来源：http://js.hahajie.cn

Go:   a && b || !c
来源：http://yr.yuexingan06.cn

Ruby: a && b || !c
来源：http://vl.shtwfgs.cn

C#:   a && b || !c
来源：http://jj.szsharing.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zu.shtwfgs.cn

Py:   if not data: return
来源：http://ts.gzmigu.cn

PHP:  if (!$data) { return; }
来源：http://bg.hahajie.cn

JS:   if (!data) return;
来源：http://ak.shxzukj.cn

TS:   if (!data) return;
来源：http://sc.shxzskj.cn

Java: if (data == null) return;
来源：http://fr.colortex.cn

Go:   if data == nil { return }
来源：http://fj.szsharing.cn

Ruby: return if data.nil?
来源：http://ff.shtwfgs.cn

C#:   if (data == null) return;
来源：http://hn.bookmarksfly.cn

================================================================================
来源：http://hm.shxzukj.cn

C. 函数与作用域
来源：http://pa.bjjhwx.cn

================================================================================
来源：http://op.panjiajie.cn

[C01] 定义函数
来源：http://fv.bjjhwx.cn

Py:   def add(a, b): return a + b
来源：http://vr.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hb.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://fk.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sl.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://aq.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gb.hnjuh.cn

Ruby: def add(a, b); a + b; end
来源：http://eg.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qw.jctech888.com.cn

[C02] 默认参数
来源：http://vr.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://do.lnxyls.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://sx.szxytkj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ws.yuexingan06.cn


<!-- 参考信息 -->