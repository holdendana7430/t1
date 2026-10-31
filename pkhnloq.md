代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ub.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://eg.gzmigu.cn

TS:   `Hello, ${name}!`
来源：http://dm.haigaiapp.cn

Java: "Hello, %s!".formatted(name)
来源：http://ou.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jw.huixiangedu.cn

Ruby: "Hello, #{name}!"
来源：http://la.hnjuh.cn

C#:   $"Hello, {name}!"
来源：http://if.panjiajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xe.shxzskj.cn

Py:   "第一行\n第二行"
来源：http://jj.muxihuayi.cn

PHP:  "第一行\n第二行"
来源：http://ic.colortex.cn

JS:   "第一行\n第二行"
来源：http://xg.nszjky.cn

TS:   "第一行\n第二行"
来源：http://pe.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://iu.nicolike.cn

Go:   "第一行\n第二行"
来源：http://dd.jctech888.com.cn

Ruby: "第一行\n第二行"
来源：http://hl.9csxet.cn

C#:   "第一行\n第二行"
来源：http://vp.yuexingan06.cn

[A14] 注释写法
来源：http://gz.521024.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dr.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qt.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://rq.bjjhwx.cn

TS:   // 单行；/* 多行 */
来源：http://wb.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wo.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://er.shtwfgs.cn

Ruby: # 单行；=begin 多行 =end
来源：http://za.shxzukj.cn

C#:   // 单行；/* 多行 */
来源：http://kt.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://zg.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://kr.shxzskj.cn

PHP:  $value = $data ?? "默认值";
来源：http://wd.haigaiapp.cn

JS:   const value = data ?? "默认值";
来源：http://ko.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://fz.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rd.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://td.nszjky.cn

Ruby: value = data || "默认值"
来源：http://yo.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://vx.bookmarksfly.cn

[A16] 真假值判断规则
来源：http://yn.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fg.panjiajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wl.bjjhwx.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zd.lnxyls.cn

TS:   if (!x) {}
来源：http://if.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://is.hahajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tz.nszjky.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fi.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nz.bookmarksfly.cn

[A17] 位运算
来源：http://wj.shxzskj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://on.colortex.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://md.lnxyls.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xw.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rx.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dk.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lz.521024.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ro.colortex.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pc.yuexingan06.cn

[A18] 字符与 ASCII 码互转
来源：http://bp.chemitech.net.cn

Py:   ord("A"); chr(65)
来源：http://sy.shtwfgs.cn

PHP:  ord("A"); chr(65)
来源：http://ag.chemitech.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nw.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eg.jctech888.com.cn

Java: (int) 'A'; (char) 65
来源：http://dz.colortex.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vy.521024.cn

Ruby: "A".ord; 65.chr
来源：http://xa.521024.cn

C#:   (int)'A'; (char)65
来源：http://xw.muxihuayi.cn

[A19] 交换两个变量
来源：http://mh.colortex.cn

Py:   a, b = b, a
来源：http://kr.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://un.panjiajie.cn

JS:   [a, b] = [b, a];
来源：http://uu.shxzskj.cn

TS:   [a, b] = [b, a];
来源：http://zo.szxytkj.cn

Java: int t = a; a = b; b = t;
来源：http://td.asd995.cn

Go:   a, b = b, a
来源：http://mh.jianghongdianzi.cn

Ruby: a, b = b, a
来源：http://dt.bjjhwx.cn

C#:   (a, b) = (b, a);
来源：http://zr.asd995.cn

[A20] 读取标准输入
来源：http://bb.newstarts.cn

Py:   name = input("请输入：")
来源：http://gv.jctech888.com.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vk.yuexingan06.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rz.bjjhwx.cn

TS:   // Node.js：readline 模块
来源：http://fw.shxzukj.cn

Java: new Scanner(System.in).nextLine()
来源：http://uu.wgjwhj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://en.nicolike.cn

Ruby: gets.chomp
来源：http://dw.jctech888.com.cn

C#:   Console.ReadLine();
来源：http://vu.huixinmuqiang.cn

[A21] 保留指定小数位输出
来源：http://sr.yuntaijiaju.cn

Py:   f"{3.14159:.2f}"
来源：http://sk.asd995.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ru.9csxet.cn

JS:   (3.14159).toFixed(2)
来源：http://jl.szxytkj.cn

TS:   (3.14159).toFixed(2)
来源：http://kj.shtwfgs.cn

Java: String.format("%.2f", 3.14159)
来源：http://ak.muxihuayi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jt.shtwfgs.cn

