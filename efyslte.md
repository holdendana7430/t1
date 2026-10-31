代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mj.yuexingan06.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hj.wgjwhj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rf.nicolike.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://at.lnxyls.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jj.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ta.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wq.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://cj.huixiangedu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nu.shxzskj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kb.yuntaijiaju.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gt.yuntaijiaju.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yc.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qu.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ql.asd995.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wd.jianghongdianzi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ef.szsharing.cn

[A10] 生成随机数
来源：http://ya.521024.cn

Py:   import random; random.randint(1, 100)
来源：http://fc.shxzukj.cn

PHP:  random_int(1, 100);
来源：http://gu.hnjuh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dn.jianghongdianzi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lx.lnxyls.cn

Java: new Random().nextInt(100) + 1
来源：http://bp.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cs.huanxung.cn

Ruby: rand(1..100)
来源：http://wt.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://eh.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://dv.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://zy.szxytkj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ze.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ld.chemitech.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ay.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://ly.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zx.jctech888.com.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tv.nszjky.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cs.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://ke.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qy.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rf.shtwfgs.cn

JS:   `Hello, ${name}!`
来源：http://oq.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://wx.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://wf.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sy.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://ax.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://lm.muxihuayi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jy.hahajie.cn

Py:   "第一行\n第二行"
来源：http://tp.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://ja.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://gh.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://mb.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://ud.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://oc.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://db.hnjuh.cn

C#:   "第一行\n第二行"
来源：http://fb.521024.cn

[A14] 注释写法
来源：http://jq.gzmigu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ww.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ac.panjiajie.cn

JS:   // 单行；/* 多行 */
来源：http://fy.shxzskj.cn

TS:   // 单行；/* 多行 */
来源：http://vk.huixiangedu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ws.haigaiapp.cn

Go:   // 单行；/* 多行 */
来源：http://vf.lnxyls.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rw.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://fv.hnjuh.cn

[A15] 空值判断与默认值
来源：http://zq.panjiajie.cn

Py:   value = data or "默认值"
来源：http://pg.asd995.cn

PHP:  $value = $data ?? "默认值";
来源：http://cd.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://ee.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://pv.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ux.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://ow.panjiajie.cn

Ruby: value = data || "默认值"
来源：http://th.gzmigu.cn

C#:   var value = data ?? "默认值";
来源：http://vo.9csxet.cn

[A16] 真假值判断规则
来源：http://wl.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mk.hnjuh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lh.szsharing.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://np.hahajie.cn

TS:   if (!x) {}
来源：http://qw.hnjuh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gn.szsharing.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nv.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pl.hnjuh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hx.shxzskj.cn

[A17] 位运算
来源：http://mc.jianghongdianzi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://se.jctech888.com.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uu.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qv.huanxung.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rg.panjiajie.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ab.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mf.huixinmuqiang.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tb.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tf.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://cg.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://tb.wgjwhj.cn

PHP:  ord("A"); chr(65)
来源：http://tz.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ur.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zl.bjjhwx.cn

Java: (int) 'A'; (char) 65
来源：http://hg.bjjhwx.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rm.yuntaijiaju.cn

Ruby: "A".ord; 65.chr
来源：http://ek.szsharing.cn

C#:   (int)'A'; (char)65
来源：http://ed.szsharing.cn

[A19] 交换两个变量
来源：http://ed.huixinmuqiang.cn

Py:   a, b = b, a
来源：http://mw.9csxet.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qi.colortex.cn

JS:   [a, b] = [b, a];
来源：http://gb.newstarts.cn

TS:   [a, b] = [b, a];
来源：http://ty.hahajie.cn

Java: int t = a; a = b; b = t;
来源：http://vs.huixiangedu.cn

Go:   a, b = b, a
来源：http://av.shtwfgs.cn

Ruby: a, b = b, a
来源：http://fn.szxytkj.cn

C#:   (a, b) = (b, a);
来源：http://dp.bjjhwx.cn

[A20] 读取标准输入
来源：http://oc.gzmigu.cn

Py:   name = input("请输入：")
来源：http://xj.asd995.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ux.shxzskj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uo.haigaiapp.cn

TS:   // Node.js：readline 模块
来源：http://rr.yuexingan06.cn

Java: new Scanner(System.in).nextLine()
来源：http://zw.asd995.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zo.hnjuh.cn

Ruby: gets.chomp
来源：http://ff.yuexingan06.cn

C#:   Console.ReadLine();
来源：http://gc.huanxung.cn

[A21] 保留指定小数位输出
来源：http://ox.jianghongdianzi.cn

Py:   f"{3.14159:.2f}"
来源：http://ou.szsharing.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jw.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://wn.huixiangedu.cn

TS:   (3.14159).toFixed(2)
来源：http://gh.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://nd.haigaiapp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zi.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://sq.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://dq.hahajie.cn

[A22] 获取字符串长度
来源：http://sx.yuntaijiaju.cn

Py:   len(s)
来源：http://oh.chemitech.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tq.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vo.huanxung.cn

TS:   s.length
来源：http://os.wgjwhj.cn

Java: s.length()
来源：http://ia.lnxyls.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jd.chemitech.net.cn

Ruby: s.length
来源：http://pr.shxzskj.cn

C#:   s.Length
来源：http://df.panjiajie.cn

[A23] 大小写转换
来源：http://vz.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ie.9csxet.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rj.asd995.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://md.newstarts.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ho.haigaiapp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gz.yuntaijiaju.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xq.521024.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sy.shxzskj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://id.newstarts.cn

[A24] 去除首尾空白
来源：http://zm.jianghongdianzi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ra.newstarts.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kz.yuexingan06.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ri.9csxet.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ku.newstarts.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kh.lnxyls.cn

