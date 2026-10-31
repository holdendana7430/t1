代发 wailian999

Java: 7 / 2; 7 % 2
来源：http://sj.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://ss.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://rv.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://ns.wgjwhj.cn

[A06] 字符串转数字
来源：http://ch.panjiajie.cn

Py:   int("42"); float("3.14")
来源：http://ia.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gm.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://iv.szsharing.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ic.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ox.yuntaijiaju.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lj.colortex.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://yy.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zs.newstarts.cn

[A07] 数字转字符串
来源：http://fd.bookmarksfly.cn

Py:   str(42)
来源：http://py.panjiajie.cn

PHP:  (string) 42; strval(42)
来源：http://eb.haigaiapp.cn

JS:   String(42); (42).toString()
来源：http://zf.9csxet.cn

TS:   String(42)
来源：http://tp.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xx.chemitech.net.cn

Go:   strconv.Itoa(42)
来源：http://wp.colortex.cn

Ruby: 42.to_s
来源：http://vl.huixinmuqiang.cn

C#:   42.ToString()
来源：http://kx.hahajie.cn

[A08] 取整与四舍五入
来源：http://pj.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lz.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mv.hnjuh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ou.yuntaijiaju.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://si.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://eh.wgjwhj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jj.shtwfgs.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ci.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ua.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://iq.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pp.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ry.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hc.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sn.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ze.bjjhwx.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xt.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uv.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wm.chemitech.net.cn

[A10] 生成随机数
来源：http://kg.huanxung.cn

Py:   import random; random.randint(1, 100)
来源：http://we.chemitech.net.cn

PHP:  random_int(1, 100);
来源：http://em.colortex.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wj.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xh.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://jq.lnxyls.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sx.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://lv.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://hw.9csxet.cn

[A11] 条件表达式（三元）
来源：http://nh.huixiangedu.cn

Py:   "yes" if x > 0 else "no"
来源：http://vn.panjiajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xp.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ii.szsharing.cn

TS:   x > 0 ? "yes" : "no"
来源：http://po.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://if.huixiangedu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pd.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ev.521024.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hi.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://co.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wn.yuexingan06.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jn.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://bs.huanxung.cn

TS:   `Hello, ${name}!`
来源：http://nq.newstarts.cn

Java: "Hello, %s!".formatted(name)
来源：http://cr.panjiajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ma.bookmarksfly.cn

Ruby: "Hello, #{name}!"
来源：http://fz.asd995.cn

C#:   $"Hello, {name}!"
来源：http://fq.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ag.panjiajie.cn

Py:   "第一行\n第二行"
来源：http://kd.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://ch.shxzukj.cn

JS:   "第一行\n第二行"
来源：http://ae.newstarts.cn

TS:   "第一行\n第二行"
来源：http://ud.jianghongdianzi.cn

Java: "第一行\n第二行"
来源：http://dr.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://ve.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://ia.huixiangedu.cn

C#:   "第一行\n第二行"
来源：http://jw.huanxung.cn

[A14] 注释写法
来源：http://rq.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zr.panjiajie.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kx.gzmigu.cn

JS:   // 单行；/* 多行 */
来源：http://sv.huanxung.cn

TS:   // 单行；/* 多行 */
来源：http://dj.szsharing.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xu.yuexingan06.cn

Go:   // 单行；/* 多行 */
来源：http://of.bookmarksfly.cn

Ruby: # 单行；=begin 多行 =end
来源：http://lj.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://lb.521024.cn

[A15] 空值判断与默认值
来源：http://hp.lnxyls.cn

Py:   value = data or "默认值"
来源：http://ky.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://sg.bjjhwx.cn

JS:   const value = data ?? "默认值";
来源：http://px.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://ul.hnjuh.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rd.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://cg.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://ug.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://fy.haigaiapp.cn

[A16] 真假值判断规则
来源：http://ma.shtwfgs.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vw.huixinmuqiang.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ec.jctech888.com.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bp.muxihuayi.cn

TS:   if (!x) {}
来源：http://th.gzmigu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://di.bjjhwx.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ei.hnjuh.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ql.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ml.shxzskj.cn

