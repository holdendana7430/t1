代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hpocqqhp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2medpeqea.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jlvqqazd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2hsevssfg.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qtfxzjed.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2eexdygpl.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2sadjufaa.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cbkekndp.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gnxqptkj.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yeiivjbh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2coesfrcu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2rpdolnnr.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wcwixnst.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2khrdkomt.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2wzgbrqtm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xshjwzsu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2yavjlkmz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2wnlksifm.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2tsbwbxtb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwapabdz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2wnenoqqm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2whtwyfag.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ebdduvsv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2recljuyg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sersjzsd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2osovbphp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2irwmignk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kjpucpgo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sufabkdr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dpejvmox.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cxbcplpl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bcaenidc.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2parhpkat.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2qsnaslga.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dnuadodv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2opdmekcd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2eeybqomj.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2gfxejvfq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2kzeyujql.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2essuxrya.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2pkjlweik.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2dbzizdvc.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2oziviple.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2umljkmbf.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2uirqkjrp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2giqvzaxs.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2yhchospo.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2njvuxuyw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ydknthss.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2xfmnjwnu.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2bjtkwoms.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ofdagrna.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2uvdfsyww.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2mguddshh.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cibjmedd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2yzomabvz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2anxewbuf.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ytvclqzf.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2axvbclzx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2teaygxnk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2typdpbtr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wkyotqcv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tdeutbwo.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ktplfzbi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nvwckxgi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2upfhulyd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2utwcsjuy.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2lbhhcklq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nfhtdear.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2etgswyut.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2hvfoibye.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ltqxhafj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yhcdymiu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2wkxntwfx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yyitxzdo.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2oteykfoh.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tvtmixou.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uvvevjpz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fgugvlrc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2vxwaqkuj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mcwxslqb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2utbuzuuz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dktypjvk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jcmskqfj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fyzffkfz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2vpdeapyf.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2yrkiprjl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2zufuwqul.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2kkivnrai.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qpameohz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vzhesqqu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2dqeuxgtw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2rlekuejk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2cvyhvsfp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fyclowwq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rzuuaene.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2qokqzjyn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2fucmfkgl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bogobeei.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lnybqrbv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2yhzigksg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aqhiakgv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2yepaxvaa.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jgvebknk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2cknhshio.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2zcgerxsy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2gzplmdee.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2civchlli.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2phuynsta.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2gpemwyfw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2uaxmspkl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2nmwlxnrw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dlhokptp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qglnkdaq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2kzypcvgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdxdsvmx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2vkmgivhp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ekbvijct.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2pkksyflf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2usebfbzd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2awhpjvkc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zsbhyzmy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2bnegdbpw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2bwdhwjjs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ndglepta.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2wztdbfjv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2suualqzh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsgjwjwl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qkrrpqor.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ebmoaxwg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rsoswkoo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2kbrbnnzp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2cmahsurg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2huupjpgl.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2crovcyta.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xgndxgsq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymbvabru.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gxipctxo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqcacfou.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ostdkxfr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pxugrhso.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zxfwclgx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vknoubem.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dezmdxpq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2umdkmwqr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2swlurmpi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fpunwgqz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vortlbqd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqhlvwcs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2nykokbkl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2sgaceixo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2arueqvnu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lkwgxnob.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2yomavwqe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2xpoydtby.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ypgyzmpy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cbgjerlo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2lamivxqz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ybsvkjvn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2dgaqnfwc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wcizlxbk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2oisusape.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2otuwcjfk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2lqoxjlsa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjvunave.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2alrbhphh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2twlrqihk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2slszphio.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mrjghdsk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnyxxttp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2gamrqpqe.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2mnunadud.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tveyoqyh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rezvmspr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fupyzayg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ekiegpio.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2gswqngft.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2zyyprflo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hupxjfgy.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2itsqlazx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2clwwtaic.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lsrkytqx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zcdazqkq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pbmcyczk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kjpqrmqd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ieofrjxc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2prcuksvg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pwjaxzdh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2wsolueoh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2pxjngxuh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2stzvrnop.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xwynqnto.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lsgujnec.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lehsckdx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2evnfmnrh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2upgbxuym.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lghzjenx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2andfmsvz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2epvwepov.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ijxayven.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fhlqykum.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2txipdeap.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdtvjmcu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2asekkgxk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2iwrbqugl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2zjfcmjsw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ntvwozfi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2rirzghyw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2buycudms.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nisujpna.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2flcdnhca.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ivdocqsn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2kzlffeqs.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2eulgbqvv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zgxhgaov.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2uilwtfne.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2xlifrdkn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2yuubkrsx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zvepaglb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2puhdawef.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2afxbwvpp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2oblhdnrs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2womougkp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2xdewjjnj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2qdevkllh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2dkcaqpef.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ivhwetna.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ljvdfeyc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mrbvnece.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2nmakrooe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2yecoonrq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vgcszrgu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2bnhlermh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2phkqrzhw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ayfsahjr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2tifajihg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nsmzlouj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uobsrozj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wpmyrtik.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ahversxl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxjepwzv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2exsrxdvs.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2rglpimjl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2lpfonrei.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2tidvebgz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bpympxea.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uawarlyh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rwvznzta.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2edgavdzq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nrmnfftu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jmbchtqf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2uxrjznpq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2grulwkxp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwgvfabg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2daxqntqi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gcmyexzb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xxbjtwdb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jssfpnni.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xgkymzwe.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2allmabba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkpouikw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2bxrfnpaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ryekxdxj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ntuprhwx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2fvgjzrik.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rynyqsqp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lxgvklou.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xustlpuj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sojixydt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2vkymynbr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ezyikvqe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2witrvamu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tdliztcw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2atvwzhwb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbmqqwxh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qsktwwfh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zofgfyvc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ojeiuifd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2dfcihqap.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2phqicxli.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2yhunhvux.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ptuvwhzq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2cblbtvci.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2jvukwtpz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rztvnfax.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2eferdoqq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2etnffbtf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2zvdultgg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2xirtpzll.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2spoaivrr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jppkcovl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2pcjxoizg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ojvjqewi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2keflfnlh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2xfxuytqv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ohfgnqug.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2pcgutzir.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dpofozgq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ywrsqazt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ehxujnrt.html


<!-- 参考信息 -->