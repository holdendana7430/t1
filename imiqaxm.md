代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://aq.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://tu.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dv.hnjuh.cn

Ruby: rand(1..100)
来源：http://xv.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://wm.nicolike.cn

[A11] 条件表达式（三元）
来源：http://be.bjjhwx.cn

Py:   "yes" if x > 0 else "no"
来源：http://ft.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gr.panjiajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://be.9csxet.cn

TS:   x > 0 ? "yes" : "no"
来源：http://na.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://ri.jctech888.com.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hp.521024.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wr.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://hb.jianghongdianzi.cn

[A12] 字符串插值 / 格式化
来源：http://ep.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cr.9csxet.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uf.bookmarksfly.cn

JS:   `Hello, ${name}!`
来源：http://nm.521024.cn

TS:   `Hello, ${name}!`
来源：http://xo.nszjky.cn

Java: "Hello, %s!".formatted(name)
来源：http://nn.wgjwhj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ks.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://dy.gzmigu.cn

C#:   $"Hello, {name}!"
来源：http://ci.chemitech.net.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ap.9csxet.cn

Py:   "第一行\n第二行"
来源：http://dp.huanxung.cn

PHP:  "第一行\n第二行"
来源：http://fd.shtwfgs.cn

JS:   "第一行\n第二行"
来源：http://yz.muxihuayi.cn

TS:   "第一行\n第二行"
来源：http://kv.521024.cn

Java: "第一行\n第二行"
来源：http://kq.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://sv.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://bp.nszjky.cn

C#:   "第一行\n第二行"
来源：http://kz.huixinmuqiang.cn

[A14] 注释写法
来源：http://jj.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kn.huanxung.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dg.chemitech.net.cn

JS:   // 单行；/* 多行 */
来源：http://ac.521024.cn

TS:   // 单行；/* 多行 */
来源：http://qv.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ig.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://tn.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ku.shtwfgs.cn

C#:   // 单行；/* 多行 */
来源：http://zv.hahajie.cn

[A15] 空值判断与默认值
来源：http://js.shxzskj.cn

Py:   value = data or "默认值"
来源：http://oz.521024.cn

PHP:  $value = $data ?? "默认值";
来源：http://fq.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://yz.nszjky.cn

TS:   const value = data ?? "默认值";
来源：http://lu.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://en.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://kv.newstarts.cn

Ruby: value = data || "默认值"
来源：http://ui.hahajie.cn

C#:   var value = data ?? "默认值";
来源：http://ls.lnxyls.cn

[A16] 真假值判断规则
来源：http://hz.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xa.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lh.gzmigu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hr.gzmigu.cn

TS:   if (!x) {}
来源：http://nf.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mr.huixiangedu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ab.521024.cn

Ruby: unless x            # nil 与 false 为假
来源：http://in.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://do.asd995.cn

[A17] 位运算
来源：http://rw.nszjky.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ez.szsharing.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://od.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ub.521024.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ic.huixiangedu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://es.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mh.szxytkj.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cb.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bd.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://an.shtwfgs.cn

Py:   ord("A"); chr(65)
来源：http://ne.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://uw.yuexingan06.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hf.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oi.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://ha.gzmigu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://go.9csxet.cn

Ruby: "A".ord; 65.chr
来源：http://nc.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://ny.bjjhwx.cn

[A19] 交换两个变量
来源：http://kj.hahajie.cn

Py:   a, b = b, a
来源：http://ob.huanxung.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ov.jctech888.com.cn

JS:   [a, b] = [b, a];
来源：http://pk.asd995.cn

TS:   [a, b] = [b, a];
来源：http://vh.huixinmuqiang.cn

Java: int t = a; a = b; b = t;
来源：http://ny.chemitech.net.cn

Go:   a, b = b, a
来源：http://ng.newstarts.cn

Ruby: a, b = b, a
来源：http://ap.9csxet.cn

C#:   (a, b) = (b, a);
来源：http://tz.colortex.cn

[A20] 读取标准输入
来源：http://yk.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://wn.nicolike.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://da.huixiangedu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zf.szxytkj.cn

TS:   // Node.js：readline 模块
来源：http://sd.muxihuayi.cn

Java: new Scanner(System.in).nextLine()
来源：http://wv.bjjhwx.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sb.newstarts.cn

Ruby: gets.chomp
来源：http://vm.lnxyls.cn

