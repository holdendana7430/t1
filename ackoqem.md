代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gucftvtgm.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gyfgwlbcc.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/ghdzaapfy.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gxivhdrgf.sHtML

Java: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/grluoprsa.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gdzdyfhug.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gxevujhbt.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/glcbooqma.sHtML

[A14] 注释写法
来源：http://m.share.fehbvm.com/Article/details/gvqcujhlx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.zdbjq.cn/Article/details/gdeyxxrwx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gedvexgrw.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gioppvhfa.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gtjtjbyxc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/gsnpaqryv.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gkdnltagb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fehbvm.com/Article/details/gxyqgquhx.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gfmywtepm.sHtML

[A15] 空值判断与默认值
来源：http://wap.fehbvm.com/Article/details/gbtzhnaok.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/gunbuasxc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gxltgqkwm.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/ggryoxqes.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gvwsxzwzk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.zdbjq.cn/Article/details/glanagmgx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.zdbjq.cn/Article/details/gsgkwlchz.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fehbvm.com/Article/details/gzxlsrjup.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gtyfcvucu.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fehbvm.com/Article/details/gmfnuogyj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.hesvh.cn/Article/details/grksonyal.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.hesvh.cn/Article/details/gqoavrmys.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.zdbjq.cn/Article/details/gontozqsw.sHtML

TS:   if (!x) {}
来源：http://www.share.fehbvm.com/Article/details/gdgpmlpqm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.hesvh.cn/Article/details/gyjyuhopy.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.zdbjq.cn/Article/details/goercuacm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.hesvh.cn/Article/details/grzhzoaay.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.hesvh.cn/Article/details/gwighasmx.sHtML

[A17] 位运算
来源：http://www.blog.zdbjq.cn/Article/details/ggnwjbwrj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gjoqyrpbn.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.hesvh.cn/Article/details/gnecfelpz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gfqnjocdh.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gqeiownip.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gpqcpjuhd.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gkmunnlom.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gjiydilqi.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gyhhotwwq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.fehbvm.com/Article/details/gjkivycgn.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gbsfycwlo.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gmijskygf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/gnqlidobz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gjaxvufzw.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.hesvh.cn/Article/details/gnamrvzbj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.hesvh.cn/Article/details/goptpzfmx.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fehbvm.com/Article/details/gzsqzksnd.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.zdbjq.cn/Article/details/gbktnloef.sHtML

[A19] 交换两个变量
来源：http://www.m.share.hesvh.cn/Article/details/gghnbrocw.sHtML

Py:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gnwbqpyvn.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.hesvh.cn/Article/details/gciiibtqa.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.hesvh.cn/Article/details/guancbzdh.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gleulquyw.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.zdbjq.cn/Article/details/gtprcfylu.sHtML

Go:   a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/gbhmcuouy.sHtML

Ruby: a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gasgkinut.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.zdbjq.cn/Article/details/giaxvmhyh.sHtML

[A20] 读取标准输入
来源：http://mobile.fehbvm.com/Article/details/geirelndx.sHtML

Py:   name = input("请输入：")
来源：http://read.share.zdbjq.cn/Article/details/gbphumayh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.hesvh.cn/Article/details/gbmfikgww.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.zdbjq.cn/Article/details/gvsirifen.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.zdbjq.cn/Article/details/gnwoqujbv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fehbvm.com/Article/details/gchdteyhu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.hesvh.cn/Article/details/gcjfspjet.sHtML

Ruby: gets.chomp
来源：http://www.blog.hesvh.cn/Article/details/gtnsxnfeq.sHtML

C#:   Console.ReadLine();
来源：http://baike.fehbvm.com/Article/details/ghprsvioj.sHtML

[A21] 保留指定小数位输出
来源：http://baike.zdbjq.cn/Article/details/gksnyvnep.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.zdbjq.cn/Article/details/gjmzuwpjz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gtpxmuqjb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/ggpqoslje.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gtisdfcpw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/goikevdyn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gwnrtybxn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjxnkvrr.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fehbvm.com/Article/details/gjfolftcw.sHtML

