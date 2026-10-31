代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://md.huanxung.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qk.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://wr.yuntaijiaju.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://eg.chemitech.net.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://od.yuntaijiaju.cn

JS:   `Hello, ${name}!`
来源：http://ft.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://ki.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://iz.nicolike.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vw.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://zi.szxytkj.cn

C#:   $"Hello, {name}!"
来源：http://lb.hnjuh.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://mg.szxytkj.cn

Py:   "第一行\n第二行"
来源：http://ux.nszjky.cn

PHP:  "第一行\n第二行"
来源：http://ox.muxihuayi.cn

JS:   "第一行\n第二行"
来源：http://zm.521024.cn

TS:   "第一行\n第二行"
来源：http://zm.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://zk.521024.cn

Go:   "第一行\n第二行"
来源：http://oq.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://nx.shxzukj.cn

C#:   "第一行\n第二行"
来源：http://gx.shxzskj.cn

[A14] 注释写法
来源：http://un.nicolike.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://np.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sy.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://ja.gzmigu.cn

TS:   // 单行；/* 多行 */
来源：http://db.lnxyls.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yz.szxytkj.cn

Go:   // 单行；/* 多行 */
来源：http://qt.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ca.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://fm.shxzukj.cn

[A15] 空值判断与默认值
来源：http://ja.jianghongdianzi.cn

Py:   value = data or "默认值"
来源：http://uu.hnjuh.cn

PHP:  $value = $data ?? "默认值";
来源：http://gu.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://gv.muxihuayi.cn

TS:   const value = data ?? "默认值";
来源：http://rp.shxzskj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qc.hnjuh.cn

Go:   if data == "" { data = "默认值" }
来源：http://ml.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://bt.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://jv.nszjky.cn

[A16] 真假值判断规则
来源：http://fx.lnxyls.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rs.jianghongdianzi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cu.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jf.bookmarksfly.cn

TS:   if (!x) {}
来源：http://kb.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pu.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gb.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://st.asd995.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hh.521024.cn

[A17] 位运算
来源：http://zc.shxzukj.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gp.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hf.jianghongdianzi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xq.9csxet.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zo.muxihuayi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vx.nszjky.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sj.nszjky.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mx.haigaiapp.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ko.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://sq.gzmigu.cn

Py:   ord("A"); chr(65)
来源：http://ao.szxytkj.cn

PHP:  ord("A"); chr(65)
来源：http://ge.9csxet.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wi.yuexingan06.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zl.bjjhwx.cn

Java: (int) 'A'; (char) 65
来源：http://so.szxytkj.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hu.gzmigu.cn

Ruby: "A".ord; 65.chr
来源：http://ff.huixiangedu.cn

C#:   (int)'A'; (char)65
来源：http://jo.huixinmuqiang.cn

[A19] 交换两个变量
来源：http://xb.jctech888.com.cn

Py:   a, b = b, a
来源：http://ht.wgjwhj.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://br.chemitech.net.cn

JS:   [a, b] = [b, a];
来源：http://of.nszjky.cn

TS:   [a, b] = [b, a];
来源：http://ab.yuntaijiaju.cn

Java: int t = a; a = b; b = t;
来源：http://rh.huanxung.cn

Go:   a, b = b, a
来源：http://wa.jctech888.com.cn

Ruby: a, b = b, a
来源：http://qy.hnjuh.cn

C#:   (a, b) = (b, a);
来源：http://gx.huanxung.cn

[A20] 读取标准输入
来源：http://ij.hahajie.cn

Py:   name = input("请输入：")
来源：http://wq.yuntaijiaju.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ro.shxzukj.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jc.huixiangedu.cn

TS:   // Node.js：readline 模块
来源：http://do.9csxet.cn

Java: new Scanner(System.in).nextLine()
来源：http://pp.huixinmuqiang.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jv.nicolike.cn

Ruby: gets.chomp
来源：http://eo.chemitech.net.cn

C#:   Console.ReadLine();
来源：http://fg.9csxet.cn

[A21] 保留指定小数位输出
来源：http://sk.jctech888.com.cn

Py:   f"{3.14159:.2f}"
来源：http://cc.colortex.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://st.hnjuh.cn

JS:   (3.14159).toFixed(2)
来源：http://kh.jctech888.com.cn

TS:   (3.14159).toFixed(2)
来源：http://yj.asd995.cn

Java: String.format("%.2f", 3.14159)
来源：http://es.521024.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fi.hahajie.cn

Ruby: format("%.2f", 3.14159)
来源：http://kj.bookmarksfly.cn