C#:   Console.ReadLine();
来源：http://tp.shxzskj.cn

[A21] 保留指定小数位输出
来源：http://dl.szxytkj.cn

Py:   f"{3.14159:.2f}"
来源：http://vt.huixiangedu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oz.wgjwhj.cn

JS:   (3.14159).toFixed(2)
来源：http://wd.lnxyls.cn

TS:   (3.14159).toFixed(2)
来源：http://nr.hnjuh.cn

Java: String.format("%.2f", 3.14159)
来源：http://td.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xn.nszjky.cn

Ruby: format("%.2f", 3.14159)
来源：http://xe.shtwfgs.cn

C#:   3.14159.ToString("F2")
来源：http://zr.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://rl.hahajie.cn

Py:   len(s)
来源：http://jz.jianghongdianzi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tj.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gt.bookmarksfly.cn

TS:   s.length
来源：http://uw.asd995.cn

Java: s.length()
来源：http://ly.chemitech.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://im.newstarts.cn

Ruby: s.length
来源：http://xo.huixiangedu.cn

C#:   s.Length
来源：http://mm.huanxung.cn

[A23] 大小写转换
来源：http://fs.haigaiapp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fj.szsharing.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yn.huanxung.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nj.jctech888.com.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jg.hnjuh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zw.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dr.muxihuayi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://to.nicolike.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://xw.newstarts.cn

[A24] 去除首尾空白
来源：http://bw.huixiangedu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://do.jctech888.com.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mr.shxzskj.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bh.szsharing.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ee.bookmarksfly.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://su.shtwfgs.cn

Go:   strings.TrimSpace(s)
来源：http://sx.szxytkj.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ai.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ur.yuntaijiaju.cn

[A25] 字符串比较
来源：http://wb.lnxyls.cn

Py:   s1 == s2; s1 != s2
来源：http://li.jctech888.com.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ex.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sk.yuntaijiaju.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cz.colortex.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hm.wgjwhj.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uv.huixinmuqiang.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nn.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rw.panjiajie.cn

[A26] 类型转换总览
来源：http://kg.panjiajie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dj.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://la.521024.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kv.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://pj.shxzskj.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xk.chemitech.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://am.muxihuayi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ii.yuexingan06.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gg.chemitech.net.cn

================================================================================
来源：http://ce.bjjhwx.cn

B. 流程控制
来源：http://ik.hahajie.cn

================================================================================
来源：http://po.hahajie.cn

[B01] 条件判断 if / else
来源：http://vg.chemitech.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wu.colortex.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jj.yuexingan06.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jq.haigaiapp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mo.chemitech.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ie.szsharing.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nx.bjjhwx.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wt.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mz.bookmarksfly.cn

[B02] 多分支 else if / elif
来源：http://np.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yy.asd995.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rj.bookmarksfly.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jy.asd995.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jr.colortex.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ek.chemitech.net.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hl.muxihuayi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ue.shxzskj.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cd.colortex.cn

[B03] switch / match / case
来源：http://rs.colortex.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fb.panjiajie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kw.shxzskj.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nb.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kn.shxzskj.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mm.bookmarksfly.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pv.shtwfgs.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mz.huixinmuqiang.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qh.shtwfgs.cn

[B04] for 计数循环
来源：http://ae.bjjhwx.cn

Py:   for i in range(10): print(i)
来源：http://cb.colortex.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zg.jctech888.com.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ho.yuntaijiaju.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ng.huixiangedu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aq.asd995.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pl.bjjhwx.cn

Ruby: 10.times { |i| puts i }
来源：http://cz.yuexingan06.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mj.yuexingan06.cn

[B05] 遍历数组 / 列表
来源：http://sk.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://zm.shxzskj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hk.hahajie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://va.nicolike.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ye.huanxung.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ug.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ip.shtwfgs.cn

Ruby: arr.each { |item| puts item }
来源：http://ci.521024.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ey.colortex.cn

[B06] 遍历字典 / 对象
来源：http://ap.521024.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gn.521024.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kg.nszjky.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cb.colortex.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ef.yuntaijiaju.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jk.lnxyls.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fe.szxytkj.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ge.shxzskj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zs.hnjuh.cn

[B07] while 循环
来源：http://wv.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://ih.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xd.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://ib.nicolike.cn

TS:   while (i < 10) { i++; }
来源：http://to.bjjhwx.cn