[A22] 获取字符串长度
来源：http://blog.fehbvm.com/Article/details/gzxutzruh.sHtML

Py:   len(s)
来源：http://mobile.hesvh.cn/Article/details/gembmaiiu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.fehbvm.com/Article/details/gbsjwuynd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.zdbjq.cn/Article/details/gzkblovhh.sHtML

TS:   s.length
来源：http://baike.fehbvm.com/Article/details/gqycttyck.sHtML

Java: s.length()
来源：http://wap.zdbjq.cn/Article/details/geeywdrvc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.zdbjq.cn/Article/details/gxkuudnls.sHtML

Ruby: s.length
来源：http://baike.zdbjq.cn/Article/details/gdcnzhawq.sHtML

C#:   s.Length
来源：http://m.share.hesvh.cn/Article/details/gzqdeoyoe.sHtML

[A23] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gswgtyutd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.zdbjq.cn/Article/details/gplxsngsi.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fehbvm.com/Article/details/gthqdgefk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gbvndzfhp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gufvudnwt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/gxjnrwxsi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fehbvm.com/Article/details/gvlfamfue.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gptaiyhlh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.hesvh.cn/Article/details/gjzkqyzbl.sHtML

[A24] 去除首尾空白
来源：http://read.share.fehbvm.com/Article/details/gpskrnvrc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.hesvh.cn/Article/details/gxkgdleda.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fehbvm.com/Article/details/gagyjoobq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gakrrckdg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gbtpwjkph.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.zdbjq.cn/Article/details/gzxwbwwgh.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.zdbjq.cn/Article/details/gakszkebp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.zdbjq.cn/Article/details/gyutehskp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/gzvyfnfno.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gkjiprfdw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.zdbjq.cn/Article/details/gvxhqfblo.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fehbvm.com/Article/details/gmuylsxgn.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/gtgoiswwf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/guxwivumw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.zdbjq.cn/Article/details/gqnhjkmtk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gutwivqlk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.zdbjq.cn/Article/details/gtfxpajne.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gpuhuwkpd.sHtML

[A26] 类型转换总览
来源：http://baike.zdbjq.cn/Article/details/gyyxqvhqq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.hesvh.cn/Article/details/gyuujubte.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.hesvh.cn/Article/details/gfjgqgtfj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.zdbjq.cn/Article/details/ggafjgeby.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/gtrbznpfe.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/gnqpskeme.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.zdbjq.cn/Article/details/gahrznvyf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.hesvh.cn/Article/details/gbpptmvwa.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.hesvh.cn/Article/details/gsejntlqi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdrciwgeb.sHtML

B. 流程控制
来源：http://wap.zdbjq.cn/Article/details/gufkyszgg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsrbfqrbx.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/gavegkubc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gowtuqgza.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gggmbsgxy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gdcqflfqy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gzgooavgq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gikusijzn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.hesvh.cn/Article/details/gtxixxqfv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.hesvh.cn/Article/details/gjyhlowgz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gxzmttpot.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.hesvh.cn/Article/details/gwmoksbgo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gbnxmmnnz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.zdbjq.cn/Article/details/gjxaxyttw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/ganaosiwb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gdjidgtjt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gcwaczzxw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.zdbjq.cn/Article/details/gnhitafoi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fehbvm.com/Article/details/gyamttwri.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gteglcnvd.sHtML

[B03] switch / match / case
来源：http://baike.fehbvm.com/Article/details/gfvnphmhs.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.hesvh.cn/Article/details/gyughmtgg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsqwibgac.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gixzbzipg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/grnlqqapd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmudpbtaz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.zdbjq.cn/Article/details/gvdjlgsyc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gjvqtyvwp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/gsawsifju.sHtML

