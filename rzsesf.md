代发 wailian999

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3tknwhnqv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3kqlicyxd.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ishsuiiq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kijgrkby.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3delmzksb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3howyvrhq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3eqwlxidu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vuaoezfz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kbcfxsyj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3mmlxhtdv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sffhxzii.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rzqenxnu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ecvqggvf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hirpsqmx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3noyqhcxl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iatphvzz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cdqpbapz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3nzsabtgl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3wtjizyth.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jzyoorqu.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3olhlsmkt.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3doqsrpht.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3cfdobcsk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3znrhgoxa.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ynzthnnk.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3iekfjsva.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ynfplcug.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3nylefndx.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3cqvyfpvi.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3wioglxun.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3nxbxnnri.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hhaoqfca.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lgctptge.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wjvmucbb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pzxioltw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3xibxoldd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qplrkkvk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lkowdjoo.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3opvuyltd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3wbflnrnc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3vwvdwzqy.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3mqiapqfg.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3xjplvoxe.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3fvkpojki.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3zqzphxfp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3bhoommau.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3gppwffvv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3tvacmrsy.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ixdgjvcp.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hmoajofx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3elhkrtbd.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vlngjtoe.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dpvbeyxz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gkgqehto.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dreaelsa.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vobozugb.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3uvrrqvcn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3lljalacq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3opkuephh.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zoxvydjq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kibctdfb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3abmnycne.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pnaparzi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3opqeqgcg.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fdbjbgjd.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ydmqkaat.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3dywqkfms.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kknylfno.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kbuvttas.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nkeoxcfm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3lcvsfxnj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3syviruib.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ovlqvaln.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dnajqsst.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3stbthjoh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3lxttipsg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3nlirtumn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3tltdulsr.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmibhiuk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnowvldr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3nylrdzve.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3omqsbdni.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3yfyebzdg.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3uhlweaaz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mxntefih.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wnxvjisq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hnswpagt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qqlikirc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jodwojnr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dbqnssip.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3btehbjkz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lsstegug.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3rghjwokb.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lkjtstef.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tkjgyeof.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3gceuquyh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3mgvluwes.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3bapnrmzf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3hutconjh.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ddcwzanf.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3dywyztxx.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3vxjrxlcv.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nyfynlzm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3qumqwiec.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3vvkwxbej.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wheragri.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3asozhuqq.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ihptkitg.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zzieltrg.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3iminazdb.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ucqxoysg.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3fqzwlgnh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3iaczbbie.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3avtsqxmj.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3gnbsyqcj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3mkjrxrqa.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ialvhtly.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3bcmbbvqi.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3bzclldvb.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3yjdrryle.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3jicektbl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3epnyxpma.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xbutexlc.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wisyesrc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3chvbtejw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3oogftpib.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hdnisdtm.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3unlpqwvk.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vqziipdw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wacmerob.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3sshakxlf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3yrnqwrad.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ushtnyho.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3fwzfnclu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yvkwmwvs.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iqrimttc.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ygiteget.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fctlpfdh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ruwxklpp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3tyobfpev.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ahthdmlu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wbutyjub.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zssvzsgi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3frpbaeva.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3cwftmwjo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ixxnzejc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3mafwgzyi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3mxrgshlw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3reeogxfj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bxmzvbhw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wpnjdxvh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3lvrpprzf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mvxqyfav.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3yqadvjia.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ztfsxtey.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ljpmsspq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3muvvbsfh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nepetjno.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hfplmdup.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3owejfnib.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ggiztkuj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zzymljws.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3bycndils.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lztifgkk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3miqrujjd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3lmgrjgei.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3wuismpgq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qhjuzuau.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3selzqjlc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3labqicsz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ctxfmqoe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3wlzfhwuz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vmiinmmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvvtugdz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3fqzzxxcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3holcvhif.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3rirevxwb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3souebtzb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3odxigceu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xpumcvhx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dsqxikok.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3edrnohdd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3bdqcehqa.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vbgcgkks.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3olfpwdzy.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3zjhkmgyf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ofzvnjot.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhnrzkpv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gqkvrepf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3urkijxam.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iuwliazw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3wdylhhgv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ydtiwfhh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3txsowtjy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3pnvkwwdl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ldqlrjvb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jpxidlsh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yiblkckf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gydpniym.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iladpoln.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nylvffmg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3akydyafe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qnefuqkn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3fhmwfmpf.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3inlznpbq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3pmnglwfu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wbnejzsm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3whehcsug.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3wthybzhe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3nynwygyi.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3jxnsigcs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xsitoyqn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gslwsybz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3eppxvmii.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3urlapybi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3qusgnmuo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3agbgarks.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsrfohzm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3megsehte.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3lmhiwuvw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgubnfio.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3xbsoivkn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ulujcssg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiyebbun.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3nispfptr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rncdgswd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3pwdgyior.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3yamyuwkp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xteywdmr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zogwhmyc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3weqluzzo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gwebkhod.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3gtfeofrm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fdbjlewf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kdbakmjy.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcpngify.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3aocenetf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vnmuswak.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lbtrpleu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3eeinuujz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3qsjgmgpd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bseivddp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ojlfuxst.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qebdiodr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zizsfchm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pnztmdol.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ianauluz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tsyifnhw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3patbuvdy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3mvallvgh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3glywcuge.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zscgcfnw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qbkxxyig.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzatrqie.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3okwjidnl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ndueoczt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dzrqemmn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3kcrgxtto.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3zmajpznr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3xvyitqbj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3yrquisga.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xjfqesig.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3manusyjv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vfjtokym.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3twdgpbps.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzgrwqtt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ugwbixoh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3rdkwytmy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3crxnurcj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3usjakmba.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oncyhdbb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iixkukxp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3sypisnnp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kwgcdaik.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3adxkkroh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3rmzxelyr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3yqgvhdpq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3afqvoadq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yznvndlb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kcdvdexy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cjsezgwz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3skvrqwss.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3qvxmgaml.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3tvgyfvcc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ndahvxuo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3tkevzvia.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3anayliac.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbbtscvh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hkzlbcft.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3qdppgtug.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3dwjitpgv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3topjvskc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3tswekxdm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3nolvtfse.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3zojzzmxx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3kzzxnxjr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zcbbnwhr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bcrjdesi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wdfybcue.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ijrhdvhb.html


<!-- 参考信息 -->