C#:   3.14159.ToString("F2")
来源：http://zg.szxytkj.cn

[A22] 获取字符串长度
来源：http://fx.shxzskj.cn

Py:   len(s)
来源：http://ah.shxzskj.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://za.shxzukj.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dk.newstarts.cn

TS:   s.length
来源：http://tz.gzmigu.cn

Java: s.length()
来源：http://bs.huixinmuqiang.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vg.lnxyls.cn

Ruby: s.length
来源：http://sj.jctech888.com.cn

C#:   s.Length
来源：http://cr.jctech888.com.cn

[A23] 大小写转换
来源：http://us.wgjwhj.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ph.wgjwhj.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zr.gzmigu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://or.huixiangedu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lb.9csxet.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gr.bjjhwx.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jw.gzmigu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xh.bookmarksfly.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uq.haigaiapp.cn

[A24] 去除首尾空白
来源：http://qj.bookmarksfly.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jx.shxzskj.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bd.newstarts.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ws.shtwfgs.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ns.szxytkj.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bp.szxytkj.cn

Go:   strings.TrimSpace(s)
来源：http://nn.9csxet.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ux.jianghongdianzi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zw.shxzukj.cn

[A25] 字符串比较
来源：http://yw.jianghongdianzi.cn

Py:   s1 == s2; s1 != s2
来源：http://qz.szsharing.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eu.9csxet.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ym.jianghongdianzi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eq.shxzskj.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nj.hahajie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pg.nszjky.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qu.shtwfgs.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wx.nicolike.cn

[A26] 类型转换总览
来源：http://oz.chemitech.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wi.shxzskj.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ar.huixinmuqiang.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cb.hahajie.cn

TS:   Number() String() Boolean() x as number
来源：http://au.newstarts.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ko.asd995.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kb.wgjwhj.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ux.panjiajie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wg.jianghongdianzi.cn

================================================================================
来源：http://qq.muxihuayi.cn

B. 流程控制
来源：http://uf.jctech888.com.cn

================================================================================
来源：http://mx.bjjhwx.cn

[B01] 条件判断 if / else
来源：http://jy.wgjwhj.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ci.shxzukj.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ke.nicolike.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bn.szxytkj.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qt.muxihuayi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ri.9csxet.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yr.gzmigu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gb.bjjhwx.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xv.gzmigu.cn

[B02] 多分支 else if / elif
来源：http://yt.shxzskj.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kt.yuntaijiaju.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bq.hahajie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oz.yuntaijiaju.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mn.chemitech.net.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fb.wgjwhj.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rf.szsharing.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yr.jianghongdianzi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ck.panjiajie.cn

[B03] switch / match / case
来源：http://kw.lnxyls.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pc.bjjhwx.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oj.bjjhwx.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ul.jctech888.com.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vs.521024.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ut.huixinmuqiang.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vd.521024.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oa.521024.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oe.yuexingan06.cn

[B04] for 计数循环
来源：http://zz.muxihuayi.cn

Py:   for i in range(10): print(i)
来源：http://qn.panjiajie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pe.nicolike.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dd.wgjwhj.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iv.nicolike.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mk.chemitech.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hu.nszjky.cn

Ruby: 10.times { |i| puts i }
来源：http://hx.jctech888.com.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gz.asd995.cn

[B05] 遍历数组 / 列表
来源：http://xj.haigaiapp.cn

Py:   for item in arr: print(item)
来源：http://og.chemitech.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bz.shxzukj.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://go.shtwfgs.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ji.shxzskj.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lt.nszjky.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://uv.huanxung.cn

Ruby: arr.each { |item| puts item }
来源：http://an.wgjwhj.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mf.szsharing.cn

[B06] 遍历字典 / 对象
来源：http://qf.haigaiapp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cd.huanxung.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gq.szxytkj.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kt.panjiajie.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gu.lnxyls.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hl.chemitech.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ri.lnxyls.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ra.lnxyls.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vm.muxihuayi.cn

[B07] while 循环
来源：http://jb.muxihuayi.cn

Py:   while i < 10: i += 1
来源：http://kw.huixinmuqiang.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xe.szxytkj.cn

JS:   while (i < 10) { i++; }
来源：http://zn.panjiajie.cn

TS:   while (i < 10) { i++; }
来源：http://jj.yuntaijiaju.cn

Java: while (i < 10) { i++; }
来源：http://pt.jctech888.com.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eu.chemitech.net.cn

Ruby: while i < 10; i += 1; end
来源：http://xl.jianghongdianzi.cn

C#:   while (i < 10) { i++; }
来源：http://tp.szsharing.cn