[B04] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gvsjklkkc.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.hesvh.cn/Article/details/gdxaakiov.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.zdbjq.cn/Article/details/gynorqpwn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gjnqfuuoz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gwddfywrm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/gkubdliaz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/gfzhalyfq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fehbvm.com/Article/details/gxbaazbpq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fehbvm.com/Article/details/gdhgzeezd.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gcavhmcbg.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gbzgqkodb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/gyxxwaisu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gxxcskaxw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gsjhphept.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/gstnmbcvn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.hesvh.cn/Article/details/ggzrkhnuq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/gmfzlfuej.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gsjndfjqk.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.hesvh.cn/Article/details/gsqxxhhzk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.hesvh.cn/Article/details/gfysswlrz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fehbvm.com/Article/details/gzocqjelp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gvgakidpo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/grjxkskvv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/gdmrzcroe.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.zdbjq.cn/Article/details/gwmudbkkm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.hesvh.cn/Article/details/gttlzlqvw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.hesvh.cn/Article/details/gzztvrbiz.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gliajebyx.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.zdbjq.cn/Article/details/gatvcedue.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.hesvh.cn/Article/details/gbncfnmnf.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gsdleduxn.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gfkedlrxe.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gxngzprsx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/gkdwiodpk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gsdlrqolj.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gwfdnnzbf.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/gwmjsudnr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gsodntgiz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gynuuivbt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gqxakjjud.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gntjtmlui.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/ggecxvodh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/gmmreelfc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gzsqmjwhq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/glehlnsgb.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gayjuznfo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/guxrkives.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gutgfxogg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gasimakqm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gqptvadgq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gvivjfzlu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gpwemlukr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/geosekakd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gvplydrup.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gmbhvcdzg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gxvngxjet.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fehbvm.com/Article/details/gmozcraqu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/guekzbzjm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/garpcdbgx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/gldoeocoe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/ghfazgxfm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gqonrjohv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gwygqgjjt.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/girqyjziz.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gidudjuxe.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gusdpjtpb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gwligzjjc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gcywppikb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gsrjvklux.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/ggpfhttgt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gqjnojpmk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gjjqcgwfe.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gyhxybroy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gzmisnnqw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/gtwkgyilw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gvqsjagpa.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/grfxhuljt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/ggbnvmpta.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gosucepql.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gipgicxcw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gkirrlmdz.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gqtojzrju.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gdbxzsarg.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/glbumswvy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/giziebeey.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzetjhodu.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/geeoshfxu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gamxyppgq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gyxpugvtg.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gdzagdegm.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gsziqajei.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gplcjpfxr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gtrjdsneo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/ghywaokrw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gvdzlxqrf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gtdkaftng.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/gxjtbpxri.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gwozgfmqf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gdmujhbhv.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gktiqhjct.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/golhntffd.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gigsvinna.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/glyoxpixt.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gfwxymuzx.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gzgomjgai.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gkdwrqrjl.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gyctwmpfr.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gxayghsxa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gglekqmay.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/guodpxygw.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gwmzzjnld.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gblobnslf.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gcgyepfbe.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gofpougrk.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gihhcgpim.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gtwsviygf.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gqqieueaw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzzjcoubj.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/getueptwy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtukycocv.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gqwtrlrcl.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gsvasvxmp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gdkppcsxj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gpwrpiudr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/ghmvwzgyg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gnilcnyph.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gcxzydlni.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/genfqwwht.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ghwtuyexg.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/glceenbry.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gcvqrfrgf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gffobkxhe.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjlqwfvxw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gjtxnzxsz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gnxjafvvx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/ghaauzqob.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gzifuvpco.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gosrgxlxd.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gziqdnhuz.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/girnjedmu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gjwjlmeeg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gtdoydqxu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gzxinlmow.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gotwbufzg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gavgzpken.sHtML


<!-- 参考信息 -->