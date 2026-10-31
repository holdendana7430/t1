代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ku.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ol.muxihuayi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://oa.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lw.szxytkj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sj.szxytkj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qy.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uc.yuexingan06.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pt.jctech888.com.cn

[A10] 生成随机数
来源：http://yn.hnjuh.cn

Py:   import random; random.randint(1, 100)
来源：http://cq.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://aj.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jl.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://em.jctech888.com.cn

Java: new Random().nextInt(100) + 1
来源：http://aa.shxzukj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://za.newstarts.cn

Ruby: rand(1..100)
来源：http://yv.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://gx.9csxet.cn

[A11] 条件表达式（三元）
来源：http://wr.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://qj.szxytkj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xq.panjiajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://va.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://aa.bjjhwx.cn

Java: x > 0 ? "yes" : "no"
来源：http://mx.newstarts.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zu.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kq.wgjwhj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://dd.shxzukj.cn

[A12] 字符串插值 / 格式化
来源：http://vu.nszjky.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hr.nicolike.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nk.huixiangedu.cn

JS:   `Hello, ${name}!`
来源：http://jy.shxzukj.cn

TS:   `Hello, ${name}!`
来源：http://dq.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://hr.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cg.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://nj.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://wz.chemitech.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://lh.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://rq.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://tp.szsharing.cn

JS:   "第一行\n第二行"
来源：http://er.colortex.cn

TS:   "第一行\n第二行"
来源：http://ij.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://eo.huanxung.cn

Go:   "第一行\n第二行"
来源：http://cb.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://bx.lnxyls.cn

C#:   "第一行\n第二行"
来源：http://ie.muxihuayi.cn

[A14] 注释写法
来源：http://qd.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xe.szsharing.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bb.bjjhwx.cn

JS:   // 单行；/* 多行 */
来源：http://jk.bookmarksfly.cn

TS:   // 单行；/* 多行 */
来源：http://lj.bjjhwx.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jj.szsharing.cn

Go:   // 单行；/* 多行 */
来源：http://cx.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hs.huixinmuqiang.cn

C#:   // 单行；/* 多行 */
来源：http://po.szxytkj.cn

[A15] 空值判断与默认值
来源：http://sq.colortex.cn

Py:   value = data or "默认值"
来源：http://rj.panjiajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://zp.szxytkj.cn

JS:   const value = data ?? "默认值";
来源：http://wd.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://jo.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gm.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://lk.shxzukj.cn

Ruby: value = data || "默认值"
来源：http://et.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://yg.hnjuh.cn

[A16] 真假值判断规则
来源：http://pd.jianghongdianzi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hl.bjjhwx.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uk.bookmarksfly.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xj.haigaiapp.cn

TS:   if (!x) {}
来源：http://kl.jianghongdianzi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uq.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fa.shtwfgs.cn

Ruby: unless x            # nil 与 false 为假
来源：http://bv.9csxet.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kw.hnjuh.cn

[A17] 位运算
来源：http://ib.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kj.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xx.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vy.bjjhwx.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nn.shxzukj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lw.hnjuh.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ux.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ob.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zf.szsharing.cn

[A18] 字符与 ASCII 码互转
来源：http://mf.yuexingan06.cn

Py:   ord("A"); chr(65)
来源：http://bh.nszjky.cn

PHP:  ord("A"); chr(65)
来源：http://lt.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fs.szsharing.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ah.szxytkj.cn

Java: (int) 'A'; (char) 65
来源：http://ta.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rn.shxzskj.cn

Ruby: "A".ord; 65.chr
来源：http://qd.gzmigu.cn

C#:   (int)'A'; (char)65
来源：http://yr.9csxet.cn

[A19] 交换两个变量
来源：http://zl.9csxet.cn

Py:   a, b = b, a
来源：http://wo.colortex.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://em.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://hw.yuntaijiaju.cn

TS:   [a, b] = [b, a];
来源：http://mi.huanxung.cn