[A17] 位运算
来源：http://ht.asd995.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dc.hnjuh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ur.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://st.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vf.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lb.nicolike.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nw.bjjhwx.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hu.lnxyls.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iz.hahajie.cn

[A18] 字符与 ASCII 码互转
来源：http://rc.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://aq.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://ew.jctech888.com.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ni.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oz.muxihuayi.cn

Java: (int) 'A'; (char) 65
来源：http://ez.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bz.huixinmuqiang.cn

Ruby: "A".ord; 65.chr
来源：http://qu.jianghongdianzi.cn

C#:   (int)'A'; (char)65
来源：http://um.haigaiapp.cn

[A19] 交换两个变量
来源：http://ll.wgjwhj.cn

Py:   a, b = b, a
来源：http://ee.hnjuh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tb.wgjwhj.cn

JS:   [a, b] = [b, a];
来源：http://ze.asd995.cn

TS:   [a, b] = [b, a];
来源：http://ry.chemitech.net.cn

Java: int t = a; a = b; b = t;
来源：http://ht.shxzskj.cn

Go:   a, b = b, a
来源：http://el.lnxyls.cn

Ruby: a, b = b, a
来源：http://dn.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://hr.jianghongdianzi.cn

[A20] 读取标准输入
来源：http://ue.colortex.cn

Py:   name = input("请输入：")
来源：http://dt.muxihuayi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://jx.szsharing.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://et.shtwfgs.cn

TS:   // Node.js：readline 模块
来源：http://hn.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://ny.hnjuh.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tg.jianghongdianzi.cn

Ruby: gets.chomp
来源：http://ig.szsharing.cn

C#:   Console.ReadLine();
来源：http://qq.wgjwhj.cn

[A21] 保留指定小数位输出
来源：http://fx.yuexingan06.cn

Py:   f"{3.14159:.2f}"
来源：http://xo.hnjuh.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ia.shtwfgs.cn

JS:   (3.14159).toFixed(2)
来源：http://le.colortex.cn

TS:   (3.14159).toFixed(2)
来源：http://yz.shxzskj.cn

Java: String.format("%.2f", 3.14159)
来源：http://cn.huixinmuqiang.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qp.huixinmuqiang.cn

Ruby: format("%.2f", 3.14159)
来源：http://jw.bjjhwx.cn

C#:   3.14159.ToString("F2")
来源：http://nt.huixiangedu.cn

[A22] 获取字符串长度
来源：http://gt.huanxung.cn

Py:   len(s)
来源：http://tw.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uq.lnxyls.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eu.shxzukj.cn

TS:   s.length
来源：http://kp.haigaiapp.cn

Java: s.length()
来源：http://xz.hahajie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sy.huixiangedu.cn

Ruby: s.length
来源：http://lo.shtwfgs.cn

C#:   s.Length
来源：http://tz.muxihuayi.cn

[A23] 大小写转换
来源：http://la.colortex.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fq.shxzskj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vb.huixiangedu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kh.9csxet.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ou.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kv.asd995.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yl.jianghongdianzi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tv.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fg.jctech888.com.cn

[A24] 去除首尾空白
来源：http://qq.shxzukj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xt.yuntaijiaju.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pj.huixinmuqiang.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ik.haigaiapp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wi.lnxyls.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xj.szsharing.cn

Go:   strings.TrimSpace(s)
来源：http://ik.haigaiapp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ar.lnxyls.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ct.jianghongdianzi.cn

[A25] 字符串比较
来源：http://nj.yuexingan06.cn

Py:   s1 == s2; s1 != s2
来源：http://os.jianghongdianzi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qs.wgjwhj.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ff.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hh.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zn.jctech888.com.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ng.colortex.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xh.panjiajie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ev.9csxet.cn

[A26] 类型转换总览
来源：http://qf.wgjwhj.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bs.newstarts.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jf.newstarts.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ex.yuntaijiaju.cn

TS:   Number() String() Boolean() x as number
来源：http://mq.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nq.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tw.521024.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://kt.szxytkj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vi.shxzukj.cn

