代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vv.hahajie.cn

[A07] 数字转字符串
来源：http://oc.yuexingan06.cn

Py:   str(42)
来源：http://li.chemitech.net.cn

PHP:  (string) 42; strval(42)
来源：http://qu.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://ev.chemitech.net.cn

TS:   String(42)
来源：http://jl.huanxung.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gr.nszjky.cn

Go:   strconv.Itoa(42)
来源：http://jk.shxzskj.cn

Ruby: 42.to_s
来源：http://wa.wgjwhj.cn

C#:   42.ToString()
来源：http://ee.yuntaijiaju.cn

[A08] 取整与四舍五入
来源：http://uh.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nx.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ec.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cw.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://iv.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ap.colortex.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://sm.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://hf.shtwfgs.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yj.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://yy.shtwfgs.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pz.9csxet.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vt.nicolike.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yw.hnjuh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lo.chemitech.net.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dp.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uu.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ia.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fr.gzmigu.cn

[A10] 生成随机数
来源：http://ix.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://os.chemitech.net.cn

PHP:  random_int(1, 100);
来源：http://yi.lnxyls.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tw.shxzukj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rr.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://qo.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bq.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://mh.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://vf.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://xi.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://iv.gzmigu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lb.nszjky.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xg.nicolike.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dx.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://da.huixiangedu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nj.newstarts.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mp.bjjhwx.cn

C#:   x > 0 ? "yes" : "no"
来源：http://em.bjjhwx.cn

[A12] 字符串插值 / 格式化
来源：http://yy.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ld.shxzskj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nq.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://in.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://ye.shxzskj.cn

Java: "Hello, %s!".formatted(name)
来源：http://pa.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ku.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://np.szsharing.cn

C#:   $"Hello, {name}!"
来源：http://dh.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://et.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://ao.shxzskj.cn

PHP:  "第一行\n第二行"
来源：http://em.9csxet.cn

JS:   "第一行\n第二行"
来源：http://ny.hahajie.cn

TS:   "第一行\n第二行"
来源：http://bv.yuntaijiaju.cn

Java: "第一行\n第二行"
来源：http://qq.haigaiapp.cn

Go:   "第一行\n第二行"
来源：http://ad.bjjhwx.cn

Ruby: "第一行\n第二行"
来源：http://qk.newstarts.cn

C#:   "第一行\n第二行"
来源：http://lf.hnjuh.cn

[A14] 注释写法
来源：http://cj.yuntaijiaju.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hf.gzmigu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mc.szsharing.cn

JS:   // 单行；/* 多行 */
来源：http://nq.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://nb.yuexingan06.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sw.hahajie.cn

Go:   // 单行；/* 多行 */
来源：http://mu.yuntaijiaju.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ok.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://bn.nszjky.cn

[A15] 空值判断与默认值
来源：http://ol.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://xt.bjjhwx.cn

PHP:  $value = $data ?? "默认值";
来源：http://ll.shxzskj.cn

JS:   const value = data ?? "默认值";
来源：http://cy.wgjwhj.cn

TS:   const value = data ?? "默认值";
来源：http://jo.521024.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qd.wgjwhj.cn

Go:   if data == "" { data = "默认值" }
来源：http://rq.huanxung.cn

Ruby: value = data || "默认值"
来源：http://ge.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://nx.jctech888.com.cn

[A16] 真假值判断规则
来源：http://gi.521024.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mw.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fy.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kw.szsharing.cn

TS:   if (!x) {}
来源：http://tf.wgjwhj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://du.521024.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xa.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ve.nszjky.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ro.newstarts.cn

[A17] 位运算
来源：http://ir.yuexingan06.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nc.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zv.muxihuayi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rg.huixinmuqiang.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sh.nicolike.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://si.asd995.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jz.huixiangedu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wh.muxihuayi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kb.nszjky.cn

[A18] 字符与 ASCII 码互转
来源：http://mz.colortex.cn

Py:   ord("A"); chr(65)
来源：http://sp.szsharing.cn

