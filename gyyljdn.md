代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yd.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://or.nszjky.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bg.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://yt.shxzukj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tb.gzmigu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nr.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ql.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zv.szsharing.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ru.szxytkj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zy.lnxyls.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lu.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gm.hnjuh.cn

[A10] 生成随机数
来源：http://op.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://dt.asd995.cn

PHP:  random_int(1, 100);
来源：http://ae.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rn.shxzukj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lz.szsharing.cn

Java: new Random().nextInt(100) + 1
来源：http://to.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://su.hnjuh.cn

Ruby: rand(1..100)
来源：http://da.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://bo.panjiajie.cn

[A11] 条件表达式（三元）
来源：http://pk.9csxet.cn

Py:   "yes" if x > 0 else "no"
来源：http://ym.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dt.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xo.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ob.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://lz.shxzskj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cw.yuexingan06.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lk.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rh.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://aq.yuexingan06.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bg.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jj.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://zo.shtwfgs.cn

TS:   `Hello, ${name}!`
来源：http://yz.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://uy.shxzskj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ux.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://jl.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://jd.panjiajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fw.hahajie.cn

Py:   "第一行\n第二行"
来源：http://zi.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://kl.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://wl.gzmigu.cn

TS:   "第一行\n第二行"
来源：http://jy.gzmigu.cn

Java: "第一行\n第二行"
来源：http://zt.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://xw.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://dy.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://qq.gzmigu.cn

[A14] 注释写法
来源：http://vy.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://eu.bjjhwx.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://jp.wgjwhj.cn

JS:   // 单行；/* 多行 */
来源：http://wd.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://dw.shxzukj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yd.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://vu.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ii.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://xu.huixinmuqiang.cn

[A15] 空值判断与默认值
来源：http://hk.huixiangedu.cn

Py:   value = data or "默认值"
来源：http://ux.haigaiapp.cn

PHP:  $value = $data ?? "默认值";
来源：http://ah.shxzukj.cn

JS:   const value = data ?? "默认值";
来源：http://ks.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://kg.bookmarksfly.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://iz.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://st.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://mk.wgjwhj.cn

C#:   var value = data ?? "默认值";
来源：http://wb.szxytkj.cn

[A16] 真假值判断规则
来源：http://es.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fz.yuntaijiaju.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kj.haigaiapp.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rz.hahajie.cn

TS:   if (!x) {}
来源：http://en.szxytkj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kg.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ul.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://kb.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bt.nszjky.cn

[A17] 位运算
来源：http://um.nszjky.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wi.lnxyls.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mr.bookmarksfly.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ei.muxihuayi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qg.haigaiapp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qi.panjiajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dz.hnjuh.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://td.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://id.lnxyls.cn

[A18] 字符与 ASCII 码互转
来源：http://da.wgjwhj.cn

Py:   ord("A"); chr(65)
来源：http://ap.hahajie.cn

PHP:  ord("A"); chr(65)
来源：http://ig.huanxung.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qn.jianghongdianzi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xq.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://ik.hnjuh.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ee.huixiangedu.cn

Ruby: "A".ord; 65.chr
来源：http://ke.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://ed.chemitech.net.cn

[A19] 交换两个变量
来源：http://dq.huixiangedu.cn

Py:   a, b = b, a
来源：http://bl.shxzukj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wt.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://im.huanxung.cn

TS:   [a, b] = [b, a];
来源：http://nc.jianghongdianzi.cn

Java: int t = a; a = b; b = t;
来源：http://bl.jctech888.com.cn

Go:   a, b = b, a
来源：http://vp.huixinmuqiang.cn

Ruby: a, b = b, a
来源：http://sa.wgjwhj.cn

C#:   (a, b) = (b, a);
来源：http://pj.bjjhwx.cn

[A20] 读取标准输入
来源：http://qv.shxzukj.cn

