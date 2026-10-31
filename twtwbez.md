代发 wailian999

Py:   "第一行\n第二行"
来源：http://ef.wgjwhj.cn

PHP:  "第一行\n第二行"
来源：http://ja.hahajie.cn

JS:   "第一行\n第二行"
来源：http://rj.bookmarksfly.cn

TS:   "第一行\n第二行"
来源：http://pj.szsharing.cn

Java: "第一行\n第二行"
来源：http://rl.jctech888.com.cn

Go:   "第一行\n第二行"
来源：http://kl.huixiangedu.cn

Ruby: "第一行\n第二行"
来源：http://co.nicolike.cn

C#:   "第一行\n第二行"
来源：http://mp.panjiajie.cn

[A14] 注释写法
来源：http://rl.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bb.hnjuh.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qu.shxzukj.cn

JS:   // 单行；/* 多行 */
来源：http://sx.hnjuh.cn

TS:   // 单行；/* 多行 */
来源：http://ho.newstarts.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://li.muxihuayi.cn

Go:   // 单行；/* 多行 */
来源：http://ne.shtwfgs.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tt.jianghongdianzi.cn

C#:   // 单行；/* 多行 */
来源：http://bl.shxzukj.cn

[A15] 空值判断与默认值
来源：http://bk.chemitech.net.cn

Py:   value = data or "默认值"
来源：http://ba.muxihuayi.cn

PHP:  $value = $data ?? "默认值";
来源：http://yz.newstarts.cn

JS:   const value = data ?? "默认值";
来源：http://gb.yuntaijiaju.cn

TS:   const value = data ?? "默认值";
来源：http://ak.huixinmuqiang.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oh.szxytkj.cn

Go:   if data == "" { data = "默认值" }
来源：http://fo.hahajie.cn

Ruby: value = data || "默认值"
来源：http://kn.asd995.cn

C#:   var value = data ?? "默认值";
来源：http://fv.jctech888.com.cn

[A16] 真假值判断规则
来源：http://vr.shxzskj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wa.huanxung.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sm.muxihuayi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qt.szxytkj.cn

TS:   if (!x) {}
来源：http://tq.yuexingan06.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hs.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mp.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://dd.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vk.huixiangedu.cn

[A17] 位运算
来源：http://ar.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rr.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hk.asd995.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mj.jianghongdianzi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rb.huixinmuqiang.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kc.jctech888.com.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ll.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ll.szsharing.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pv.yuntaijiaju.cn

[A18] 字符与 ASCII 码互转
来源：http://vf.panjiajie.cn

Py:   ord("A"); chr(65)
来源：http://ru.521024.cn

PHP:  ord("A"); chr(65)
来源：http://od.muxihuayi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lm.nicolike.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bb.nicolike.cn

Java: (int) 'A'; (char) 65
来源：http://pb.huanxung.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ez.bookmarksfly.cn

Ruby: "A".ord; 65.chr
来源：http://mc.bjjhwx.cn

C#:   (int)'A'; (char)65
来源：http://mb.lnxyls.cn

[A19] 交换两个变量
来源：http://hg.jianghongdianzi.cn

Py:   a, b = b, a
来源：http://fn.nicolike.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qv.521024.cn

JS:   [a, b] = [b, a];
来源：http://fc.szxytkj.cn

TS:   [a, b] = [b, a];
来源：http://nm.lnxyls.cn

Java: int t = a; a = b; b = t;
来源：http://up.asd995.cn

Go:   a, b = b, a
来源：http://xa.bookmarksfly.cn

Ruby: a, b = b, a
来源：http://kn.colortex.cn

C#:   (a, b) = (b, a);
来源：http://ni.yuexingan06.cn

[A20] 读取标准输入
来源：http://zw.shtwfgs.cn

Py:   name = input("请输入：")
来源：http://th.yuexingan06.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wy.huixinmuqiang.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ml.hahajie.cn

TS:   // Node.js：readline 模块
来源：http://th.bookmarksfly.cn

Java: new Scanner(System.in).nextLine()
来源：http://ar.shxzskj.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vy.yuntaijiaju.cn

Ruby: gets.chomp
来源：http://ol.521024.cn

C#:   Console.ReadLine();
来源：http://sw.bookmarksfly.cn

[A21] 保留指定小数位输出
来源：http://jc.bjjhwx.cn

Py:   f"{3.14159:.2f}"
来源：http://ss.nicolike.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hc.yuntaijiaju.cn

JS:   (3.14159).toFixed(2)
来源：http://rp.muxihuayi.cn

TS:   (3.14159).toFixed(2)
来源：http://aq.nszjky.cn

Java: String.format("%.2f", 3.14159)
来源：http://ee.hahajie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kk.jctech888.com.cn