PHP:  ord("A"); chr(65)
来源：http://ba.lnxyls.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iw.muxihuayi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://do.panjiajie.cn

Java: (int) 'A'; (char) 65
来源：http://eo.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ey.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://vi.huixinmuqiang.cn

C#:   (int)'A'; (char)65
来源：http://tl.colortex.cn

[A19] 交换两个变量
来源：http://wu.shtwfgs.cn

Py:   a, b = b, a
来源：http://uk.szsharing.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qd.newstarts.cn

JS:   [a, b] = [b, a];
来源：http://fx.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://se.newstarts.cn

Java: int t = a; a = b; b = t;
来源：http://yd.szxytkj.cn

Go:   a, b = b, a
来源：http://ha.yuexingan06.cn

Ruby: a, b = b, a
来源：http://vl.asd995.cn

C#:   (a, b) = (b, a);
来源：http://es.huixinmuqiang.cn

[A20] 读取标准输入
来源：http://iw.colortex.cn

Py:   name = input("请输入：")
来源：http://fi.bookmarksfly.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://av.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zu.nicolike.cn

TS:   // Node.js：readline 模块
来源：http://pz.szsharing.cn

Java: new Scanner(System.in).nextLine()
来源：http://lf.szsharing.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zk.nicolike.cn

Ruby: gets.chomp
来源：http://gz.szxytkj.cn

C#:   Console.ReadLine();
来源：http://zr.nicolike.cn

[A21] 保留指定小数位输出
来源：http://my.lnxyls.cn

Py:   f"{3.14159:.2f}"
来源：http://lg.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xf.muxihuayi.cn

JS:   (3.14159).toFixed(2)
来源：http://qu.521024.cn

TS:   (3.14159).toFixed(2)
来源：http://jb.szsharing.cn

Java: String.format("%.2f", 3.14159)
来源：http://xu.gzmigu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hr.jianghongdianzi.cn

Ruby: format("%.2f", 3.14159)
来源：http://td.shxzukj.cn

C#:   3.14159.ToString("F2")
来源：http://ki.9csxet.cn

[A22] 获取字符串长度
来源：http://dx.wgjwhj.cn

Py:   len(s)
来源：http://cr.nszjky.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lk.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cj.gzmigu.cn

TS:   s.length
来源：http://pb.521024.cn

Java: s.length()
来源：http://mk.asd995.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ao.huixinmuqiang.cn

Ruby: s.length
来源：http://co.jianghongdianzi.cn

C#:   s.Length
来源：http://td.hnjuh.cn

[A23] 大小写转换
来源：http://jj.hnjuh.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pi.asd995.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://cg.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xn.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lq.nszjky.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ae.shtwfgs.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jy.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nn.colortex.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vt.hahajie.cn

[A24] 去除首尾空白
来源：http://jv.muxihuayi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sh.521024.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://up.panjiajie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ms.lnxyls.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dj.hnjuh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://et.nicolike.cn

Go:   strings.TrimSpace(s)
来源：http://dj.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yy.panjiajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ny.asd995.cn

[A25] 字符串比较
来源：http://ca.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://dj.szxytkj.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dj.yuexingan06.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zc.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jc.panjiajie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://np.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jh.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ls.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bw.bjjhwx.cn

[A26] 类型转换总览
来源：http://lm.9csxet.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fz.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mi.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bb.jianghongdianzi.cn

TS:   Number() String() Boolean() x as number
来源：http://ox.szxytkj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wt.shxzukj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://av.jctech888.com.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qc.shxzukj.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xb.nicolike.cn

================================================================================
来源：http://ue.szxytkj.cn

B. 流程控制
来源：http://kg.bjjhwx.cn

================================================================================
来源：http://xz.asd995.cn

[B01] 条件判断 if / else
来源：http://ja.panjiajie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jx.jctech888.com.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uv.szxytkj.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tj.huixinmuqiang.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lv.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pd.nicolike.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iz.jctech888.com.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qy.wgjwhj.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ie.hahajie.cn

