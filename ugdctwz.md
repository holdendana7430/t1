代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hv.shxzukj.cn

Java: new Random().nextInt(100) + 1
来源：http://ah.521024.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bj.shxzukj.cn

Ruby: rand(1..100)
来源：http://rl.yuntaijiaju.cn

C#:   new Random().Next(1, 101)
来源：http://no.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://eh.muxihuayi.cn

Py:   "yes" if x > 0 else "no"
来源：http://uc.szsharing.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ou.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://je.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://of.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://kf.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sz.colortex.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lj.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qo.huixiangedu.cn

[A12] 字符串插值 / 格式化
来源：http://mh.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ng.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sx.szxytkj.cn

JS:   `Hello, ${name}!`
来源：http://cl.huixinmuqiang.cn

TS:   `Hello, ${name}!`
来源：http://yl.asd995.cn

Java: "Hello, %s!".formatted(name)
来源：http://uz.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yp.lnxyls.cn

Ruby: "Hello, #{name}!"
来源：http://yg.bookmarksfly.cn

C#:   $"Hello, {name}!"
来源：http://rs.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vl.9csxet.cn

Py:   "第一行\n第二行"
来源：http://on.gzmigu.cn

PHP:  "第一行\n第二行"
来源：http://xh.wgjwhj.cn

JS:   "第一行\n第二行"
来源：http://dn.szsharing.cn

TS:   "第一行\n第二行"
来源：http://kx.szsharing.cn

Java: "第一行\n第二行"
来源：http://ug.bookmarksfly.cn

Go:   "第一行\n第二行"
来源：http://eh.huixinmuqiang.cn

Ruby: "第一行\n第二行"
来源：http://gy.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://qo.yuntaijiaju.cn

[A14] 注释写法
来源：http://pu.haigaiapp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mq.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dw.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://zn.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://jj.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rt.nicolike.cn

Go:   // 单行；/* 多行 */
来源：http://wi.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ok.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://kg.jctech888.com.cn

[A15] 空值判断与默认值
来源：http://wm.huixiangedu.cn

Py:   value = data or "默认值"
来源：http://uy.9csxet.cn

PHP:  $value = $data ?? "默认值";
来源：http://wa.jctech888.com.cn

JS:   const value = data ?? "默认值";
来源：http://fh.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://vp.asd995.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rp.shxzukj.cn

Go:   if data == "" { data = "默认值" }
来源：http://fa.szsharing.cn

Ruby: value = data || "默认值"
来源：http://nb.panjiajie.cn

C#:   var value = data ?? "默认值";
来源：http://vo.521024.cn

[A16] 真假值判断规则
来源：http://ry.bjjhwx.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kg.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jo.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wx.haigaiapp.cn

TS:   if (!x) {}
来源：http://hk.haigaiapp.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xy.muxihuayi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ix.yuexingan06.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fh.panjiajie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cl.shtwfgs.cn

[A17] 位运算
来源：http://ul.huixiangedu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oi.bookmarksfly.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vn.colortex.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yr.bookmarksfly.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vo.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cp.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://je.wgjwhj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ok.panjiajie.cn

[A18] 字符与 ASCII 码互转
来源：http://cq.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://nu.shxzukj.cn

PHP:  ord("A"); chr(65)
来源：http://zm.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hk.gzmigu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wg.asd995.cn

Java: (int) 'A'; (char) 65
来源：http://qk.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fq.nszjky.cn

Ruby: "A".ord; 65.chr
来源：http://yn.nszjky.cn

C#:   (int)'A'; (char)65
来源：http://jz.shxzskj.cn

[A19] 交换两个变量
来源：http://mm.chemitech.net.cn

Py:   a, b = b, a
来源：http://me.nszjky.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hp.huixinmuqiang.cn

JS:   [a, b] = [b, a];
来源：http://sd.shxzukj.cn

TS:   [a, b] = [b, a];
来源：http://gn.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://ej.haigaiapp.cn

Go:   a, b = b, a
来源：http://cu.hnjuh.cn

Ruby: a, b = b, a
来源：http://xn.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://vd.bjjhwx.cn

[A20] 读取标准输入
来源：http://ni.9csxet.cn

Py:   name = input("请输入：")
来源：http://ju.hahajie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://so.panjiajie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tp.yuexingan06.cn

TS:   // Node.js：readline 模块
来源：http://aa.521024.cn