Java: while (i < 10) { i++; }
来源：http://sa.wgjwhj.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://me.colortex.cn

Ruby: while i < 10; i += 1; end
来源：http://ei.huixinmuqiang.cn

C#:   while (i < 10) { i++; }
来源：http://iu.yuntaijiaju.cn

[B08] do-while（至少执行一次）
来源：http://ix.lnxyls.cn

Py:   # 无 do-while：用 while True + break
来源：http://hs.szsharing.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uc.jianghongdianzi.cn

JS:   do { i++; } while (i < 10);
来源：http://he.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://pi.hnjuh.cn

Java: do { i++; } while (i < 10);
来源：http://ts.gzmigu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ul.hnjuh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jf.bjjhwx.cn

C#:   do { i++; } while (i < 10);
来源：http://gn.colortex.cn

[B09] break 与 continue
来源：http://nf.shxzskj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fx.huixinmuqiang.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ne.chemitech.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fw.szxytkj.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zr.gzmigu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gv.hahajie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mz.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yg.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://em.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://je.gzmigu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ey.hahajie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kx.bjjhwx.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ru.shxzukj.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qj.hnjuh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cn.nicolike.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wf.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://on.bjjhwx.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lx.521024.cn

[B11] 生成数字序列 / 区间
来源：http://ma.haigaiapp.cn

Py:   list(range(0, 10, 2))
来源：http://qa.lnxyls.cn

PHP:  range(0, 10, 2);
来源：http://gy.gzmigu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pk.yuexingan06.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qf.bookmarksfly.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vj.asd995.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qz.lnxyls.cn

Ruby: (0...10).step(2).to_a
来源：http://ba.shxzukj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xo.lnxyls.cn

[B12] 跳出多层循环
来源：http://kg.shxzukj.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iw.huixiangedu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://do.shxzskj.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dr.jianghongdianzi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ke.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wn.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://up.jianghongdianzi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://st.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pd.jianghongdianzi.cn

[B13] 判断是否为数字
来源：http://lz.colortex.cn

Py:   isinstance(x, (int, float))
来源：http://le.szsharing.cn

PHP:  is_numeric($x)
来源：http://bh.shtwfgs.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xc.hnjuh.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hm.colortex.cn

Java: x instanceof Number
来源：http://to.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bw.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://ll.bookmarksfly.cn

C#:   x is int or double or decimal
来源：http://rp.jianghongdianzi.cn

[B14] 判断值是否在集合内
来源：http://jg.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://in.hahajie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cn.szsharing.cn

JS:   [1, 2, 3].includes(x)
来源：http://jk.huixiangedu.cn

TS:   [1, 2, 3].includes(x)
来源：http://wi.huanxung.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dd.wgjwhj.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zo.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lh.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eq.wgjwhj.cn

[B15] 布尔运算与取反
来源：http://lw.asd995.cn

Py:   a and b or not c
来源：http://yc.hahajie.cn

PHP:  $a && $b || !$c
来源：http://nz.shxzskj.cn

JS:   a && b || !c
来源：http://qp.521024.cn

TS:   a && b || !c
来源：http://do.jianghongdianzi.cn

Java: a && b || !c
来源：http://pe.jctech888.com.cn

Go:   a && b || !c
来源：http://ii.shxzskj.cn

Ruby: a && b || !c
来源：http://wx.jctech888.com.cn

C#:   a && b || !c
来源：http://uv.9csxet.cn

[B16] 卫语句：不满足条件提前返回
来源：http://py.wgjwhj.cn

Py:   if not data: return
来源：http://wn.nszjky.cn

PHP:  if (!$data) { return; }
来源：http://zi.bookmarksfly.cn

JS:   if (!data) return;
来源：http://fd.huixiangedu.cn

TS:   if (!data) return;
来源：http://vn.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://vb.bookmarksfly.cn

Go:   if data == nil { return }
来源：http://tz.hahajie.cn

Ruby: return if data.nil?
来源：http://ns.hahajie.cn

C#:   if (data == null) return;
来源：http://pr.nicolike.cn

================================================================================
来源：http://mw.newstarts.cn

C. 函数与作用域
来源：http://iu.huixinmuqiang.cn

================================================================================
来源：http://nu.nszjky.cn

[C01] 定义函数
来源：http://og.bookmarksfly.cn


<!-- 参考信息 -->