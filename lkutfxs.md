代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://rq.huanxung.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uh.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://kw.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yz.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fp.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kc.haigaiapp.cn

[A12] 字符串插值 / 格式化
来源：http://nr.jctech888.com.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jw.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kt.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://ay.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://ef.nicolike.cn

Java: "Hello, %s!".formatted(name)
来源：http://nw.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://le.lnxyls.cn

Ruby: "Hello, #{name}!"
来源：http://hn.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://wq.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hu.hahajie.cn

Py:   "第一行\n第二行"
来源：http://nn.huixinmuqiang.cn

PHP:  "第一行\n第二行"
来源：http://zr.9csxet.cn

JS:   "第一行\n第二行"
来源：http://ow.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://js.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://dy.huanxung.cn

Go:   "第一行\n第二行"
来源：http://nu.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://rh.shtwfgs.cn

C#:   "第一行\n第二行"
来源：http://fl.shtwfgs.cn

[A14] 注释写法
来源：http://ea.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ef.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gm.nicolike.cn

JS:   // 单行；/* 多行 */
来源：http://se.huixinmuqiang.cn

TS:   // 单行；/* 多行 */
来源：http://nu.bookmarksfly.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cg.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://lm.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pb.panjiajie.cn

C#:   // 单行；/* 多行 */
来源：http://fd.gzmigu.cn

[A15] 空值判断与默认值
来源：http://yv.9csxet.cn

Py:   value = data or "默认值"
来源：http://pd.hahajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://ap.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://gj.szxytkj.cn

TS:   const value = data ?? "默认值";
来源：http://qx.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://to.lnxyls.cn

Go:   if data == "" { data = "默认值" }
来源：http://vj.yuntaijiaju.cn

Ruby: value = data || "默认值"
来源：http://em.nszjky.cn

C#:   var value = data ?? "默认值";
来源：http://su.panjiajie.cn

[A16] 真假值判断规则
来源：http://ni.huanxung.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mp.yuexingan06.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pw.shtwfgs.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lp.nicolike.cn

TS:   if (!x) {}
来源：http://nm.asd995.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wl.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://aj.huixinmuqiang.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zd.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zw.nicolike.cn

[A17] 位运算
来源：http://lu.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ni.muxihuayi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gz.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bv.yuntaijiaju.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mf.521024.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xg.szxytkj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kk.colortex.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xd.huanxung.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xx.jianghongdianzi.cn

[A18] 字符与 ASCII 码互转
来源：http://ey.bjjhwx.cn

Py:   ord("A"); chr(65)
来源：http://vt.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://ii.newstarts.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pt.chemitech.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://st.nszjky.cn

Java: (int) 'A'; (char) 65
来源：http://ak.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mk.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://cw.shxzukj.cn

C#:   (int)'A'; (char)65
来源：http://jo.huanxung.cn

[A19] 交换两个变量
来源：http://pq.newstarts.cn

Py:   a, b = b, a
来源：http://dj.jianghongdianzi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://vx.9csxet.cn

JS:   [a, b] = [b, a];
来源：http://kk.shxzukj.cn

TS:   [a, b] = [b, a];
来源：http://ry.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://fs.panjiajie.cn

Go:   a, b = b, a
来源：http://do.asd995.cn

Ruby: a, b = b, a
来源：http://tw.nicolike.cn

C#:   (a, b) = (b, a);
来源：http://qm.jctech888.com.cn

[A20] 读取标准输入
来源：http://bi.szsharing.cn

Py:   name = input("请输入：")
来源：http://dh.9csxet.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fz.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mc.wgjwhj.cn

TS:   // Node.js：readline 模块
来源：http://qb.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://aj.yuntaijiaju.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ok.hnjuh.cn

Ruby: gets.chomp
来源：http://pd.szxytkj.cn

C#:   Console.ReadLine();
来源：http://vd.colortex.cn

[A21] 保留指定小数位输出
来源：http://ye.shxzukj.cn

