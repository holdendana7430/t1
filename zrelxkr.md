代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://al.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://jz.huixinmuqiang.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ta.521024.cn

Ruby: rand(1..100)
来源：http://mh.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://wx.hahajie.cn

[A11] 条件表达式（三元）
来源：http://jx.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://nn.huanxung.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://og.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ck.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gq.bookmarksfly.cn

Java: x > 0 ? "yes" : "no"
来源：http://ha.chemitech.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jw.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lk.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mt.wgjwhj.cn

[A12] 字符串插值 / 格式化
来源：http://fj.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uo.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qr.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://ax.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://pc.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://mu.bjjhwx.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xd.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://vi.nicolike.cn

C#:   $"Hello, {name}!"
来源：http://kj.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ph.huanxung.cn

Py:   "第一行\n第二行"
来源：http://fa.nicolike.cn

PHP:  "第一行\n第二行"
来源：http://rf.chemitech.net.cn

JS:   "第一行\n第二行"
来源：http://kv.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://jq.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://db.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://ws.shtwfgs.cn

Ruby: "第一行\n第二行"
来源：http://wp.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://ct.huixinmuqiang.cn

[A14] 注释写法
来源：http://cq.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gv.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ld.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://df.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://iq.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mh.521024.cn

Go:   // 单行；/* 多行 */
来源：http://rm.nicolike.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kl.nszjky.cn

C#:   // 单行；/* 多行 */
来源：http://kh.hnjuh.cn

[A15] 空值判断与默认值
来源：http://eq.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://yn.gzmigu.cn

PHP:  $value = $data ?? "默认值";
来源：http://sf.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://cl.hnjuh.cn

TS:   const value = data ?? "默认值";
来源：http://do.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bb.yuntaijiaju.cn

Go:   if data == "" { data = "默认值" }
来源：http://tp.9csxet.cn

Ruby: value = data || "默认值"
来源：http://no.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://si.szxytkj.cn

[A16] 真假值判断规则
来源：http://lw.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ep.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zn.shxzukj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ai.bookmarksfly.cn

TS:   if (!x) {}
来源：http://ho.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dv.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yb.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lj.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fv.newstarts.cn

[A17] 位运算
来源：http://qx.shtwfgs.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ql.huixiangedu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pw.shxzukj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cx.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pc.shtwfgs.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ni.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ei.shtwfgs.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oz.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xk.newstarts.cn

[A18] 字符与 ASCII 码互转
来源：http://jd.haigaiapp.cn

Py:   ord("A"); chr(65)
来源：http://lk.hnjuh.cn

PHP:  ord("A"); chr(65)
来源：http://xk.shtwfgs.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tq.nszjky.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://as.szsharing.cn

Java: (int) 'A'; (char) 65
来源：http://zr.chemitech.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lj.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://ub.shxzskj.cn

C#:   (int)'A'; (char)65
来源：http://mk.9csxet.cn

[A19] 交换两个变量
来源：http://tc.szxytkj.cn

Py:   a, b = b, a
来源：http://fy.hahajie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nj.haigaiapp.cn

JS:   [a, b] = [b, a];
来源：http://eg.shtwfgs.cn

TS:   [a, b] = [b, a];
来源：http://in.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://kq.panjiajie.cn

Go:   a, b = b, a
来源：http://wg.hahajie.cn

Ruby: a, b = b, a
来源：http://fr.bjjhwx.cn

C#:   (a, b) = (b, a);
来源：http://st.521024.cn

[A20] 读取标准输入
来源：http://gm.521024.cn

Py:   name = input("请输入：")
来源：http://wm.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://mp.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xd.gzmigu.cn

TS:   // Node.js：readline 模块
来源：http://eu.panjiajie.cn

Java: new Scanner(System.in).nextLine()
来源：http://lf.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fd.szsharing.cn

Ruby: gets.chomp
来源：http://xn.huixiangedu.cn

C#:   Console.ReadLine();
来源：http://sc.asd995.cn