Py:   name = input("请输入：")
来源：http://yj.shtwfgs.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gq.colortex.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://au.newstarts.cn

TS:   // Node.js：readline 模块
来源：http://pt.bjjhwx.cn

Java: new Scanner(System.in).nextLine()
来源：http://zr.9csxet.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ew.asd995.cn

Ruby: gets.chomp
来源：http://bi.hahajie.cn

C#:   Console.ReadLine();
来源：http://nt.chemitech.net.cn

[A21] 保留指定小数位输出
来源：http://yd.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://fm.bookmarksfly.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mq.9csxet.cn

JS:   (3.14159).toFixed(2)
来源：http://cb.shxzukj.cn

TS:   (3.14159).toFixed(2)
来源：http://ct.newstarts.cn

Java: String.format("%.2f", 3.14159)
来源：http://bd.nszjky.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hn.bookmarksfly.cn

Ruby: format("%.2f", 3.14159)
来源：http://ac.hnjuh.cn

C#:   3.14159.ToString("F2")
来源：http://pr.huixinmuqiang.cn

[A22] 获取字符串长度
来源：http://am.muxihuayi.cn

Py:   len(s)
来源：http://gh.huixinmuqiang.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://la.huixinmuqiang.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yb.jctech888.com.cn

TS:   s.length
来源：http://oc.haigaiapp.cn

Java: s.length()
来源：http://vr.haigaiapp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cc.huixinmuqiang.cn

Ruby: s.length
来源：http://tv.asd995.cn

C#:   s.Length
来源：http://yb.newstarts.cn

[A23] 大小写转换
来源：http://sn.huixiangedu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xf.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ue.yuexingan06.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dj.panjiajie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wf.panjiajie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nd.huanxung.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hq.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://et.huanxung.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ap.hahajie.cn

[A24] 去除首尾空白
来源：http://hn.nicolike.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bp.haigaiapp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sk.huanxung.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cb.yuexingan06.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mi.szsharing.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jo.nszjky.cn

Go:   strings.TrimSpace(s)
来源：http://fr.colortex.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qe.wgjwhj.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xg.nszjky.cn

[A25] 字符串比较
来源：http://vg.newstarts.cn

Py:   s1 == s2; s1 != s2
来源：http://et.lnxyls.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dx.jianghongdianzi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xl.newstarts.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tc.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ld.yuexingan06.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lz.muxihuayi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ia.jctech888.com.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ff.muxihuayi.cn

[A26] 类型转换总览
来源：http://ff.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bx.szsharing.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nz.lnxyls.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lx.panjiajie.cn

TS:   Number() String() Boolean() x as number
来源：http://hb.asd995.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fs.hahajie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ou.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rm.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hp.jianghongdianzi.cn

================================================================================
来源：http://rk.huanxung.cn

B. 流程控制
来源：http://mw.panjiajie.cn

================================================================================
来源：http://bh.szsharing.cn

[B01] 条件判断 if / else
来源：http://aa.asd995.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mz.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dg.shtwfgs.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ag.asd995.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uu.huixiangedu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://aq.jctech888.com.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gw.nicolike.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lh.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ut.yuntaijiaju.cn

[B02] 多分支 else if / elif
来源：http://ns.newstarts.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wh.9csxet.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dp.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rl.huanxung.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bz.szxytkj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dn.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qs.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ov.asd995.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ud.muxihuayi.cn

[B03] switch / match / case
来源：http://uh.huanxung.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wr.hnjuh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qz.szxytkj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://od.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lr.bookmarksfly.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qm.haigaiapp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gt.jianghongdianzi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ii.nicolike.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qb.hahajie.cn

[B04] for 计数循环
来源：http://vn.chemitech.net.cn

Py:   for i in range(10): print(i)
来源：http://gc.muxihuayi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zw.chemitech.net.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ja.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jj.jctech888.com.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hy.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nf.nicolike.cn