Py:   f"{3.14159:.2f}"
来源：http://ho.hahajie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jw.nszjky.cn

JS:   (3.14159).toFixed(2)
来源：http://tg.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://ox.gzmigu.cn

Java: String.format("%.2f", 3.14159)
来源：http://hx.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://av.huanxung.cn

Ruby: format("%.2f", 3.14159)
来源：http://bi.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://ja.panjiajie.cn

[A22] 获取字符串长度
来源：http://mz.muxihuayi.cn

Py:   len(s)
来源：http://jy.haigaiapp.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gn.bjjhwx.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xt.shxzukj.cn

TS:   s.length
来源：http://zg.yuexingan06.cn

Java: s.length()
来源：http://yy.521024.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qn.panjiajie.cn

Ruby: s.length
来源：http://fb.shtwfgs.cn

C#:   s.Length
来源：http://ax.shxzskj.cn

[A23] 大小写转换
来源：http://su.szxytkj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hs.lnxyls.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zb.huixinmuqiang.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wq.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hg.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zc.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zt.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eu.bjjhwx.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://of.hnjuh.cn

[A24] 去除首尾空白
来源：http://lw.521024.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hp.wgjwhj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nl.shxzukj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fd.colortex.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hm.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ix.colortex.cn

Go:   strings.TrimSpace(s)
来源：http://dv.nszjky.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lc.szsharing.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ej.9csxet.cn

[A25] 字符串比较
来源：http://hg.szxytkj.cn

Py:   s1 == s2; s1 != s2
来源：http://hu.haigaiapp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bi.huixinmuqiang.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ej.bjjhwx.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sl.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uy.newstarts.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bs.asd995.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://td.bjjhwx.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sh.shxzskj.cn

[A26] 类型转换总览
来源：http://fj.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wf.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dr.huanxung.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bc.jctech888.com.cn

TS:   Number() String() Boolean() x as number
来源：http://kb.9csxet.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ge.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ll.huixiangedu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://uz.huanxung.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gj.shxzukj.cn

================================================================================
来源：http://ts.jctech888.com.cn

B. 流程控制
来源：http://op.hahajie.cn

================================================================================
来源：http://qm.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://fs.jctech888.com.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://db.newstarts.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gt.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dc.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rb.szsharing.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xw.gzmigu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hr.wgjwhj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mv.shxzskj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tb.lnxyls.cn

[B02] 多分支 else if / elif
来源：http://of.jianghongdianzi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bx.panjiajie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ze.521024.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mn.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://us.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cq.shxzukj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hb.huanxung.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jc.bookmarksfly.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fh.nicolike.cn

[B03] switch / match / case
来源：http://ge.szsharing.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jv.wgjwhj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wh.lnxyls.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ao.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://px.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pd.yuntaijiaju.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yq.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rx.huixiangedu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tv.nszjky.cn

[B04] for 计数循环
来源：http://jd.521024.cn

Py:   for i in range(10): print(i)
来源：http://kv.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mm.newstarts.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ci.asd995.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mu.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fn.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://so.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://ii.haigaiapp.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fd.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://my.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://wu.huixiangedu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://az.wgjwhj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iy.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ds.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wd.9csxet.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gb.shxzskj.cn

Ruby: arr.each { |item| puts item }
来源：http://ur.nszjky.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://er.colortex.cn

[B06] 遍历字典 / 对象
来源：http://jz.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ob.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eb.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pa.nszjky.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jf.muxihuayi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tc.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gc.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wj.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ee.haigaiapp.cn

[B07] while 循环
来源：http://dv.szxytkj.cn

Py:   while i < 10: i += 1
来源：http://dm.nszjky.cn

PHP:  while ($i < 10) { $i++; }
来源：http://re.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://za.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://wf.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://gc.huanxung.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hh.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://dh.newstarts.cn

C#:   while (i < 10) { i++; }
来源：http://pf.jctech888.com.cn

[B08] do-while（至少执行一次）
来源：http://zc.newstarts.cn