Ruby: format("%.2f", 3.14159)
来源：http://wl.nszjky.cn

C#:   3.14159.ToString("F2")
来源：http://ii.asd995.cn

[A22] 获取字符串长度
来源：http://ar.muxihuayi.cn

Py:   len(s)
来源：http://ar.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bz.huixiangedu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xf.9csxet.cn

TS:   s.length
来源：http://tq.szxytkj.cn

Java: s.length()
来源：http://ao.colortex.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oj.jctech888.com.cn

Ruby: s.length
来源：http://rw.9csxet.cn

C#:   s.Length
来源：http://ri.huixiangedu.cn

[A23] 大小写转换
来源：http://re.hahajie.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qf.huanxung.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ra.lnxyls.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kw.yuexingan06.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sn.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fu.lnxyls.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jh.hnjuh.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ci.yuntaijiaju.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://sc.yuntaijiaju.cn

[A24] 去除首尾空白
来源：http://xx.panjiajie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uv.szsharing.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sj.szsharing.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rn.chemitech.net.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ok.asd995.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://si.huixinmuqiang.cn

Go:   strings.TrimSpace(s)
来源：http://tw.bjjhwx.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ov.hnjuh.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://un.huanxung.cn

[A25] 字符串比较
来源：http://js.panjiajie.cn

Py:   s1 == s2; s1 != s2
来源：http://mh.gzmigu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ig.huixiangedu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yh.shtwfgs.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rv.huixinmuqiang.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hk.szsharing.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://be.lnxyls.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zt.huixinmuqiang.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kb.shxzskj.cn

[A26] 类型转换总览
来源：http://go.bookmarksfly.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hk.huixiangedu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vq.hnjuh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kl.szsharing.cn

TS:   Number() String() Boolean() x as number
来源：http://rz.hnjuh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jctech888.com.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://be.szxytkj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ch.huixiangedu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wd.yuntaijiaju.cn

================================================================================
来源：http://yb.lnxyls.cn

B. 流程控制
来源：http://zp.asd995.cn

================================================================================
来源：http://uv.chemitech.net.cn

[B01] 条件判断 if / else
来源：http://qn.szsharing.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dq.nszjky.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ik.jianghongdianzi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ln.yuexingan06.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mi.shxzskj.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sq.shtwfgs.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bz.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cf.huixinmuqiang.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mz.chemitech.net.cn

[B02] 多分支 else if / elif
来源：http://le.huixiangedu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cn.muxihuayi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://et.wgjwhj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lt.haigaiapp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kc.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ll.asd995.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hr.wgjwhj.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rf.9csxet.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tp.jctech888.com.cn

[B03] switch / match / case
来源：http://hc.bjjhwx.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gm.jctech888.com.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kr.shtwfgs.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ef.huixinmuqiang.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ft.huixinmuqiang.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jo.shtwfgs.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hu.newstarts.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ei.panjiajie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ax.521024.cn

[B04] for 计数循环
来源：http://uh.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://hg.huixinmuqiang.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fj.521024.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://md.colortex.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ov.panjiajie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fp.shtwfgs.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ld.yuexingan06.cn

Ruby: 10.times { |i| puts i }
来源：http://je.huixiangedu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cj.chemitech.net.cn

[B05] 遍历数组 / 列表
来源：http://gr.yuntaijiaju.cn

Py:   for item in arr: print(item)
来源：http://cy.panjiajie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dy.nszjky.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://by.chemitech.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hg.nicolike.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ai.panjiajie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yt.bookmarksfly.cn

Ruby: arr.each { |item| puts item }
来源：http://tx.jianghongdianzi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gx.wgjwhj.cn

[B06] 遍历字典 / 对象
来源：http://vc.shxzukj.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://xm.lnxyls.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wa.hnjuh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rm.bookmarksfly.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cw.nszjky.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xt.newstarts.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hn.gzmigu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ac.wgjwhj.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oh.lnxyls.cn

[B07] while 循环
来源：http://oz.bjjhwx.cn

Py:   while i < 10: i += 1
来源：http://qj.wgjwhj.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gu.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://na.shtwfgs.cn

TS:   while (i < 10) { i++; }
来源：http://wb.hnjuh.cn

Java: while (i < 10) { i++; }
来源：http://hz.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lm.hahajie.cn

Ruby: while i < 10; i += 1; end
来源：http://xl.muxihuayi.cn

C#:   while (i < 10) { i++; }
来源：http://dd.huanxung.cn

[B08] do-while（至少执行一次）
来源：http://yi.shxzskj.cn