Go:   strings.TrimSpace(s)
来源：http://hx.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nc.haigaiapp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sg.newstarts.cn

[A25] 字符串比较
来源：http://tk.haigaiapp.cn

Py:   s1 == s2; s1 != s2
来源：http://fm.wgjwhj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gs.chemitech.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gh.jctech888.com.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://py.lnxyls.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jz.gzmigu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dm.yuntaijiaju.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xo.shxzskj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gb.shtwfgs.cn

[A26] 类型转换总览
来源：http://se.jctech888.com.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://in.haigaiapp.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lm.jianghongdianzi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uo.yuexingan06.cn

TS:   Number() String() Boolean() x as number
来源：http://ec.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vb.521024.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://li.huanxung.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://aa.lnxyls.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pd.shxzukj.cn

================================================================================
来源：http://so.huanxung.cn

B. 流程控制
来源：http://ap.huixinmuqiang.cn

================================================================================
来源：http://fl.huanxung.cn

[B01] 条件判断 if / else
来源：http://jh.huanxung.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ar.hnjuh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sx.gzmigu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://id.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xy.521024.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gt.lnxyls.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pz.szsharing.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bs.lnxyls.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zr.huixiangedu.cn

[B02] 多分支 else if / elif
来源：http://ay.colortex.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xp.jianghongdianzi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lr.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wh.nszjky.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nx.jianghongdianzi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ut.nszjky.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ab.szxytkj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://er.yuntaijiaju.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bp.szxytkj.cn

[B03] switch / match / case
来源：http://hd.bookmarksfly.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://af.newstarts.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gr.hnjuh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cu.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ln.newstarts.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dr.shxzukj.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oq.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kz.szsharing.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://do.panjiajie.cn

[B04] for 计数循环
来源：http://xb.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://le.yuntaijiaju.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hc.hnjuh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dm.hahajie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sp.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pe.huixiangedu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ze.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://zj.yuntaijiaju.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wq.huixinmuqiang.cn

[B05] 遍历数组 / 列表
来源：http://ro.asd995.cn

Py:   for item in arr: print(item)
来源：http://lq.hahajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lo.yuexingan06.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tr.gzmigu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://az.huixiangedu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gm.nicolike.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vw.nicolike.cn

Ruby: arr.each { |item| puts item }
来源：http://zv.muxihuayi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sn.haigaiapp.cn

[B06] 遍历字典 / 对象
来源：http://ug.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://nd.hahajie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wh.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xp.jianghongdianzi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ii.jianghongdianzi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fq.huanxung.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jj.colortex.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://si.shxzukj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://th.muxihuayi.cn

[B07] while 循环
来源：http://fw.nszjky.cn

Py:   while i < 10: i += 1
来源：http://cu.huixiangedu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fh.asd995.cn

JS:   while (i < 10) { i++; }
来源：http://eh.bookmarksfly.cn

TS:   while (i < 10) { i++; }
来源：http://em.nicolike.cn

Java: while (i < 10) { i++; }
来源：http://px.chemitech.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sb.newstarts.cn

Ruby: while i < 10; i += 1; end
来源：http://oj.yuntaijiaju.cn

C#:   while (i < 10) { i++; }
来源：http://wq.newstarts.cn

[B08] do-while（至少执行一次）
来源：http://on.nszjky.cn

Py:   # 无 do-while：用 while True + break
来源：http://ci.gzmigu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sk.huixiangedu.cn

JS:   do { i++; } while (i < 10);
来源：http://ni.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://qx.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://ca.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vz.huanxung.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vb.nicolike.cn

C#:   do { i++; } while (i < 10);
来源：http://ll.chemitech.net.cn

[B09] break 与 continue
来源：http://bu.asd995.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://na.shxzukj.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mn.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://su.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ob.nicolike.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ja.hnjuh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wm.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://po.huanxung.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eu.lnxyls.cn

[B10] 遍历同时拿索引
来源：http://cp.521024.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wn.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cz.nicolike.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://da.yuexingan06.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://st.hahajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fq.huixinmuqiang.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oj.yuntaijiaju.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kn.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cc.bookmarksfly.cn

[B11] 生成数字序列 / 区间
来源：http://qo.521024.cn

Py:   list(range(0, 10, 2))
来源：http://lu.shxzukj.cn

PHP:  range(0, 10, 2);
来源：http://vr.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://le.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oc.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yg.bookmarksfly.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gx.jctech888.com.cn

Ruby: (0...10).step(2).to_a
来源：http://un.asd995.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mu.panjiajie.cn

[B12] 跳出多层循环
来源：http://zl.colortex.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ca.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ny.521024.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bf.521024.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rq.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nj.colortex.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yx.huixinmuqiang.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ki.shtwfgs.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ht.shxzskj.cn

[B13] 判断是否为数字
来源：http://xt.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://ip.lnxyls.cn

PHP:  is_numeric($x)
来源：http://il.asd995.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fn.jianghongdianzi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yg.shxzukj.cn

Java: x instanceof Number
来源：http://sh.9csxet.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lf.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://ok.colortex.cn

C#:   x is int or double or decimal
来源：http://rs.panjiajie.cn

[B14] 判断值是否在集合内
来源：http://yl.jctech888.com.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wv.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zj.bjjhwx.cn

JS:   [1, 2, 3].includes(x)
来源：http://gy.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://go.colortex.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fm.bookmarksfly.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rn.lnxyls.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vu.shtwfgs.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hh.shtwfgs.cn

[B15] 布尔运算与取反
来源：http://py.lnxyls.cn

Py:   a and b or not c
来源：http://so.hahajie.cn


<!-- 参考信息 -->