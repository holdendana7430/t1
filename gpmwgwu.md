代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lh.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://wc.521024.cn

TS:   `Hello, ${name}!`
来源：http://qo.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://su.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://iy.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://in.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://fz.huixinmuqiang.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tu.colortex.cn

Py:   "第一行\n第二行"
来源：http://rq.lnxyls.cn

PHP:  "第一行\n第二行"
来源：http://us.shxzskj.cn

JS:   "第一行\n第二行"
来源：http://md.9csxet.cn

TS:   "第一行\n第二行"
来源：http://uw.yuexingan06.cn

Java: "第一行\n第二行"
来源：http://cy.huanxung.cn

Go:   "第一行\n第二行"
来源：http://dy.521024.cn

Ruby: "第一行\n第二行"
来源：http://bq.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://pu.panjiajie.cn

[A14] 注释写法
来源：http://it.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kl.huixinmuqiang.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qq.hahajie.cn

JS:   // 单行；/* 多行 */
来源：http://ja.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://op.gzmigu.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yu.chemitech.net.cn

Go:   // 单行；/* 多行 */
来源：http://bs.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nl.szxytkj.cn

C#:   // 单行；/* 多行 */
来源：http://fv.szxytkj.cn

[A15] 空值判断与默认值
来源：http://sh.nicolike.cn

Py:   value = data or "默认值"
来源：http://xp.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://vp.wgjwhj.cn

JS:   const value = data ?? "默认值";
来源：http://da.shxzskj.cn

TS:   const value = data ?? "默认值";
来源：http://to.chemitech.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ww.panjiajie.cn

Go:   if data == "" { data = "默认值" }
来源：http://nq.haigaiapp.cn

Ruby: value = data || "默认值"
来源：http://gw.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://rz.huanxung.cn

[A16] 真假值判断规则
来源：http://zs.nicolike.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mw.colortex.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ic.huanxung.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ga.521024.cn

TS:   if (!x) {}
来源：http://to.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zw.shtwfgs.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hu.lnxyls.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ge.shxzskj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nc.chemitech.net.cn

[A17] 位运算
来源：http://ad.colortex.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sn.shtwfgs.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ji.chemitech.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ca.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qn.9csxet.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eg.wgjwhj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bm.gzmigu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ng.szxytkj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qk.muxihuayi.cn

[A18] 字符与 ASCII 码互转
来源：http://oh.hahajie.cn

Py:   ord("A"); chr(65)
来源：http://tc.shxzskj.cn

PHP:  ord("A"); chr(65)
来源：http://vg.nszjky.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nk.asd995.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kc.yuntaijiaju.cn

Java: (int) 'A'; (char) 65
来源：http://bd.szsharing.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ko.wgjwhj.cn

Ruby: "A".ord; 65.chr
来源：http://ym.huanxung.cn

C#:   (int)'A'; (char)65
来源：http://dn.9csxet.cn

[A19] 交换两个变量
来源：http://op.bjjhwx.cn

Py:   a, b = b, a
来源：http://zi.lnxyls.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://oq.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://rq.jctech888.com.cn

TS:   [a, b] = [b, a];
来源：http://gz.yuexingan06.cn

Java: int t = a; a = b; b = t;
来源：http://yg.szsharing.cn

Go:   a, b = b, a
来源：http://dm.yuntaijiaju.cn

Ruby: a, b = b, a
来源：http://zw.nszjky.cn

C#:   (a, b) = (b, a);
来源：http://ai.gzmigu.cn

[A20] 读取标准输入
来源：http://sq.muxihuayi.cn

Py:   name = input("请输入：")
来源：http://nd.nszjky.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ke.nszjky.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://iy.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://jg.shxzskj.cn

Java: new Scanner(System.in).nextLine()
来源：http://cn.shtwfgs.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sl.huanxung.cn

Ruby: gets.chomp
来源：http://lt.9csxet.cn

C#:   Console.ReadLine();
来源：http://of.521024.cn

[A21] 保留指定小数位输出
来源：http://ns.nszjky.cn

Py:   f"{3.14159:.2f}"
来源：http://jj.szxytkj.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ay.haigaiapp.cn

JS:   (3.14159).toFixed(2)
来源：http://bh.hnjuh.cn

TS:   (3.14159).toFixed(2)
来源：http://ai.nicolike.cn

Java: String.format("%.2f", 3.14159)
来源：http://wk.bookmarksfly.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gy.panjiajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://nf.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://us.yuntaijiaju.cn

[A22] 获取字符串长度
来源：http://hc.hnjuh.cn