Java: int t = a; a = b; b = t;
来源：http://ql.jianghongdianzi.cn

Go:   a, b = b, a
来源：http://zl.huanxung.cn

Ruby: a, b = b, a
来源：http://nc.gzmigu.cn

C#:   (a, b) = (b, a);
来源：http://ud.shxzukj.cn

[A20] 读取标准输入
来源：http://ov.hnjuh.cn

Py:   name = input("请输入：")
来源：http://jt.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ki.szxytkj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kq.shxzukj.cn

TS:   // Node.js：readline 模块
来源：http://az.colortex.cn

Java: new Scanner(System.in).nextLine()
来源：http://ul.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gg.shxzskj.cn

Ruby: gets.chomp
来源：http://lu.nicolike.cn

C#:   Console.ReadLine();
来源：http://ol.asd995.cn

[A21] 保留指定小数位输出
来源：http://qe.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://ld.haigaiapp.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rg.szxytkj.cn

JS:   (3.14159).toFixed(2)
来源：http://st.haigaiapp.cn

TS:   (3.14159).toFixed(2)
来源：http://ms.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://kv.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pt.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://bp.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://po.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://cr.9csxet.cn

Py:   len(s)
来源：http://yl.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pd.nicolike.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nf.huanxung.cn

TS:   s.length
来源：http://xe.hnjuh.cn

Java: s.length()
来源：http://gz.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://si.shxzskj.cn

Ruby: s.length
来源：http://sl.asd995.cn

C#:   s.Length
来源：http://vn.haigaiapp.cn

[A23] 大小写转换
来源：http://ol.nszjky.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gh.shxzukj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fq.nicolike.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ou.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vf.muxihuayi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kt.szxytkj.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sr.newstarts.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oc.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xu.lnxyls.cn

[A24] 去除首尾空白
来源：http://aa.9csxet.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ko.hahajie.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hs.lnxyls.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gb.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tk.521024.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vc.hahajie.cn

Go:   strings.TrimSpace(s)
来源：http://by.huanxung.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eu.shtwfgs.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lv.szsharing.cn

[A25] 字符串比较
来源：http://me.gzmigu.cn

Py:   s1 == s2; s1 != s2
来源：http://ns.hahajie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pi.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qn.haigaiapp.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bt.shxzukj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cy.bjjhwx.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ug.szsharing.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ze.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pg.huixinmuqiang.cn

[A26] 类型转换总览
来源：http://gk.yuntaijiaju.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zl.wgjwhj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dg.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fo.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://ls.muxihuayi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zb.bjjhwx.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pf.asd995.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tk.szsharing.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lr.szxytkj.cn

================================================================================
来源：http://nd.jctech888.com.cn

B. 流程控制
来源：http://rk.wgjwhj.cn

================================================================================
来源：http://di.bookmarksfly.cn

[B01] 条件判断 if / else
来源：http://cu.hahajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ds.521024.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ok.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wj.yuntaijiaju.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jn.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ft.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qs.nszjky.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rj.huixiangedu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ow.nszjky.cn

[B02] 多分支 else if / elif
来源：http://md.szxytkj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qn.shxzskj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pc.muxihuayi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jf.bookmarksfly.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wp.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eq.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ci.jctech888.com.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://us.haigaiapp.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rz.szxytkj.cn

[B03] switch / match / case
来源：http://zk.panjiajie.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ix.colortex.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wv.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cb.shxzskj.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://po.panjiajie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ud.nszjky.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rc.szsharing.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fi.nszjky.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mc.shxzukj.cn

[B04] for 计数循环
来源：http://ai.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://se.shxzukj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pa.yuntaijiaju.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bi.chemitech.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cr.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cj.nicolike.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mc.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://no.hahajie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dn.newstarts.cn

[B05] 遍历数组 / 列表
来源：http://yu.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://vk.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xf.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sa.9csxet.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cw.bjjhwx.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nm.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rj.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://rw.panjiajie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://es.521024.cn