Ruby: format("%.2f", 3.14159)
来源：http://dv.haigaiapp.cn

C#:   3.14159.ToString("F2")
来源：http://ec.nszjky.cn

[A22] 获取字符串长度
来源：http://bg.panjiajie.cn

Py:   len(s)
来源：http://zu.szsharing.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://th.gzmigu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dh.haigaiapp.cn

TS:   s.length
来源：http://uv.huixinmuqiang.cn

Java: s.length()
来源：http://bs.yuntaijiaju.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://le.colortex.cn

Ruby: s.length
来源：http://ff.panjiajie.cn

C#:   s.Length
来源：http://ok.gzmigu.cn

[A23] 大小写转换
来源：http://hf.muxihuayi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hp.nszjky.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gq.nszjky.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vo.asd995.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ho.wgjwhj.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bq.haigaiapp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bz.szxytkj.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wv.muxihuayi.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fm.nszjky.cn

[A24] 去除首尾空白
来源：http://rw.hnjuh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yj.bookmarksfly.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fv.muxihuayi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bt.shxzukj.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uy.nszjky.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mc.bjjhwx.cn

Go:   strings.TrimSpace(s)
来源：http://df.yuexingan06.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://df.huixinmuqiang.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fj.shxzskj.cn

[A25] 字符串比较
来源：http://rp.colortex.cn

Py:   s1 == s2; s1 != s2
来源：http://bp.shtwfgs.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vi.newstarts.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bs.chemitech.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cz.asd995.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mb.muxihuayi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sq.hnjuh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jw.yuntaijiaju.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tx.bjjhwx.cn

[A26] 类型转换总览
来源：http://wf.yuexingan06.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wb.jctech888.com.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wu.colortex.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ru.521024.cn

TS:   Number() String() Boolean() x as number
来源：http://po.colortex.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ee.9csxet.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kl.huixinmuqiang.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ul.jctech888.com.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ub.chemitech.net.cn

================================================================================
来源：http://sl.muxihuayi.cn

B. 流程控制
来源：http://ny.panjiajie.cn

================================================================================
来源：http://uf.lnxyls.cn

[B01] 条件判断 if / else
来源：http://bc.huixinmuqiang.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://li.haigaiapp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xl.9csxet.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sn.lnxyls.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jb.yuntaijiaju.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://im.haigaiapp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xv.newstarts.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qu.newstarts.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ej.9csxet.cn

[B02] 多分支 else if / elif
来源：http://xv.lnxyls.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kr.bookmarksfly.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nv.szxytkj.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://km.szsharing.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://at.bookmarksfly.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pm.newstarts.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pp.newstarts.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gh.muxihuayi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://is.jianghongdianzi.cn

[B03] switch / match / case
来源：http://lf.hnjuh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bg.asd995.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uv.huixinmuqiang.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qm.szsharing.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mp.huixiangedu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ev.panjiajie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ti.huixinmuqiang.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fa.asd995.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ck.yuexingan06.cn

[B04] for 计数循环
来源：http://nx.gzmigu.cn

Py:   for i in range(10): print(i)
来源：http://qa.wgjwhj.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ff.muxihuayi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ka.nicolike.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lg.szxytkj.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://me.yuexingan06.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://to.shtwfgs.cn

Ruby: 10.times { |i| puts i }
来源：http://jp.colortex.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ck.panjiajie.cn

[B05] 遍历数组 / 列表
来源：http://hy.huanxung.cn

Py:   for item in arr: print(item)
来源：http://zb.9csxet.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bg.jctech888.com.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bl.yuexingan06.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ts.521024.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rg.bookmarksfly.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yv.wgjwhj.cn

Ruby: arr.each { |item| puts item }
来源：http://gh.bookmarksfly.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qg.hahajie.cn

[B06] 遍历字典 / 对象
来源：http://qa.nszjky.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://yw.chemitech.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gf.jctech888.com.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://al.521024.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dq.jctech888.com.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oz.shxzukj.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yz.chemitech.net.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jo.nicolike.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hj.shxzskj.cn

[B07] while 循环
来源：http://ym.shtwfgs.cn

Py:   while i < 10: i += 1
来源：http://df.panjiajie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zl.huixiangedu.cn

JS:   while (i < 10) { i++; }
来源：http://zh.gzmigu.cn

TS:   while (i < 10) { i++; }
来源：http://lw.jianghongdianzi.cn

Java: while (i < 10) { i++; }
来源：http://rj.521024.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nq.haigaiapp.cn

Ruby: while i < 10; i += 1; end
来源：http://gx.wgjwhj.cn

C#:   while (i < 10) { i++; }
来源：http://af.huixinmuqiang.cn

[B08] do-while（至少执行一次）
来源：http://nf.huixiangedu.cn