[B08] do-while（至少执行一次）
来源：http://po.yuntaijiaju.cn

Py:   # 无 do-while：用 while True + break
来源：http://ix.nszjky.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fh.jctech888.com.cn

JS:   do { i++; } while (i < 10);
来源：http://bt.hnjuh.cn

TS:   do { i++; } while (i < 10);
来源：http://bf.szsharing.cn

Java: do { i++; } while (i < 10);
来源：http://tr.haigaiapp.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vx.haigaiapp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://la.muxihuayi.cn

C#:   do { i++; } while (i < 10);
来源：http://hs.nicolike.cn

[B09] break 与 continue
来源：http://cc.muxihuayi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://db.bookmarksfly.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yb.9csxet.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vr.bjjhwx.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rv.newstarts.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://on.jctech888.com.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uf.shtwfgs.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ic.nszjky.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vo.muxihuayi.cn

[B10] 遍历同时拿索引
来源：http://qk.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dc.shtwfgs.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fk.huixiangedu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vf.jianghongdianzi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uq.9csxet.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nv.huixiangedu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pw.bookmarksfly.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://if.huanxung.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yk.jianghongdianzi.cn

[B11] 生成数字序列 / 区间
来源：http://bi.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://mf.nszjky.cn

PHP:  range(0, 10, 2);
来源：http://xw.jctech888.com.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lc.hahajie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wk.chemitech.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vj.yuexingan06.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bc.hnjuh.cn

Ruby: (0...10).step(2).to_a
来源：http://ic.bjjhwx.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bd.lnxyls.cn

[B12] 跳出多层循环
来源：http://nz.yuntaijiaju.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fe.hnjuh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://je.bjjhwx.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ij.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ya.haigaiapp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://al.szxytkj.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://th.szsharing.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wg.muxihuayi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tg.shtwfgs.cn

[B13] 判断是否为数字
来源：http://lm.gzmigu.cn

Py:   isinstance(x, (int, float))
来源：http://yz.yuexingan06.cn

PHP:  is_numeric($x)
来源：http://wj.521024.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mh.bookmarksfly.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kf.521024.cn

Java: x instanceof Number
来源：http://dy.jianghongdianzi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xb.yuntaijiaju.cn

Ruby: x.is_a?(Numeric)
来源：http://do.jctech888.com.cn

C#:   x is int or double or decimal
来源：http://tk.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://ld.chemitech.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yd.chemitech.net.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bh.wgjwhj.cn

JS:   [1, 2, 3].includes(x)
来源：http://sa.jianghongdianzi.cn

TS:   [1, 2, 3].includes(x)
来源：http://fg.nicolike.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ye.9csxet.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ex.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bu.hnjuh.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vv.jianghongdianzi.cn

[B15] 布尔运算与取反
来源：http://py.yuexingan06.cn

Py:   a and b or not c
来源：http://nk.hahajie.cn

PHP:  $a && $b || !$c
来源：http://np.hnjuh.cn

JS:   a && b || !c
来源：http://ic.haigaiapp.cn

TS:   a && b || !c
来源：http://hf.haigaiapp.cn

Java: a && b || !c
来源：http://eo.lnxyls.cn

Go:   a && b || !c
来源：http://ni.muxihuayi.cn

Ruby: a && b || !c
来源：http://mx.shtwfgs.cn

C#:   a && b || !c
来源：http://dh.shxzskj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lc.9csxet.cn

Py:   if not data: return
来源：http://mb.9csxet.cn

PHP:  if (!$data) { return; }
来源：http://xw.asd995.cn

JS:   if (!data) return;
来源：http://nu.panjiajie.cn

TS:   if (!data) return;
来源：http://kn.yuntaijiaju.cn

Java: if (data == null) return;
来源：http://tt.gzmigu.cn

Go:   if data == nil { return }
来源：http://jd.colortex.cn

Ruby: return if data.nil?
来源：http://io.szsharing.cn

C#:   if (data == null) return;
来源：http://sa.yuexingan06.cn

================================================================================
来源：http://hg.gzmigu.cn

C. 函数与作用域
来源：http://dj.newstarts.cn

================================================================================
来源：http://to.asd995.cn

[C01] 定义函数
来源：http://mo.asd995.cn

Py:   def add(a, b): return a + b
来源：http://wx.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ow.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://rc.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://et.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rh.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ey.521024.cn

Ruby: def add(a, b); a + b; end
来源：http://au.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kp.huanxung.cn

[C02] 默认参数
来源：http://zz.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://ka.jianghongdianzi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dl.hahajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://ct.shxzukj.cn


<!-- 参考信息 -->