Java: new Scanner(System.in).nextLine()
来源：http://te.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nl.newstarts.cn

Ruby: gets.chomp
来源：http://tw.wgjwhj.cn

C#:   Console.ReadLine();
来源：http://yn.jctech888.com.cn

[A21] 保留指定小数位输出
来源：http://qf.panjiajie.cn

Py:   f"{3.14159:.2f}"
来源：http://ml.shxzukj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ym.newstarts.cn

JS:   (3.14159).toFixed(2)
来源：http://un.wgjwhj.cn

TS:   (3.14159).toFixed(2)
来源：http://rc.bjjhwx.cn

Java: String.format("%.2f", 3.14159)
来源：http://fe.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cc.521024.cn

Ruby: format("%.2f", 3.14159)
来源：http://cz.jctech888.com.cn

C#:   3.14159.ToString("F2")
来源：http://vc.chemitech.net.cn

[A22] 获取字符串长度
来源：http://jq.hahajie.cn

Py:   len(s)
来源：http://fd.colortex.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zm.yuexingan06.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://am.panjiajie.cn

TS:   s.length
来源：http://dw.newstarts.cn

Java: s.length()
来源：http://zl.shxzskj.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ii.shxzskj.cn

Ruby: s.length
来源：http://yt.shxzskj.cn

C#:   s.Length
来源：http://ow.yuexingan06.cn

[A23] 大小写转换
来源：http://ql.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ci.yuntaijiaju.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pf.9csxet.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zd.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ep.bookmarksfly.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tg.newstarts.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://af.shxzskj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ec.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bg.haigaiapp.cn

[A24] 去除首尾空白
来源：http://tr.szsharing.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kr.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ey.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nv.hahajie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cm.9csxet.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://so.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://uf.shtwfgs.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nf.hahajie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mf.haigaiapp.cn

[A25] 字符串比较
来源：http://sh.hnjuh.cn

Py:   s1 == s2; s1 != s2
来源：http://io.521024.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iv.lnxyls.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yx.yuexingan06.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jh.bookmarksfly.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wo.nicolike.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bh.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wn.szxytkj.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://de.nszjky.cn

[A26] 类型转换总览
来源：http://tk.bjjhwx.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sq.bjjhwx.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hy.hahajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eb.colortex.cn

TS:   Number() String() Boolean() x as number
来源：http://sn.bookmarksfly.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rp.wgjwhj.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yb.chemitech.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vk.nicolike.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nj.lnxyls.cn

================================================================================
来源：http://rn.panjiajie.cn

B. 流程控制
来源：http://rr.haigaiapp.cn

================================================================================
来源：http://fc.hnjuh.cn

[B01] 条件判断 if / else
来源：http://gd.521024.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ze.szxytkj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rz.haigaiapp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tv.huixiangedu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bu.shtwfgs.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wr.shxzskj.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ai.panjiajie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uv.jianghongdianzi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ad.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://vz.huixinmuqiang.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hj.chemitech.net.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://an.yuexingan06.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pe.lnxyls.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yu.haigaiapp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yl.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hn.panjiajie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fj.huixinmuqiang.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mi.szsharing.cn

[B03] switch / match / case
来源：http://kv.haigaiapp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://re.shxzukj.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ee.yuntaijiaju.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ei.yuntaijiaju.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ws.nszjky.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ok.huanxung.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pn.shxzukj.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uq.jianghongdianzi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ku.haigaiapp.cn

[B04] for 计数循环
来源：http://uk.hahajie.cn

Py:   for i in range(10): print(i)
来源：http://ia.szxytkj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ip.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://we.nszjky.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rn.nszjky.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kf.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ji.huanxung.cn

Ruby: 10.times { |i| puts i }
来源：http://yq.bjjhwx.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hv.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://ct.jctech888.com.cn

Py:   for item in arr: print(item)
来源：http://io.lnxyls.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zw.9csxet.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dj.jctech888.com.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ju.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jy.huixiangedu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cu.asd995.cn

Ruby: arr.each { |item| puts item }
来源：http://rt.huixiangedu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ob.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://rg.gzmigu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ya.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tt.asd995.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://js.lnxyls.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zw.shxzskj.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://df.gzmigu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://og.newstarts.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ip.huixiangedu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gr.lnxyls.cn

[B07] while 循环
来源：http://km.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://ch.yuexingan06.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uo.szsharing.cn

