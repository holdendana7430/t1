代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ikqvtahs.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3gvpmzkrd.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3phuwseib.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ufrbebtq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3jxhojzil.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3boovujfy.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3kvmkktjo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3dmlxddai.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3easaqheo.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wjfqlmil.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gmrjffiv.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ucnoeuov.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pcsjzxci.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gktltxai.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hpmabqhi.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rurzndbd.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3voezlacu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3cqmobcys.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xpnqxvpb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jumdlqdt.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ndmznebh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3tahcpkpr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dubnafrt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3dvzcbpmy.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vntwykxl.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3kgowsjfy.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3dfbpkuzr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mbfjsxtt.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wmpfuxkm.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qoqpywtn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3pqbwqjum.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3fbicdzqz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pwkzjxaf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wpfaqlaq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3tvdcbgal.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3gkofruwb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3sisgjitn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3gfbmkknx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3xjpjtruf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3muvnlvwi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3yamcvjoj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3xasqgogy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mujrvnml.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3zfxtmpeo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ckvuukbs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rbdocjmr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dirqopcr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3thkvdjrf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3irtcutbv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hqqbmoqd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vnagoegu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ckjchnoe.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ezztzhan.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ibbidlbg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sqddvmiq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3umzeowbf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bsvbjhnb.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3xdvnflif.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3rympwqsk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3jtieraym.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ecqjkvry.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3tdfriveo.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ugrlrtfn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3tvbtqide.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xhqaqakz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3phisggos.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3xkwitmki.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nwdjccud.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rckmhzdr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3kmrkupzj.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3rroptadw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3pvkosfjf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3isjjertg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3eknmunvr.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3sawjjgua.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3xlgpwcrp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3lgjhryar.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3gupuldbx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3pumgbeqm.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3hxvrohts.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3wdvxwjkg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bharxdzx.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qgjzwkwc.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3srmmvmcp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3aerhlsyq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xewwbjxj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ztmslkuy.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ubqifywt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yocwnpiz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3djbpovon.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3kiegywgi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3astjsiym.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3rldfxhdg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yxpvhmvm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sxlgerzm.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rgewdxwp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ckjmeagd.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jprbbkgi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3alodrjzj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3shfotrdm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pwwfchza.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nglobmcb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qmvnrzxl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3oklydzwj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yvvsxefm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3mnvyrpvu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3yxfhljdr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3nvaczysu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3lebugqbv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ofzyhckl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rsftvisf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3cqcaaxri.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3urzqgoyc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3jugquucd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uzgnfeed.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3luserfuv.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3xiaawckq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mwwaaxma.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3nmdcjshf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nwduxpoh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qwyghswv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ilwkykgy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3fiknlrlk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3gukkvemp.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3jtqkofpq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3pqmcbtgp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3iagamryc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ozjccwsj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3drzkkdgd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3wmirkbsq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3lldxmync.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kldzukjf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3txchlssj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wcoxcjao.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3uupzfnby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pzduxlcf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ebedhjok.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nvdbkoib.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikkdtazq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zsmvxadg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yuamscvb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dcskzmiq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ssjidmno.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3nwbvgemx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dkstwnam.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3rvviojoj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3xrijfqmb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsldrqur.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zodjewle.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qlhsadyv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lfzrkqvo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3itguopwm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qomznpff.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sqlbiaha.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3gpntzqqe.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3nibwhyiz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3umpuvohk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yyjoceru.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mvjitrqw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3myceqbnz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tvykilvi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3cztaakyz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3orshevpc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3uugfjuoj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3alykurls.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3eonngwmm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgjkordg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3whgxbkqh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyrthydy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ugxwrmfz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hkgulkie.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfxashtj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gsnbaazu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3didauaro.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ybtpmnxd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mmgmzgsb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3osmxjllk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgklcknx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3qzrgunal.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ymisgwpm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojkvwrsw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3bhjtlcxj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3yprlqmey.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3hftwkhvm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ivubotvw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdmqkmvc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3htcigkbv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3cfkeletf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3utqggpqt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnxotczb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3khaltfqg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3rlvzbwds.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvzrhypz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wizgwwks.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ibmhalfr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkcljlql.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3gipawjea.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3apobxqst.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xomgdtoe.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vdfrfzfq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3cidifxoh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ugfwsrgk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vqpknoce.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3irbvpzub.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zofbbkli.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wbiitmmb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3pxemhyxd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bwwlzsxj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3zvinpejh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3gxtvemav.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cziuqsvp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncnenkpn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yqhmwdlz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jmlxpsul.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ktdlunct.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3heezatwa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpuduqyf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3btdsmaql.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3hclxynms.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3qlrgtago.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3yvenxvwc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pozwcesd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3iiybqmnv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ddnitnnx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3rucwehgw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3qgfrbhpj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3whtpgtfo.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xkizdxjm.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3uxcmziut.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ifidxmqk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mroyycwa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zjxwufdf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3bqqlqddy.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zzabzapz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3unuodsqg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3engotbmv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3rwryitwh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3lwsviqox.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qkspahqm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aytdvsgm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3klkmlyuj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3dlzdchmw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3lylmkktn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3xfqeeesm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3plddtezd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3thgmowbl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjtblocl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qhrnnzho.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ujvvksua.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3lngxbhee.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3cenjaasi.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3navlanli.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3wqggjscb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3lmxatiaf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3kwypjvci.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3mfchujrz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ndmdsnal.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcghdtky.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qtckcvtf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yrrlboif.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cxnedebl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mdevokyh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3sgmslyjm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3dpnjpmyh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3hxyzjkgq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ewlmbgae.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wdivcicd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zqvxkpij.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3khkvbxjc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uxefrcyc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wcfiubtj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jwdzmwrw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3nufabcit.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdwunjea.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kfzynfdn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mggwhpne.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tqrukljw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ftrmpmdo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3brclgegc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cgvurmkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcxwhziv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mzzwhlfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzgcrgcw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qkmedlek.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wfgmggio.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkyciueq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yuyhdajk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xakavlqm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3arpkbhvc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3frsraowx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3npumzwop.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kuwdhffg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3alrzymiw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3kigaxpdn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3famjmxzw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gadabrtf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xjllbkjp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3kqgixvfj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ewshpgar.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3uwbdfzxe.html


<!-- 参考信息 -->