Ruby: 10.times { |i| puts i }
来源：http://op.asd995.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nn.wgjwhj.cn

[B05] 遍历数组 / 列表
来源：http://jq.nszjky.cn

Py:   for item in arr: print(item)
来源：http://lq.szxytkj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zc.newstarts.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pg.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fc.muxihuayi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xy.shxzskj.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ru.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://wv.asd995.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jp.newstarts.cn

[B06] 遍历字典 / 对象
来源：http://ez.szxytkj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xa.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xq.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kk.szxytkj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wq.huanxung.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tf.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lw.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ly.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xd.szxytkj.cn

[B07] while 循环
来源：http://cc.huixinmuqiang.cn

Py:   while i < 10: i += 1
来源：http://jv.shxzskj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://di.huanxung.cn

JS:   while (i < 10) { i++; }
来源：http://pu.colortex.cn

TS:   while (i < 10) { i++; }
来源：http://cr.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://un.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uy.huixinmuqiang.cn

Ruby: while i < 10; i += 1; end
来源：http://vh.szxytkj.cn

C#:   while (i < 10) { i++; }
来源：http://sg.jianghongdianzi.cn

[B08] do-while（至少执行一次）
来源：http://fo.jianghongdianzi.cn

Py:   # 无 do-while：用 while True + break
来源：http://st.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nl.9csxet.cn

JS:   do { i++; } while (i < 10);
来源：http://aq.panjiajie.cn

TS:   do { i++; } while (i < 10);
来源：http://tp.521024.cn

Java: do { i++; } while (i < 10);
来源：http://mu.shxzukj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ii.nszjky.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dk.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://sr.huanxung.cn

[B09] break 与 continue
来源：http://sc.9csxet.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dx.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zo.hahajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ly.colortex.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://en.hahajie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kq.huanxung.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eu.chemitech.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tx.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tr.huixiangedu.cn

[B10] 遍历同时拿索引
来源：http://ds.yuexingan06.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gh.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lc.panjiajie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uf.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ao.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sx.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gj.hahajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yh.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ph.shtwfgs.cn

[B11] 生成数字序列 / 区间
来源：http://ha.yuexingan06.cn

Py:   list(range(0, 10, 2))
来源：http://fq.asd995.cn

PHP:  range(0, 10, 2);
来源：http://jf.huixiangedu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wa.asd995.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ry.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ce.shxzskj.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://er.yuexingan06.cn

Ruby: (0...10).step(2).to_a
来源：http://qs.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lf.colortex.cn

[B12] 跳出多层循环
来源：http://lw.yuexingan06.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xr.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bd.gzmigu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ow.haigaiapp.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uj.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wr.bjjhwx.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wk.hahajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ht.nszjky.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wx.521024.cn

[B13] 判断是否为数字
来源：http://rs.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://hu.nicolike.cn

PHP:  is_numeric($x)
来源：http://ft.nicolike.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ij.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wz.hnjuh.cn

Java: x instanceof Number
来源：http://km.panjiajie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sv.shtwfgs.cn

Ruby: x.is_a?(Numeric)
来源：http://xl.hnjuh.cn

C#:   x is int or double or decimal
来源：http://it.9csxet.cn

[B14] 判断值是否在集合内
来源：http://pi.nicolike.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cu.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dh.newstarts.cn

JS:   [1, 2, 3].includes(x)
来源：http://pd.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://wu.muxihuayi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ng.521024.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tq.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://eu.521024.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pq.szxytkj.cn

[B15] 布尔运算与取反
来源：http://ox.newstarts.cn

Py:   a and b or not c
来源：http://da.lnxyls.cn

PHP:  $a && $b || !$c
来源：http://tu.newstarts.cn

JS:   a && b || !c
来源：http://ew.bjjhwx.cn

TS:   a && b || !c
来源：http://hw.yuexingan06.cn

Java: a && b || !c
来源：http://ha.521024.cn


<!-- 参考信息 -->