[A21] 保留指定小数位输出
来源：http://pm.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://ib.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cm.chemitech.net.cn

JS:   (3.14159).toFixed(2)
来源：http://cd.asd995.cn

TS:   (3.14159).toFixed(2)
来源：http://pw.muxihuayi.cn

Java: String.format("%.2f", 3.14159)
来源：http://yx.colortex.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cx.colortex.cn

Ruby: format("%.2f", 3.14159)
来源：http://oz.lnxyls.cn

C#:   3.14159.ToString("F2")
来源：http://ft.colortex.cn

[A22] 获取字符串长度
来源：http://so.chemitech.net.cn

Py:   len(s)
来源：http://hx.wgjwhj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wy.shtwfgs.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mw.huixiangedu.cn

TS:   s.length
来源：http://qq.szxytkj.cn

Java: s.length()
来源：http://eu.huixiangedu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ma.hahajie.cn

Ruby: s.length
来源：http://rh.yuntaijiaju.cn

C#:   s.Length
来源：http://zp.muxihuayi.cn

[A23] 大小写转换
来源：http://oq.shtwfgs.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xb.panjiajie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rb.shxzskj.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tk.wgjwhj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uw.colortex.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dx.bookmarksfly.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ca.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fs.szsharing.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vi.shxzskj.cn

[A24] 去除首尾空白
来源：http://gr.newstarts.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nz.huixiangedu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ve.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pj.nicolike.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://es.jianghongdianzi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jh.shxzskj.cn

Go:   strings.TrimSpace(s)
来源：http://ni.521024.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fs.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ke.yuexingan06.cn

[A25] 字符串比较
来源：http://rh.wgjwhj.cn

Py:   s1 == s2; s1 != s2
来源：http://pj.hnjuh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vr.colortex.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://we.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jo.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qv.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ln.wgjwhj.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lj.hahajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kc.nicolike.cn

[A26] 类型转换总览
来源：http://vz.muxihuayi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xs.lnxyls.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qt.shtwfgs.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xe.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://fm.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://od.shxzskj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bn.szsharing.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://av.nszjky.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wk.newstarts.cn

================================================================================
来源：http://zk.haigaiapp.cn

B. 流程控制
来源：http://au.jianghongdianzi.cn

================================================================================
来源：http://wi.huixinmuqiang.cn

[B01] 条件判断 if / else
来源：http://wa.yuntaijiaju.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tl.9csxet.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ka.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jg.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://az.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ul.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lt.huixiangedu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ls.nszjky.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mz.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://qk.wgjwhj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ap.bjjhwx.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jo.asd995.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://az.muxihuayi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tk.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gl.jctech888.com.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xa.9csxet.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sg.nicolike.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pu.newstarts.cn

[B03] switch / match / case
来源：http://xo.asd995.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://to.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ir.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fb.nszjky.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dt.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gv.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jd.huixiangedu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ei.bookmarksfly.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ja.haigaiapp.cn

[B04] for 计数循环
来源：http://xn.szsharing.cn

Py:   for i in range(10): print(i)
来源：http://zl.shxzskj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ev.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kj.gzmigu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fu.chemitech.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ir.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uk.huixiangedu.cn

Ruby: 10.times { |i| puts i }
来源：http://vn.lnxyls.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zv.huixiangedu.cn

[B05] 遍历数组 / 列表
来源：http://gh.shtwfgs.cn

Py:   for item in arr: print(item)
来源：http://du.huanxung.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mo.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ke.newstarts.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://od.chemitech.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ow.szsharing.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dt.hahajie.cn

Ruby: arr.each { |item| puts item }
来源：http://rd.bjjhwx.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qk.lnxyls.cn

[B06] 遍历字典 / 对象
来源：http://sn.jianghongdianzi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vg.nszjky.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gi.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nx.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nx.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vp.muxihuayi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qe.huixinmuqiang.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ns.newstarts.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wt.colortex.cn

[B07] while 循环
来源：http://qz.jianghongdianzi.cn