Py:   len(s)
来源：http://jc.bookmarksfly.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pa.newstarts.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ok.panjiajie.cn

TS:   s.length
来源：http://kz.panjiajie.cn

Java: s.length()
来源：http://yw.bjjhwx.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nr.huanxung.cn

Ruby: s.length
来源：http://mi.jianghongdianzi.cn

C#:   s.Length
来源：http://fw.colortex.cn

[A23] 大小写转换
来源：http://lg.yuntaijiaju.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vl.gzmigu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xv.szsharing.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ug.szxytkj.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fw.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ag.nicolike.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kr.asd995.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rg.szxytkj.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hh.huixinmuqiang.cn

[A24] 去除首尾空白
来源：http://mq.wgjwhj.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pn.muxihuayi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hp.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dw.huixiangedu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pt.nicolike.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wi.huixiangedu.cn

Go:   strings.TrimSpace(s)
来源：http://zr.newstarts.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gf.gzmigu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hf.chemitech.net.cn

[A25] 字符串比较
来源：http://fz.shxzukj.cn

Py:   s1 == s2; s1 != s2
来源：http://tm.colortex.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rf.haigaiapp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eh.lnxyls.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wy.jianghongdianzi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://or.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gr.hahajie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vz.colortex.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ny.szxytkj.cn

[A26] 类型转换总览
来源：http://se.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hc.hahajie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aj.panjiajie.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zj.9csxet.cn

TS:   Number() String() Boolean() x as number
来源：http://bp.panjiajie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ix.nszjky.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fd.bjjhwx.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zg.muxihuayi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://un.yuntaijiaju.cn

================================================================================
来源：http://cv.nicolike.cn

B. 流程控制
来源：http://bm.szsharing.cn

================================================================================
来源：http://zb.szxytkj.cn

[B01] 条件判断 if / else
来源：http://xl.hnjuh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://xw.szsharing.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zn.hahajie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pr.szsharing.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tm.yuexingan06.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qb.hnjuh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vy.hnjuh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ny.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://df.shxzukj.cn

[B02] 多分支 else if / elif
来源：http://pc.521024.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bk.shxzukj.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fw.bjjhwx.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tn.shtwfgs.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://px.szsharing.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://el.hnjuh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lv.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jx.hnjuh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sq.panjiajie.cn

[B03] switch / match / case
来源：http://px.gzmigu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sf.gzmigu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kw.muxihuayi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://th.yuexingan06.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sq.shtwfgs.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zx.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qu.huanxung.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nq.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uz.shtwfgs.cn

[B04] for 计数循环
来源：http://us.9csxet.cn

Py:   for i in range(10): print(i)
来源：http://xm.gzmigu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wo.hahajie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xe.szxytkj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lw.bjjhwx.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uw.shxzskj.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fu.wgjwhj.cn

Ruby: 10.times { |i| puts i }
来源：http://im.bookmarksfly.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ar.521024.cn

[B05] 遍历数组 / 列表
来源：http://sf.lnxyls.cn

Py:   for item in arr: print(item)
来源：http://uk.wgjwhj.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ju.haigaiapp.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ng.521024.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://se.huixinmuqiang.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rj.huixinmuqiang.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vp.hnjuh.cn

Ruby: arr.each { |item| puts item }
来源：http://zk.szsharing.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://on.gzmigu.cn

[B06] 遍历字典 / 对象
来源：http://gl.huixiangedu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://is.szxytkj.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ng.bookmarksfly.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mv.huanxung.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ot.newstarts.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kb.szsharing.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pj.bjjhwx.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zu.bookmarksfly.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://py.jianghongdianzi.cn

[B07] while 循环
来源：http://jx.newstarts.cn

Py:   while i < 10: i += 1
来源：http://fu.521024.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ji.yuntaijiaju.cn

JS:   while (i < 10) { i++; }
来源：http://rr.asd995.cn

TS:   while (i < 10) { i++; }
来源：http://ts.huixinmuqiang.cn

Java: while (i < 10) { i++; }
来源：http://tz.lnxyls.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vl.wgjwhj.cn

Ruby: while i < 10; i += 1; end
来源：http://ta.jctech888.com.cn

C#:   while (i < 10) { i++; }
来源：http://rv.yuexingan06.cn

[B08] do-while（至少执行一次）
来源：http://tx.panjiajie.cn

Py:   # 无 do-while：用 while True + break
来源：http://uk.wgjwhj.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tt.yuntaijiaju.cn

JS:   do { i++; } while (i < 10);
来源：http://hx.hahajie.cn

TS:   do { i++; } while (i < 10);
来源：http://nq.jctech888.com.cn

