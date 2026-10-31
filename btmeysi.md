代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://pi.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://jz.colortex.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dx.szsharing.cn

Ruby: rand(1..100)
来源：http://mm.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://qa.gzmigu.cn

[A11] 条件表达式（三元）
来源：http://ip.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://pq.nszjky.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://eh.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cs.haigaiapp.cn

TS:   x > 0 ? "yes" : "no"
来源：http://mv.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://gf.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dj.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zw.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ku.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://qj.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ae.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://in.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://zi.szxytkj.cn

TS:   `Hello, ${name}!`
来源：http://wz.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://my.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://aw.bjjhwx.cn

Ruby: "Hello, #{name}!"
来源：http://il.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://hv.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hv.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://xo.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://ib.wgjwhj.cn

JS:   "第一行\n第二行"
来源：http://qj.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://un.haigaiapp.cn

Java: "第一行\n第二行"
来源：http://tp.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://vw.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://wg.9csxet.cn

C#:   "第一行\n第二行"
来源：http://qg.hnjuh.cn

[A14] 注释写法
来源：http://wd.huixiangedu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qd.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://tc.huixiangedu.cn

JS:   // 单行；/* 多行 */
来源：http://ho.szxytkj.cn

TS:   // 单行；/* 多行 */
来源：http://ta.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tv.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://zy.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ou.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://ys.nicolike.cn

[A15] 空值判断与默认值
来源：http://wi.huixinmuqiang.cn

Py:   value = data or "默认值"
来源：http://pq.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://yv.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://tv.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://fl.haigaiapp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fu.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://uc.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://if.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://kc.huixinmuqiang.cn

[A16] 真假值判断规则
来源：http://sw.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nc.newstarts.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://av.nicolike.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ki.wgjwhj.cn

TS:   if (!x) {}
来源：http://hy.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://aw.szxytkj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vu.colortex.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xt.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nl.yuexingan06.cn

[A17] 位运算
来源：http://jk.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oz.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nc.bjjhwx.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://km.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gm.bookmarksfly.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gv.9csxet.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yw.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vi.shtwfgs.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jj.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://sn.nszjky.cn

Py:   ord("A"); chr(65)
来源：http://wj.chemitech.net.cn

PHP:  ord("A"); chr(65)
来源：http://mw.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ot.shxzskj.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vq.lnxyls.cn

Java: (int) 'A'; (char) 65
来源：http://it.yuntaijiaju.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nv.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://uf.colortex.cn

C#:   (int)'A'; (char)65
来源：http://zl.nszjky.cn

[A19] 交换两个变量
来源：http://pr.hahajie.cn

Py:   a, b = b, a
来源：http://pf.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ed.hahajie.cn

JS:   [a, b] = [b, a];
来源：http://iw.szsharing.cn

TS:   [a, b] = [b, a];
来源：http://is.muxihuayi.cn

Java: int t = a; a = b; b = t;
来源：http://ur.521024.cn

Go:   a, b = b, a
来源：http://fj.huanxung.cn

Ruby: a, b = b, a
来源：http://wf.jctech888.com.cn

C#:   (a, b) = (b, a);
来源：http://tq.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://nv.yuexingan06.cn

Py:   name = input("请输入：")
来源：http://jv.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mt.hnjuh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nz.hnjuh.cn

TS:   // Node.js：readline 模块
来源：http://yp.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://yg.szxytkj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ga.shtwfgs.cn

Ruby: gets.chomp
来源：http://vt.nicolike.cn

C#:   Console.ReadLine();
来源：http://fy.shtwfgs.cn

[A21] 保留指定小数位输出
来源：http://ne.hnjuh.cn

Py:   f"{3.14159:.2f}"
来源：http://au.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ck.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://rm.gzmigu.cn

TS:   (3.14159).toFixed(2)
来源：http://lr.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://za.shxzskj.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yn.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://pd.521024.cn

C#:   3.14159.ToString("F2")
来源：http://hj.lnxyls.cn

[A22] 获取字符串长度
来源：http://rx.shtwfgs.cn

Py:   len(s)
来源：http://gy.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vv.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xu.asd995.cn

TS:   s.length
来源：http://ay.szsharing.cn

Java: s.length()
来源：http://mp.nszjky.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sm.huixinmuqiang.cn

Ruby: s.length
来源：http://qn.wgjwhj.cn

C#:   s.Length
来源：http://xw.colortex.cn

[A23] 大小写转换
来源：http://pq.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bq.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iu.jianghongdianzi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oq.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cz.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nj.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tu.colortex.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gs.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://eg.huanxung.cn

[A24] 去除首尾空白
来源：http://du.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xa.nszjky.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ge.haigaiapp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://um.jianghongdianzi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ig.hahajie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ww.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://dr.yuntaijiaju.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gm.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xr.chemitech.net.cn

[A25] 字符串比较
来源：http://vt.jctech888.com.cn

Py:   s1 == s2; s1 != s2
来源：http://bw.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tb.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ev.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nb.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://du.shxzukj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gr.huanxung.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wi.521024.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://no.nszjky.cn

[A26] 类型转换总览
来源：http://ll.nszjky.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ec.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://by.szsharing.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rs.gzmigu.cn

TS:   Number() String() Boolean() x as number
来源：http://qp.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zl.haigaiapp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mp.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://px.asd995.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nz.yuntaijiaju.cn

================================================================================
来源：http://jk.hahajie.cn

B. 流程控制
来源：http://ok.panjiajie.cn

================================================================================
来源：http://fn.hnjuh.cn

[B01] 条件判断 if / else
来源：http://os.huixiangedu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yy.huixinmuqiang.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dl.bookmarksfly.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vd.newstarts.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wc.lnxyls.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jr.huanxung.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kc.hahajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qo.asd995.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ps.szxytkj.cn