[B02] 多分支 else if / elif
来源：http://fq.bjjhwx.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xj.shtwfgs.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yh.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ns.jianghongdianzi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sd.wgjwhj.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eh.bjjhwx.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qb.huixiangedu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hs.bjjhwx.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kg.9csxet.cn

[B03] switch / match / case
来源：http://ku.jianghongdianzi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zf.szsharing.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://da.nszjky.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fd.huixiangedu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://in.chemitech.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ud.yuexingan06.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://my.asd995.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qy.newstarts.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vb.asd995.cn

[B04] for 计数循环
来源：http://mb.hnjuh.cn

Py:   for i in range(10): print(i)
来源：http://zk.9csxet.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cc.huanxung.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ie.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rc.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xt.huanxung.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rw.muxihuayi.cn

Ruby: 10.times { |i| puts i }
来源：http://hf.muxihuayi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ia.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://kg.asd995.cn

Py:   for item in arr: print(item)
来源：http://se.521024.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wb.huixinmuqiang.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yz.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gz.hahajie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jv.hahajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nr.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://jl.yuntaijiaju.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lf.521024.cn

[B06] 遍历字典 / 对象
来源：http://yb.huanxung.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jp.huixiangedu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yl.haigaiapp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lo.wgjwhj.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xy.9csxet.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tn.yuntaijiaju.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fe.muxihuayi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uo.nszjky.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vv.muxihuayi.cn

[B07] while 循环
来源：http://yp.shxzskj.cn

Py:   while i < 10: i += 1
来源：http://xv.szxytkj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zx.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://mw.jianghongdianzi.cn

TS:   while (i < 10) { i++; }
来源：http://jc.521024.cn

Java: while (i < 10) { i++; }
来源：http://ul.newstarts.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xc.hnjuh.cn

Ruby: while i < 10; i += 1; end
来源：http://zk.nszjky.cn

C#:   while (i < 10) { i++; }
来源：http://lu.bjjhwx.cn

[B08] do-while（至少执行一次）
来源：http://qh.huanxung.cn

Py:   # 无 do-while：用 while True + break
来源：http://li.shxzukj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gj.yuexingan06.cn

JS:   do { i++; } while (i < 10);
来源：http://iu.szsharing.cn

TS:   do { i++; } while (i < 10);
来源：http://bz.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://qv.szxytkj.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vx.521024.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qo.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://cy.bjjhwx.cn

[B09] break 与 continue
来源：http://la.nicolike.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uh.szsharing.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nv.yuexingan06.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iv.szsharing.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://go.jctech888.com.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jw.huixiangedu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vw.haigaiapp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fg.panjiajie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ij.jctech888.com.cn

[B10] 遍历同时拿索引
来源：http://xq.huixinmuqiang.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ra.jianghongdianzi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ds.muxihuayi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gt.nicolike.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xe.shxzskj.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dt.colortex.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fk.hnjuh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xj.shtwfgs.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ix.hahajie.cn

[B11] 生成数字序列 / 区间
来源：http://ov.lnxyls.cn

Py:   list(range(0, 10, 2))
来源：http://vf.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://zn.yuexingan06.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qc.jianghongdianzi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nd.asd995.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xk.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vw.shxzukj.cn

Ruby: (0...10).step(2).to_a
来源：http://wa.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ev.bjjhwx.cn

[B12] 跳出多层循环
来源：http://im.9csxet.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qy.nszjky.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qp.shtwfgs.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vr.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zw.hnjuh.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jz.shxzukj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qf.muxihuayi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cm.lnxyls.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ek.hahajie.cn

[B13] 判断是否为数字
来源：http://pg.szxytkj.cn

Py:   isinstance(x, (int, float))
来源：http://kp.newstarts.cn

PHP:  is_numeric($x)
来源：http://un.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ae.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ec.newstarts.cn

Java: x instanceof Number
来源：http://ki.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hw.521024.cn

Ruby: x.is_a?(Numeric)
来源：http://ym.huixiangedu.cn


<!-- 参考信息 -->