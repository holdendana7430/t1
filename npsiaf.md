代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gkfkjhwf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2uypmvfzr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2oihkyout.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ibhxfwkw.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2xposegnw.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2okylueea.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2tmskomss.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2boblzkku.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xhjxzzyj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2enbxydkf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2aimjnphy.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2rbdcvdlx.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2lvxqwvjr.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ellaxgbe.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2mdfpwsfa.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2foukkiuz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jqlrhwhe.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dkbbtrbo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yxylhtvm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2fldskacd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2accesspg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bdahynwb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wvpjxrvz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2xhycgdoj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2wxaiuchh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2fpsdjtpf.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2qktpvzna.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pvhmxszq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2kwgecder.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2yymxhrhh.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2jlcrjimb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2kjujzarf.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wpfxnuvw.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rzelhoto.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2crateqmy.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lxclkbhk.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aysnaewi.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lunlzdam.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xhqgpetm.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vbnqxsbv.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2wfzuhvkt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2liztazzl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kkqiqqtk.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ysjzmfpw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fumacudh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2lgohhlpb.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cqijoypd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ggpsbymd.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kerhvuky.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2evtxuzfo.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xobwtzha.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2eczylmwz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bdddslgj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bmnhoctg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2tquzhijf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2wtfllanu.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zgqymfii.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ixvxvork.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2pykiklgc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pjffmntp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2bepkrnfa.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2nnchjasj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2kkxeqkpk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2uengmyzp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2kjepdwzz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rtfuccwa.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2brjxnkmy.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2cirtktpx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ggtffjth.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mukombul.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2misertzp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2unbdzhin.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jjctbsva.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zzyijhnw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2geasjaoa.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2klqkhupc.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2yuctoqzj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ertobujj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2vbgophro.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2orthghvz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2huzitknu.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2twwccahe.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ckjfsdss.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2mkaxhqui.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2aifkepwi.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2bycvxqzj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ujaxdsdh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2throjomo.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2yqjphluh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wwegrjjq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2cdypxnhk.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cvtscyrk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wolpxnnt.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2zlxsjcwq.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2bcszdvyk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2fuegicdv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2jbfxgsbp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2pvpkvsxw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mfofpykq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2wbmnjyyk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2prfvsfjt.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2jnmbesdb.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2xlnpxrmm.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2xzxgpage.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2kvlwyumx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yirprrid.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nvgrtrvf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ivabigdf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ihsumtii.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ckjqbokr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2aervawnj.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2gcyfrfke.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nedgshnu.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ihgnisys.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2fildavdk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2udhydobi.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2xufgqqlq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2dzmaaeis.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2cixrzcia.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oubkdbnq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dixcuayp.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2klutvcbs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2eokncwir.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2weinprze.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2folhzwgw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pcseefxe.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xahekgyv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ozjgfbcg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2smgfeari.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2yihtkmkj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2jycniygq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2dpqztbjf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ipxspgyk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lmutuxxz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fatwseex.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2eyltbpmz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvregxza.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2mjmxuzmw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jxkgxtfd.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xskctsyz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2xzokcrue.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2tdnhqkwa.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2uhckhlmf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rfsygshm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ejjovqwq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lgbprumr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2gfxetxgh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qybbcsup.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ajuxuxrb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2glcrgqnq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2udridbzv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2sdieeabl.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2osetmnto.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xogkeqfi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ovwblljo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bxhftykm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pddbmzjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucxzfwsa.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2hzvaeisj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdjcqkpf.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2uonblldh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2chywwywr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yptxrxtk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jsymxabs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bnuaurtl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vuhaqnzs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2crswlkjn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2zvruncqw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mbmoqvnb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2qvlvulyq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2dsganwlp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjovyjmw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ffourtdd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nexbjago.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xvjqxxwl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rgqpztdg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vzitbgao.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qicfagsb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2qbetiytx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2fvxarftr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ivjfyqlz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlqzixwv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lssilwjr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yhquxize.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pigcyqar.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2oyibykry.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lbpxmedz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cqncomsx.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xpjwhnqy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvcqydnj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqlrqkgh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kudivcek.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zcxgsssw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2mukvaotx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ajjmwsaw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ettpvvfw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2upihtnfz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ryeolqcn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2tulfqszk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhhdxrzt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ujpxqlsp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2usxejlrm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2vbgmrlks.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2aemcxurw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2pklttmld.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zcxoervo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xpffhsfx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2gcofivys.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rmljqcue.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjuxxsga.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdlrsgpk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2vzmddxfq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2caekpctc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2hxwxlaji.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2kpximnup.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ounfstkf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2drufzlba.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxehczvq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2myybspuo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qcypbcov.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2eyfskhfu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2fzkhwlzl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2okicrwpk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2hzfdjotb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2moropcwi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xtdksuii.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2csnipcab.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cpwjsefr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ajbcauht.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zpjdehte.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2tsearxqo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mpaueqcq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2bybabqxh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2vqobxmur.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wgadotjw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2twmdrwgp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqvszsbo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnthoqby.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dzfyuypr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2citovwsp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvpjhgeg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2oorliosg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ewsccmyk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2verbxilb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dnqmgufg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2etruzuzq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncakxkpn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2huqvidko.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dqgjdzdf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2cjisnmqv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2bhoiyvhq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2bgxqejbw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2uvhrwkqs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zxkmzsqw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2iwrjfphp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2wddzuosn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2lfgnmtzl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2whpncynl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2twnmefow.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bexkyudw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fahbmzpi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2abtvgqbf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2sehjgycx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mphlgvle.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2acsnlitt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2kowzrlvr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2yqwcrqsc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2khovpbhm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2rmcntubo.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2klforbin.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2wjsjaudf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ewuebhiq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2idzqadnn.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2cpnvnonc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2tewvxtwc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2mejvxlmz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2pspgmqoy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2dlzyapsn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jxcrurop.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2hwzqeeux.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vqmbafnh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pkfebsqj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kwqwjspj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2hnbcbvvq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dnjmlpbw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2frubgeir.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2nkvjftlr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gkmvtwrt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2bxccaujq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rtdvving.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hfhpcnun.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jmenafku.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2imlwqxgl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tvmmmcia.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jjfozaxw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2afuekyvc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ozcyoxjv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2vcudzxwj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gihzhiim.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2okaljohr.html


<!-- 参考信息 -->