================================================================================
来源：http://gh.panjiajie.cn

B. 流程控制
来源：http://mk.jctech888.com.cn

================================================================================
来源：http://zm.szxytkj.cn

[B01] 条件判断 if / else
来源：http://xo.jianghongdianzi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tn.panjiajie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ne.huanxung.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yx.shtwfgs.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fv.jctech888.com.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ki.szxytkj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qo.shxzskj.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eo.nicolike.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://su.newstarts.cn

[B02] 多分支 else if / elif
来源：http://rm.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ks.newstarts.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kz.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xy.huixinmuqiang.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ph.shxzukj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rn.9csxet.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fd.chemitech.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ae.panjiajie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ca.chemitech.net.cn

[B03] switch / match / case
来源：http://ni.jctech888.com.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ng.huanxung.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ff.bookmarksfly.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fs.hahajie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cs.wgjwhj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://py.hahajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://na.gzmigu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hy.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pm.haigaiapp.cn

[B04] for 计数循环
来源：http://pt.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://kn.shtwfgs.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://my.yuexingan06.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dg.shxzukj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cz.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ir.muxihuayi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ha.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://bx.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ry.hnjuh.cn

[B05] 遍历数组 / 列表
来源：http://rg.gzmigu.cn

Py:   for item in arr: print(item)
来源：http://jg.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sv.szsharing.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fq.bookmarksfly.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ny.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gv.asd995.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bq.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://dt.colortex.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lz.asd995.cn

[B06] 遍历字典 / 对象
来源：http://hs.muxihuayi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fb.jianghongdianzi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lc.huixinmuqiang.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tk.hnjuh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ju.haigaiapp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pf.wgjwhj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uv.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qt.hnjuh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wp.shxzukj.cn

[B07] while 循环
来源：http://qz.nszjky.cn

Py:   while i < 10: i += 1
来源：http://cz.szsharing.cn

PHP:  while ($i < 10) { $i++; }
来源：http://at.521024.cn

JS:   while (i < 10) { i++; }
来源：http://qg.yuntaijiaju.cn

TS:   while (i < 10) { i++; }
来源：http://nr.asd995.cn

Java: while (i < 10) { i++; }
来源：http://mk.asd995.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ii.jianghongdianzi.cn

Ruby: while i < 10; i += 1; end
来源：http://eq.chemitech.net.cn

C#:   while (i < 10) { i++; }
来源：http://uk.lnxyls.cn

[B08] do-while（至少执行一次）
来源：http://ls.bookmarksfly.cn

Py:   # 无 do-while：用 while True + break
来源：http://fh.huixiangedu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://io.bjjhwx.cn

JS:   do { i++; } while (i < 10);
来源：http://ut.shtwfgs.cn

TS:   do { i++; } while (i < 10);
来源：http://bk.nicolike.cn

Java: do { i++; } while (i < 10);
来源：http://se.shxzskj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mr.wgjwhj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hq.colortex.cn

C#:   do { i++; } while (i < 10);
来源：http://gq.521024.cn

[B09] break 与 continue
来源：http://qp.yuntaijiaju.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hm.521024.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yj.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mf.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pg.bjjhwx.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ul.yuexingan06.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gq.jianghongdianzi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bv.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cm.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://ts.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ie.nicolike.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ib.asd995.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jm.newstarts.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qu.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hj.9csxet.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ti.panjiajie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://de.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lb.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://rh.colortex.cn

Py:   list(range(0, 10, 2))
来源：http://hr.jctech888.com.cn

PHP:  range(0, 10, 2);
来源：http://sy.newstarts.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zt.haigaiapp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qo.lnxyls.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ct.bjjhwx.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ob.huanxung.cn

Ruby: (0...10).step(2).to_a
来源：http://qv.nszjky.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kn.shxzskj.cn

[B12] 跳出多层循环
来源：http://qh.haigaiapp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yf.szsharing.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pl.yuexingan06.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sq.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xh.nicolike.cn


<!-- 参考信息 -->