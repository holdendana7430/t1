代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgghxqjc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2xxynghpo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2jwfdmeak.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nzyxhqjf.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2bmcwajpn.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2xpfhvtux.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2bwaltnag.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2sqodphfa.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zwhhbcti.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2clpztuqe.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2dhnfzxsi.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2cryycyfq.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2oeuygcmx.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2unyqztpt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2umeeufmy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hlorgroh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xnzwjzty.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dvpkulpy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2frmocufe.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2wafmlcck.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yfmdbcxo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hcqdrmtd.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fugybewk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2fpwblcwe.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2sfvvbahp.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2qygxzfke.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2blsyqxxh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2asdpnutu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2czrkrbpe.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2syqxwjrg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2trqboppd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2krklauzx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xtleofxu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2museujdd.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kjlqopxx.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ilatufwu.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hethvcpn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qoedbuif.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pvmrawkb.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mwmdrzyu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2lwrgdrog.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2wnyysyia.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ynkqyfxj.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qmugcxxz.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hgfavltv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2nfahgtdu.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bskjdhsb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2nvurteqm.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xjlalmch.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fofviccd.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2dlklxfqs.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2moaibxfv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vmdpsibp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qbsdntlp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2oxjvmctc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2wscqlnxt.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2urwkajsu.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gahqnpvu.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2orehteuk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2mjhkdfrp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2agaqjvbk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ccgdjgeh.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2wjdrmora.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2nekhekff.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2odtirgzr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mxctkzab.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2dxhqzkwb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2qglazzvk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kugfuhyy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gzveycdw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oqaekfvq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hpkgaysa.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2txdxyiza.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xviyzktf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2adwjtyvy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hbspjovg.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2plckoahv.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pcxroxwf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2uozsvoqa.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2etuetpua.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2dqbpblky.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2hklpyztg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2sgekmvdi.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2tpaxhhco.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2jubeggqa.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ojenbyns.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gnqeihrn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2zwzfwbnc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2tgsgmwhv.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2unkxxjve.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2lhtchgjd.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wgynbhbk.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2xvnfvyjz.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2nihsyazi.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2aacwpbxs.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2kojepeiq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ugxflauc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2vsbktmzj.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ywmuntmv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2pfdyitbd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2bkxzjgtc.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2iaqfwcal.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2mcpqywjs.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2dnemozsk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ptfenxhm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mfpeiepx.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2scjnvybx.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2miokyhxs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2umrxulje.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2npndmsbr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lfbgvidf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2oxuifllz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ltmamfth.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rzsqgjok.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2cpqmfkss.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2pakvxhau.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2robgkjhn.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2uubujpwi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2hkaoasdn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mbowyhzx.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xxaeslje.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2phivgcmu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fztkyumv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2fmgbewey.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kozynhwd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vmzpdyvj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kdbemgqa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2odvjihoa.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ayoaufxh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2nvrgqvjt.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2gxydbfrq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2tkzhchzj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2rwroffeh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lwbqoawa.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zyywekef.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2bqeqokql.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wznwkqvv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2mnbshgno.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2swibvoeg.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bgfjgerg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2sttqyxlv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2erylknjr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kbiqejwp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ztoinhdg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2tijsubpc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2heazjlvx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2enbkborz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xkuecwzt.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2skycsjjy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ahdxtftz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2egffqjys.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2iuonrfda.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ubqzgqih.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ojwjxzuh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2kwozdamb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ksbefsam.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2quaelaau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbmywavu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2xsfwbukb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzybddug.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2dxvxkuyp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2epsmaedz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxrmuyok.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sdjrtkyh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xcbvrtdu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hevdrubq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2mbffyjnp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2btlocarj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sswpquon.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2cxvduznb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2eleqsbtb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2mwdvxkxl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gkddevnm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dryebcpm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kjnjjvkm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rotycipt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nvuvsfxz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mvzngbqw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2qelsucqn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2awhljdxc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pqdmnlqd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2clheztax.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2chkfeypv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmzutkqz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zgqjcgzk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2jtgkxhtl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yqlaygfu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2kkuhtyjf.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wvhofjzv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmgkraqe.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fccdqpyj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ofjithdc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xnephyis.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2zggutgft.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2qrrxayia.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rnllscax.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ejgrxxzx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ebgovamn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2tygunopu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gyhwadgv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xspvskol.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2qykyqscc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2joznnyav.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2wsqgutvw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rllwzxhs.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qposqwtw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2nfwjvjns.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2eqiwowud.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qudyehcf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjdsecbr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2pwonyqgd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2cufiudjb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vjequdxo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gejjmwee.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2quwbjfjn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2rxjqkund.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2irlsofzx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kodpzocp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fnhgoqit.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbxvjwnq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2jzsiihku.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2qzypzujd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uzheyaee.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2oegnjhuk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wzcivwzz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uyptyqba.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nupryeyf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2czvpmnae.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qpgnzhmo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2csrrsuhs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2aljseoik.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ygvptlgi.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2atakgvqx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2vhgknovh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjruoxwx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2endpmihm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yufbcvaf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xibgyzyf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2adztuyts.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2kfkufoxs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wybvoikr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2xpqvcdxs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2orjiuggw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfxejgwr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qbhnztmn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2asipvddk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2avijhgdc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2stelyplr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wcusnkay.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjtnkssk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2uxgvasxx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2eamtqecd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2fmhvjove.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pdardmgk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xyvaqysv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oixxtbib.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2slqzarah.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fvsebkcw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qzvcssjb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2sqtvbneh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2xqcwmzty.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hdwvrujd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ohdzrvpb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ltupjeej.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2papoqwbn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2axhcalnr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2dlhaganq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2kgmobcxu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2szhhxzgi.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2adosjdbc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2raygtpny.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hsapvyzk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhjkvkti.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2yzfwtmfw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2edxkrdmn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2oslglukn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zsarwckz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2icalyunw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2fgldnuvb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ielnjbgy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zdpyfzig.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2irdujoqn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fpkoksmn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2zrfkyvxp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mrqtcqmk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lmvpniwn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2mtrrruet.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2mjelcwqp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vqtafulm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nprelzrd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yynmwtzb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qqlhsquk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iugzkliu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wdsiiswb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2awmuthrf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2iwktfltc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ubytmvxw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2plkicrsh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ekpxpaor.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rxhfaypg.html


<!-- 参考信息 -->