Py:   # 无 do-while：用 while True + break
来源：http://ut.panjiajie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ok.hnjuh.cn

JS:   do { i++; } while (i < 10);
来源：http://vr.huixinmuqiang.cn

TS:   do { i++; } while (i < 10);
来源：http://do.yuexingan06.cn

Java: do { i++; } while (i < 10);
来源：http://lq.shtwfgs.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://of.shxzskj.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ma.huixiangedu.cn

C#:   do { i++; } while (i < 10);
来源：http://cj.9csxet.cn

[B09] break 与 continue
来源：http://qo.shtwfgs.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vj.yuexingan06.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fu.panjiajie.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hr.yuexingan06.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://to.wgjwhj.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ha.nszjky.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dy.huanxung.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://by.szxytkj.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rp.colortex.cn

[B10] 遍历同时拿索引
来源：http://qs.colortex.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://op.muxihuayi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ef.haigaiapp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ut.asd995.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://md.nicolike.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zl.521024.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hp.nicolike.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qt.huixiangedu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lg.wgjwhj.cn

[B11] 生成数字序列 / 区间
来源：http://um.szsharing.cn

Py:   list(range(0, 10, 2))
来源：http://zs.huixinmuqiang.cn

PHP:  range(0, 10, 2);
来源：http://zy.521024.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bi.huanxung.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rr.shxzskj.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gg.hahajie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ao.9csxet.cn

Ruby: (0...10).step(2).to_a
来源：http://hc.hnjuh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gr.muxihuayi.cn

[B12] 跳出多层循环
来源：http://mb.nicolike.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://oq.muxihuayi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://pg.9csxet.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ce.lnxyls.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dy.huixiangedu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qd.yuexingan06.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hr.shtwfgs.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wz.panjiajie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://io.gzmigu.cn

[B13] 判断是否为数字
来源：http://yb.huanxung.cn

Py:   isinstance(x, (int, float))
来源：http://pv.jianghongdianzi.cn

PHP:  is_numeric($x)
来源：http://wn.bjjhwx.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fs.jctech888.com.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://al.newstarts.cn

Java: x instanceof Number
来源：http://ns.nicolike.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lm.nszjky.cn

Ruby: x.is_a?(Numeric)
来源：http://hp.panjiajie.cn

C#:   x is int or double or decimal
来源：http://jg.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://ns.521024.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mt.huixinmuqiang.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://st.hnjuh.cn

JS:   [1, 2, 3].includes(x)
来源：http://oj.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://vd.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://st.chemitech.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oi.jctech888.com.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ni.huanxung.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cr.chemitech.net.cn

[B15] 布尔运算与取反
来源：http://dr.wgjwhj.cn

Py:   a and b or not c
来源：http://up.huanxung.cn

PHP:  $a && $b || !$c
来源：http://fz.lnxyls.cn

JS:   a && b || !c
来源：http://xd.haigaiapp.cn

TS:   a && b || !c
来源：http://cw.nicolike.cn

Java: a && b || !c
来源：http://fs.nszjky.cn

Go:   a && b || !c
来源：http://go.szxytkj.cn

Ruby: a && b || !c
来源：http://id.szsharing.cn

C#:   a && b || !c
来源：http://zs.chemitech.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zt.newstarts.cn

Py:   if not data: return
来源：http://ml.shxzukj.cn

PHP:  if (!$data) { return; }
来源：http://te.yuexingan06.cn

JS:   if (!data) return;
来源：http://bx.bjjhwx.cn

TS:   if (!data) return;
来源：http://zm.haigaiapp.cn

Java: if (data == null) return;
来源：http://fi.jianghongdianzi.cn

Go:   if data == nil { return }
来源：http://ta.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://vp.nicolike.cn

C#:   if (data == null) return;
来源：http://fq.jianghongdianzi.cn

================================================================================
来源：http://fc.jianghongdianzi.cn

C. 函数与作用域
来源：http://dg.jctech888.com.cn

================================================================================
来源：http://mh.nszjky.cn

[C01] 定义函数
来源：http://tr.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://mk.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sg.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://ok.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zn.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tq.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://op.szxytkj.cn

Ruby: def add(a, b); a + b; end
来源：http://ig.shxzukj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zw.lnxyls.cn

[C02] 默认参数
来源：http://jj.9csxet.cn

Py:   def greet(name="World"): return name
来源：http://kt.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zw.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://lv.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cn.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rz.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zw.newstarts.cn

Ruby: def greet(name = "World") = name
来源：http://mk.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://nb.nicolike.cn

[C03] 可变参数
来源：http://xu.szsharing.cn

Py:   def total(*args): return sum(args)
来源：http://fi.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vv.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gj.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qo.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ah.muxihuayi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nb.nszjky.cn


<!-- 参考信息 -->