Java: do { i++; } while (i < 10);
来源：http://fw.521024.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rr.newstarts.cn

Ruby: begin; i += 1; end while i < 10
来源：http://zh.bookmarksfly.cn

C#:   do { i++; } while (i < 10);
来源：http://rb.shtwfgs.cn

[B09] break 与 continue
来源：http://lb.521024.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vf.chemitech.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sl.colortex.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nc.huixiangedu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dq.jianghongdianzi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://au.bjjhwx.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dz.szsharing.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://be.wgjwhj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ph.colortex.cn

[B10] 遍历同时拿索引
来源：http://rg.hnjuh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qc.szxytkj.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fq.huixinmuqiang.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rb.bookmarksfly.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xf.yuntaijiaju.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ja.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://re.huixinmuqiang.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fz.muxihuayi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ct.huixiangedu.cn

[B11] 生成数字序列 / 区间
来源：http://hc.chemitech.net.cn

Py:   list(range(0, 10, 2))
来源：http://fg.chemitech.net.cn

PHP:  range(0, 10, 2);
来源：http://wr.jianghongdianzi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sr.bookmarksfly.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vq.yuexingan06.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rr.jctech888.com.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cy.shxzskj.cn

Ruby: (0...10).step(2).to_a
来源：http://eq.wgjwhj.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cp.asd995.cn

[B12] 跳出多层循环
来源：http://ox.bjjhwx.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mv.shxzukj.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://py.hahajie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gc.szsharing.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xh.wgjwhj.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yq.bookmarksfly.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ft.shxzukj.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cv.yuexingan06.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://me.asd995.cn

[B13] 判断是否为数字
来源：http://ql.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://wl.huixiangedu.cn

PHP:  is_numeric($x)
来源：http://af.huixinmuqiang.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ap.nicolike.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vn.muxihuayi.cn

Java: x instanceof Number
来源：http://ap.shxzukj.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dn.lnxyls.cn

Ruby: x.is_a?(Numeric)
来源：http://rd.shxzskj.cn

C#:   x is int or double or decimal
来源：http://gp.nicolike.cn

[B14] 判断值是否在集合内
来源：http://gg.yuntaijiaju.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fn.newstarts.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lk.hahajie.cn

JS:   [1, 2, 3].includes(x)
来源：http://ro.haigaiapp.cn

TS:   [1, 2, 3].includes(x)
来源：http://gn.yuexingan06.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kt.nszjky.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ub.hnjuh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://se.jctech888.com.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ti.panjiajie.cn

[B15] 布尔运算与取反
来源：http://iw.huanxung.cn

Py:   a and b or not c
来源：http://if.9csxet.cn

PHP:  $a && $b || !$c
来源：http://zk.huixinmuqiang.cn

JS:   a && b || !c
来源：http://gl.yuexingan06.cn

TS:   a && b || !c
来源：http://wy.wgjwhj.cn

Java: a && b || !c
来源：http://jy.panjiajie.cn

Go:   a && b || !c
来源：http://tl.newstarts.cn

Ruby: a && b || !c
来源：http://zx.521024.cn

C#:   a && b || !c
来源：http://dr.gzmigu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ts.gzmigu.cn

Py:   if not data: return
来源：http://ei.szsharing.cn

PHP:  if (!$data) { return; }
来源：http://gd.panjiajie.cn

JS:   if (!data) return;
来源：http://tx.9csxet.cn

TS:   if (!data) return;
来源：http://wo.jctech888.com.cn

Java: if (data == null) return;
来源：http://ok.nicolike.cn

Go:   if data == nil { return }
来源：http://hl.shxzskj.cn

Ruby: return if data.nil?
来源：http://dk.yuexingan06.cn

C#:   if (data == null) return;
来源：http://ib.haigaiapp.cn

================================================================================
来源：http://oj.lnxyls.cn

C. 函数与作用域
来源：http://kg.shtwfgs.cn

================================================================================
来源：http://td.haigaiapp.cn

[C01] 定义函数
来源：http://bb.muxihuayi.cn

Py:   def add(a, b): return a + b
来源：http://zg.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lr.szsharing.cn

JS:   function add(a, b) { return a + b; }
来源：http://mm.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ni.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ab.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qe.huixiangedu.cn

Ruby: def add(a, b); a + b; end
来源：http://ip.jctech888.com.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uo.shxzskj.cn

[C02] 默认参数
来源：http://hq.jianghongdianzi.cn

Py:   def greet(name="World"): return name
来源：http://im.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wp.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://oj.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://co.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wy.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pw.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://rv.hahajie.cn


<!-- 参考信息 -->