Py:   # 无 do-while：用 while True + break
来源：http://lw.newstarts.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ij.bookmarksfly.cn

JS:   do { i++; } while (i < 10);
来源：http://ja.shxzukj.cn

TS:   do { i++; } while (i < 10);
来源：http://jz.shtwfgs.cn

Java: do { i++; } while (i < 10);
来源：http://lj.hnjuh.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yj.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ao.hahajie.cn

C#:   do { i++; } while (i < 10);
来源：http://kl.shxzskj.cn

[B09] break 与 continue
来源：http://lf.huixinmuqiang.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yn.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cr.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ej.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tr.521024.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qr.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nf.huixinmuqiang.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sc.huixinmuqiang.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hq.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://gy.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uh.shxzukj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ss.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yk.jctech888.com.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lf.asd995.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://re.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hw.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://np.panjiajie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wz.asd995.cn

[B11] 生成数字序列 / 区间
来源：http://qj.asd995.cn

Py:   list(range(0, 10, 2))
来源：http://up.asd995.cn

PHP:  range(0, 10, 2);
来源：http://cr.szxytkj.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sl.newstarts.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fd.newstarts.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dm.yuntaijiaju.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gi.bookmarksfly.cn

Ruby: (0...10).step(2).to_a
来源：http://sl.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qr.huanxung.cn

[B12] 跳出多层循环
来源：http://jq.huixiangedu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://av.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eu.haigaiapp.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tn.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kp.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wl.521024.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qt.hnjuh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://po.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ee.shxzukj.cn

[B13] 判断是否为数字
来源：http://do.yuntaijiaju.cn

Py:   isinstance(x, (int, float))
来源：http://rw.newstarts.cn

PHP:  is_numeric($x)
来源：http://lo.szsharing.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dn.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uc.521024.cn

Java: x instanceof Number
来源：http://sk.bjjhwx.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mt.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://us.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://kl.jianghongdianzi.cn

[B14] 判断值是否在集合内
来源：http://gj.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://np.yuexingan06.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xe.521024.cn

JS:   [1, 2, 3].includes(x)
来源：http://jl.yuexingan06.cn

TS:   [1, 2, 3].includes(x)
来源：http://vj.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wu.newstarts.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ru.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ab.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ru.asd995.cn

[B15] 布尔运算与取反
来源：http://fp.jctech888.com.cn

Py:   a and b or not c
来源：http://yp.panjiajie.cn

PHP:  $a && $b || !$c
来源：http://hd.szsharing.cn

JS:   a && b || !c
来源：http://se.wgjwhj.cn

TS:   a && b || !c
来源：http://ul.jianghongdianzi.cn

Java: a && b || !c
来源：http://nk.521024.cn

Go:   a && b || !c
来源：http://em.9csxet.cn

Ruby: a && b || !c
来源：http://zr.hahajie.cn

C#:   a && b || !c
来源：http://eb.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://wp.9csxet.cn

Py:   if not data: return
来源：http://fb.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://ju.shxzukj.cn

JS:   if (!data) return;
来源：http://ey.szxytkj.cn

TS:   if (!data) return;
来源：http://uo.gzmigu.cn

Java: if (data == null) return;
来源：http://rd.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://ej.nicolike.cn

Ruby: return if data.nil?
来源：http://hu.newstarts.cn

C#:   if (data == null) return;
来源：http://ra.521024.cn

================================================================================
来源：http://cp.huixiangedu.cn

C. 函数与作用域
来源：http://az.wgjwhj.cn

================================================================================
来源：http://oe.wgjwhj.cn

[C01] 定义函数
来源：http://hw.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://js.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vb.muxihuayi.cn

JS:   function add(a, b) { return a + b; }
来源：http://cd.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ps.bjjhwx.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://un.bookmarksfly.cn

Go:   func add(a, b int) int { return a + b }
来源：http://td.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://gf.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lb.lnxyls.cn


<!-- 参考信息 -->