[B02] 多分支 else if / elif
来源：http://ka.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tv.521024.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xr.shxzukj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aa.colortex.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xk.lnxyls.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hf.panjiajie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dg.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vz.newstarts.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://db.jianghongdianzi.cn

[B03] switch / match / case
来源：http://jt.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qi.huixiangedu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ye.huanxung.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kk.huanxung.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ib.shxzukj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dm.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gm.bjjhwx.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gj.bjjhwx.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xx.shtwfgs.cn

[B04] for 计数循环
来源：http://fr.shxzskj.cn

Py:   for i in range(10): print(i)
来源：http://yn.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ax.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bw.521024.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gw.9csxet.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lv.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://or.lnxyls.cn

Ruby: 10.times { |i| puts i }
来源：http://et.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ou.shxzukj.cn

[B05] 遍历数组 / 列表
来源：http://jq.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://kh.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hm.shxzskj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mr.huanxung.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lk.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://um.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oo.huixiangedu.cn

Ruby: arr.each { |item| puts item }
来源：http://xc.chemitech.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gl.huixinmuqiang.cn

[B06] 遍历字典 / 对象
来源：http://ag.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ye.panjiajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yt.521024.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ua.huixiangedu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vg.colortex.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yl.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nj.huixiangedu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wx.gzmigu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sd.panjiajie.cn

[B07] while 循环
来源：http://qx.asd995.cn

Py:   while i < 10: i += 1
来源：http://pr.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dq.shxzukj.cn

JS:   while (i < 10) { i++; }
来源：http://en.bjjhwx.cn

TS:   while (i < 10) { i++; }
来源：http://hr.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://zg.nicolike.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jy.nicolike.cn

Ruby: while i < 10; i += 1; end
来源：http://ta.yuexingan06.cn

C#:   while (i < 10) { i++; }
来源：http://wi.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://bd.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://io.hahajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fz.haigaiapp.cn

JS:   do { i++; } while (i < 10);
来源：http://cp.gzmigu.cn

TS:   do { i++; } while (i < 10);
来源：http://uo.9csxet.cn

Java: do { i++; } while (i < 10);
来源：http://zh.huanxung.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gh.szsharing.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wv.nszjky.cn

C#:   do { i++; } while (i < 10);
来源：http://jo.lnxyls.cn

[B09] break 与 continue
来源：http://ex.colortex.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mv.hahajie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rc.bookmarksfly.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.haigaiapp.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wv.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://js.szxytkj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://km.shxzskj.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gg.bookmarksfly.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cv.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://cj.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://it.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ab.gzmigu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jo.huixinmuqiang.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xm.521024.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mn.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sf.shxzukj.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ux.shxzukj.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fa.panjiajie.cn

[B11] 生成数字序列 / 区间
来源：http://ev.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://gw.asd995.cn

PHP:  range(0, 10, 2);
来源：http://zu.bookmarksfly.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cb.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nh.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://da.muxihuayi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jy.wgjwhj.cn

Ruby: (0...10).step(2).to_a
来源：http://nh.yuexingan06.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cl.huixiangedu.cn

[B12] 跳出多层循环
来源：http://se.muxihuayi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gc.chemitech.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tr.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nz.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pd.muxihuayi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yn.huixiangedu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fb.jctech888.com.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pg.hnjuh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qu.szxytkj.cn

[B13] 判断是否为数字
来源：http://xc.jctech888.com.cn

Py:   isinstance(x, (int, float))
来源：http://qv.wgjwhj.cn

PHP:  is_numeric($x)
来源：http://wr.chemitech.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dh.huixinmuqiang.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xd.bookmarksfly.cn

Java: x instanceof Number
来源：http://lv.shtwfgs.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lq.9csxet.cn

Ruby: x.is_a?(Numeric)
来源：http://ka.jianghongdianzi.cn

C#:   x is int or double or decimal
来源：http://gi.huanxung.cn

[B14] 判断值是否在集合内
来源：http://cs.szxytkj.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://su.lnxyls.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://no.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://cq.chemitech.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://zk.huixiangedu.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xd.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fz.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://da.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fe.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://aj.bookmarksfly.cn

Py:   a and b or not c
来源：http://kp.hnjuh.cn

PHP:  $a && $b || !$c
来源：http://ba.muxihuayi.cn

JS:   a && b || !c
来源：http://pf.bookmarksfly.cn

TS:   a && b || !c
来源：http://yu.shxzukj.cn

Java: a && b || !c
来源：http://yn.9csxet.cn

Go:   a && b || !c
来源：http://mv.huanxung.cn

Ruby: a && b || !c
来源：http://re.chemitech.net.cn

C#:   a && b || !c
来源：http://zx.huanxung.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dr.huixiangedu.cn

Py:   if not data: return
来源：http://yu.huanxung.cn

PHP:  if (!$data) { return; }
来源：http://ck.newstarts.cn

JS:   if (!data) return;
来源：http://yk.nicolike.cn

TS:   if (!data) return;
来源：http://pi.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://ru.colortex.cn

Go:   if data == nil { return }
来源：http://km.shtwfgs.cn

Ruby: return if data.nil?
来源：http://pq.huixiangedu.cn

C#:   if (data == null) return;
来源：http://mb.jianghongdianzi.cn

================================================================================
来源：http://js.shxzskj.cn

C. 函数与作用域
来源：http://ev.panjiajie.cn

================================================================================
来源：http://ar.nicolike.cn

[C01] 定义函数
来源：http://kk.chemitech.net.cn


<!-- 参考信息 -->