JS:   while (i < 10) { i++; }
来源：http://af.shxzskj.cn

TS:   while (i < 10) { i++; }
来源：http://kz.muxihuayi.cn

Java: while (i < 10) { i++; }
来源：http://ja.szxytkj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kq.shxzskj.cn

Ruby: while i < 10; i += 1; end
来源：http://wi.huanxung.cn

C#:   while (i < 10) { i++; }
来源：http://mq.bookmarksfly.cn

[B08] do-while（至少执行一次）
来源：http://ke.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://tp.bjjhwx.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nb.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://eg.huanxung.cn

TS:   do { i++; } while (i < 10);
来源：http://bs.nszjky.cn

Java: do { i++; } while (i < 10);
来源：http://ae.yuntaijiaju.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hk.nicolike.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rm.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://ni.bjjhwx.cn

[B09] break 与 continue
来源：http://gi.newstarts.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gj.huixiangedu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://if.lnxyls.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aj.nszjky.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fh.muxihuayi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cn.lnxyls.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pd.nicolike.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kp.shtwfgs.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pj.newstarts.cn

[B10] 遍历同时拿索引
来源：http://dq.wgjwhj.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qz.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vr.szsharing.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mz.wgjwhj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yf.lnxyls.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ie.jctech888.com.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sx.chemitech.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jf.nicolike.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nr.bjjhwx.cn

[B11] 生成数字序列 / 区间
来源：http://kl.jctech888.com.cn

Py:   list(range(0, 10, 2))
来源：http://dm.asd995.cn

PHP:  range(0, 10, 2);
来源：http://nj.huixinmuqiang.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tc.9csxet.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qz.bjjhwx.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ru.hnjuh.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wd.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://xo.jianghongdianzi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zl.yuntaijiaju.cn

[B12] 跳出多层循环
来源：http://td.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ut.nicolike.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://un.chemitech.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hf.bjjhwx.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nx.nszjky.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nr.huixinmuqiang.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bf.panjiajie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rf.szxytkj.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ew.huixiangedu.cn

[B13] 判断是否为数字
来源：http://cz.nicolike.cn

Py:   isinstance(x, (int, float))
来源：http://ep.chemitech.net.cn

PHP:  is_numeric($x)
来源：http://qx.yuexingan06.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wf.muxihuayi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mu.nicolike.cn

Java: x instanceof Number
来源：http://ti.huixiangedu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://el.szxytkj.cn

Ruby: x.is_a?(Numeric)
来源：http://mk.panjiajie.cn

C#:   x is int or double or decimal
来源：http://cv.muxihuayi.cn

[B14] 判断值是否在集合内
来源：http://be.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aj.bjjhwx.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zd.9csxet.cn

JS:   [1, 2, 3].includes(x)
来源：http://tx.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://np.jianghongdianzi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://in.huixiangedu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fn.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zw.shxzukj.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yn.shxzskj.cn

[B15] 布尔运算与取反
来源：http://gc.nicolike.cn

Py:   a and b or not c
来源：http://cj.szsharing.cn

PHP:  $a && $b || !$c
来源：http://yx.shtwfgs.cn

JS:   a && b || !c
来源：http://fm.hahajie.cn

TS:   a && b || !c
来源：http://pt.shxzukj.cn

Java: a && b || !c
来源：http://lv.szsharing.cn

Go:   a && b || !c
来源：http://rz.huixiangedu.cn

Ruby: a && b || !c
来源：http://vf.huanxung.cn

C#:   a && b || !c
来源：http://bv.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vm.chemitech.net.cn

Py:   if not data: return
来源：http://qu.newstarts.cn

PHP:  if (!$data) { return; }
来源：http://un.521024.cn

JS:   if (!data) return;
来源：http://pt.yuntaijiaju.cn

TS:   if (!data) return;
来源：http://ov.gzmigu.cn

Java: if (data == null) return;
来源：http://qv.yuexingan06.cn

Go:   if data == nil { return }
来源：http://os.yuexingan06.cn

Ruby: return if data.nil?
来源：http://dq.muxihuayi.cn

C#:   if (data == null) return;
来源：http://mo.newstarts.cn

================================================================================
来源：http://lv.9csxet.cn

C. 函数与作用域
来源：http://jq.521024.cn

================================================================================
来源：http://lr.jctech888.com.cn

[C01] 定义函数
来源：http://of.huixiangedu.cn


<!-- 参考信息 -->