Py:   while i < 10: i += 1
来源：http://ci.shxzukj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vn.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://tq.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://xq.lnxyls.cn

Java: while (i < 10) { i++; }
来源：http://vg.hnjuh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ke.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://wg.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://fv.9csxet.cn

[B08] do-while（至少执行一次）
来源：http://jf.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://wy.jctech888.com.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pp.shxzukj.cn

JS:   do { i++; } while (i < 10);
来源：http://qh.chemitech.net.cn

TS:   do { i++; } while (i < 10);
来源：http://ql.shxzukj.cn

Java: do { i++; } while (i < 10);
来源：http://vb.chemitech.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dt.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ox.jctech888.com.cn

C#:   do { i++; } while (i < 10);
来源：http://go.shxzukj.cn

[B09] break 与 continue
来源：http://gx.haigaiapp.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fo.wgjwhj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ox.jctech888.com.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sc.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ei.panjiajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dm.gzmigu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zx.hnjuh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tm.muxihuayi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hp.shxzskj.cn

[B10] 遍历同时拿索引
来源：http://hv.szsharing.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zt.newstarts.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fp.9csxet.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nb.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dl.jctech888.com.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vr.gzmigu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ld.huixiangedu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qq.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ue.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://wu.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://jg.shtwfgs.cn

PHP:  range(0, 10, 2);
来源：http://xp.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ml.gzmigu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ah.szxytkj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iy.haigaiapp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://an.shtwfgs.cn

Ruby: (0...10).step(2).to_a
来源：http://sz.huixinmuqiang.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mb.9csxet.cn

[B12] 跳出多层循环
来源：http://gc.szsharing.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sw.szxytkj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hi.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cu.chemitech.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qw.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rk.hnjuh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pj.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xd.bookmarksfly.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ln.asd995.cn

[B13] 判断是否为数字
来源：http://vj.shtwfgs.cn

Py:   isinstance(x, (int, float))
来源：http://zf.hahajie.cn

PHP:  is_numeric($x)
来源：http://jk.hahajie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qr.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bu.jianghongdianzi.cn

Java: x instanceof Number
来源：http://gh.wgjwhj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fh.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://mn.521024.cn

C#:   x is int or double or decimal
来源：http://tj.jctech888.com.cn

[B14] 判断值是否在集合内
来源：http://vc.hahajie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qn.jianghongdianzi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ya.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://wu.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://lp.bookmarksfly.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rn.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ju.huixiangedu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dn.muxihuayi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wq.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://dx.9csxet.cn

Py:   a and b or not c
来源：http://bz.chemitech.net.cn

PHP:  $a && $b || !$c
来源：http://ho.huixinmuqiang.cn

JS:   a && b || !c
来源：http://ej.muxihuayi.cn

TS:   a && b || !c
来源：http://qx.9csxet.cn

Java: a && b || !c
来源：http://fi.huixiangedu.cn

Go:   a && b || !c
来源：http://br.bjjhwx.cn

Ruby: a && b || !c
来源：http://et.wgjwhj.cn

C#:   a && b || !c
来源：http://ow.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pg.szxytkj.cn

Py:   if not data: return
来源：http://jd.panjiajie.cn

PHP:  if (!$data) { return; }
来源：http://iy.521024.cn

JS:   if (!data) return;
来源：http://ma.hnjuh.cn

TS:   if (!data) return;
来源：http://mv.jianghongdianzi.cn

Java: if (data == null) return;
来源：http://ja.9csxet.cn

Go:   if data == nil { return }
来源：http://gh.shtwfgs.cn

Ruby: return if data.nil?
来源：http://lv.nicolike.cn

C#:   if (data == null) return;
来源：http://ql.hahajie.cn

================================================================================
来源：http://ol.huanxung.cn

C. 函数与作用域
来源：http://sy.newstarts.cn

================================================================================
来源：http://bv.huixinmuqiang.cn

[C01] 定义函数
来源：http://zr.panjiajie.cn


<!-- 参考信息 -->