Py:   # 无 do-while：用 while True + break
来源：http://ni.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gc.muxihuayi.cn

JS:   do { i++; } while (i < 10);
来源：http://yb.9csxet.cn

TS:   do { i++; } while (i < 10);
来源：http://tm.panjiajie.cn

Java: do { i++; } while (i < 10);
来源：http://by.yuexingan06.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dd.shxzukj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://et.huixinmuqiang.cn

C#:   do { i++; } while (i < 10);
来源：http://df.shxzukj.cn

[B09] break 与 continue
来源：http://up.wgjwhj.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://tt.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gp.huixiangedu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://la.hnjuh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ko.colortex.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ab.shxzskj.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ra.yuntaijiaju.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://da.jianghongdianzi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zh.bjjhwx.cn

[B10] 遍历同时拿索引
来源：http://qj.jctech888.com.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ka.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mu.lnxyls.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vb.chemitech.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mb.panjiajie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://px.yuexingan06.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pm.shtwfgs.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tm.jctech888.com.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://od.nicolike.cn

[B11] 生成数字序列 / 区间
来源：http://ti.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://lu.yuntaijiaju.cn

PHP:  range(0, 10, 2);
来源：http://hn.asd995.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gh.yuntaijiaju.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ww.huanxung.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uv.gzmigu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lu.muxihuayi.cn

Ruby: (0...10).step(2).to_a
来源：http://hg.shxzskj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jp.nicolike.cn

[B12] 跳出多层循环
来源：http://ie.huanxung.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gj.wgjwhj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ma.huixiangedu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jj.yuntaijiaju.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fk.panjiajie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tb.nicolike.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vh.521024.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gg.huixiangedu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xe.chemitech.net.cn

[B13] 判断是否为数字
来源：http://oj.haigaiapp.cn

Py:   isinstance(x, (int, float))
来源：http://fb.panjiajie.cn

PHP:  is_numeric($x)
来源：http://pg.lnxyls.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xm.9csxet.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://do.asd995.cn

Java: x instanceof Number
来源：http://ak.asd995.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://un.szsharing.cn

Ruby: x.is_a?(Numeric)
来源：http://hm.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://vb.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://eh.asd995.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sq.huanxung.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tf.gzmigu.cn

JS:   [1, 2, 3].includes(x)
来源：http://kx.bjjhwx.cn

TS:   [1, 2, 3].includes(x)
来源：http://ee.huixinmuqiang.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fi.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://em.newstarts.cn

Ruby: [1, 2, 3].include?(x)
来源：http://oo.nszjky.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ul.gzmigu.cn

[B15] 布尔运算与取反
来源：http://zq.521024.cn

Py:   a and b or not c
来源：http://ph.newstarts.cn

PHP:  $a && $b || !$c
来源：http://up.yuntaijiaju.cn

JS:   a && b || !c
来源：http://op.shxzukj.cn

TS:   a && b || !c
来源：http://iw.yuntaijiaju.cn

Java: a && b || !c
来源：http://xi.szxytkj.cn

Go:   a && b || !c
来源：http://rx.jctech888.com.cn

Ruby: a && b || !c
来源：http://rx.yuexingan06.cn

C#:   a && b || !c
来源：http://gx.nicolike.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bl.haigaiapp.cn

Py:   if not data: return
来源：http://fp.bookmarksfly.cn

PHP:  if (!$data) { return; }
来源：http://by.asd995.cn

JS:   if (!data) return;
来源：http://sf.9csxet.cn

TS:   if (!data) return;
来源：http://wt.hnjuh.cn

Java: if (data == null) return;
来源：http://ic.gzmigu.cn

Go:   if data == nil { return }
来源：http://nh.bookmarksfly.cn

Ruby: return if data.nil?
来源：http://vt.521024.cn

C#:   if (data == null) return;
来源：http://zn.colortex.cn

================================================================================
来源：http://nk.huixiangedu.cn

C. 函数与作用域
来源：http://rm.9csxet.cn

================================================================================
来源：http://wz.hnjuh.cn

[C01] 定义函数
来源：http://mf.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://ve.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hx.hnjuh.cn

JS:   function add(a, b) { return a + b; }
来源：http://yd.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hc.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mv.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zd.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://be.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pz.szxytkj.cn

[C02] 默认参数
来源：http://sp.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://bf.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bb.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://tu.huixiangedu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ut.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xd.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bf.bookmarksfly.cn

Ruby: def greet(name = "World") = name
来源：http://xe.haigaiapp.cn


<!-- 参考信息 -->