[B06] 遍历字典 / 对象
来源：http://xh.chemitech.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mo.yuexingan06.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fb.chemitech.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sj.gzmigu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vs.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ou.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vi.bookmarksfly.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ou.hahajie.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cx.bjjhwx.cn

[B07] while 循环
来源：http://od.jctech888.com.cn

Py:   while i < 10: i += 1
来源：http://wn.chemitech.net.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kp.nicolike.cn

JS:   while (i < 10) { i++; }
来源：http://js.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://ds.gzmigu.cn

Java: while (i < 10) { i++; }
来源：http://ov.szsharing.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vt.shxzukj.cn

Ruby: while i < 10; i += 1; end
来源：http://jc.gzmigu.cn

C#:   while (i < 10) { i++; }
来源：http://tn.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://kc.muxihuayi.cn

Py:   # 无 do-while：用 while True + break
来源：http://up.yuntaijiaju.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kz.wgjwhj.cn

JS:   do { i++; } while (i < 10);
来源：http://sm.szxytkj.cn

TS:   do { i++; } while (i < 10);
来源：http://xq.bjjhwx.cn

Java: do { i++; } while (i < 10);
来源：http://jj.wgjwhj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://if.huixiangedu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gn.wgjwhj.cn

C#:   do { i++; } while (i < 10);
来源：http://aq.hnjuh.cn

[B09] break 与 continue
来源：http://zp.chemitech.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nz.jctech888.com.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qo.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uj.panjiajie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hc.szsharing.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qp.jianghongdianzi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uh.bjjhwx.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ax.nicolike.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sq.wgjwhj.cn

[B10] 遍历同时拿索引
来源：http://jv.hahajie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://et.gzmigu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ru.chemitech.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://po.gzmigu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://le.yuexingan06.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://py.shtwfgs.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xt.521024.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yq.521024.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nd.lnxyls.cn

[B11] 生成数字序列 / 区间
来源：http://nl.szxytkj.cn

Py:   list(range(0, 10, 2))
来源：http://ry.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://cg.haigaiapp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vn.nicolike.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ds.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ib.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wh.haigaiapp.cn

Ruby: (0...10).step(2).to_a
来源：http://dr.huixiangedu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wj.shxzskj.cn

[B12] 跳出多层循环
来源：http://jd.shtwfgs.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fy.gzmigu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ex.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ov.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lp.jctech888.com.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tq.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kb.nicolike.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qg.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wl.huanxung.cn

[B13] 判断是否为数字
来源：http://kt.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://ot.gzmigu.cn

PHP:  is_numeric($x)
来源：http://kn.yuntaijiaju.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kk.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qv.colortex.cn

Java: x instanceof Number
来源：http://dr.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tv.bookmarksfly.cn

Ruby: x.is_a?(Numeric)
来源：http://ka.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://pd.nicolike.cn

[B14] 判断值是否在集合内
来源：http://bz.gzmigu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cp.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lw.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://hr.bookmarksfly.cn

TS:   [1, 2, 3].includes(x)
来源：http://si.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dm.hnjuh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wm.hahajie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ek.lnxyls.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fd.panjiajie.cn

[B15] 布尔运算与取反
来源：http://ei.huixiangedu.cn

Py:   a and b or not c
来源：http://az.haigaiapp.cn

PHP:  $a && $b || !$c
来源：http://rc.bjjhwx.cn

JS:   a && b || !c
来源：http://ag.shxzskj.cn

TS:   a && b || !c
来源：http://kz.bjjhwx.cn

Java: a && b || !c
来源：http://ld.szsharing.cn

Go:   a && b || !c
来源：http://cn.lnxyls.cn

Ruby: a && b || !c
来源：http://hu.huanxung.cn

C#:   a && b || !c
来源：http://ar.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bu.haigaiapp.cn


<!-- 参考信息 -->