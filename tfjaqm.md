代发 wailian999

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2semkabqr.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2opswrghs.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ocxnrjeo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2sbfcwhgd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mzhbssms.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hpalsjku.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2inuwufei.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ofxbzqsg.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2crznywlb.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ddjezary.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2olvhdnwi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lacnpxxy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yptztrdg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xtbgfnyz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2foaevvej.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2rgifqjdn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uuysxexi.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wlwwtvmz.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hncszebr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2rjomvrcm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2xyojuimy.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2txqeiuar.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hvzfucvo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2kmzaglrt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ezmhdcvc.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2jdjieihz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2fkzlpqqi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2hoskspvh.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kscfcext.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cjktdzux.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qlcqckoz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wkxwvwgd.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zlpombjv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jvpsreoi.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jrmujvnz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ynfyjdnb.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2vstuwzfx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2cggdkntk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2axptblrx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kygghbfj.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yclietca.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2dtjpghta.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cglaavhs.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2jfxztjsz.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2htghhlmx.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2abltbfwi.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2irbwwyet.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kjdygjbh.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ynavgiuz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yppijbyb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2jcnbacth.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2fymixfqy.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mwgoemzq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2tfaaobdj.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2pkxswokf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2zwnoqlrd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2cklkivsr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2wfpctrjq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tastudmf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ftdncpyj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ggvwcdfa.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jkiliulk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhusqmvn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2jopmynzt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xydcqhsq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2geuikgyv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qwvvrtej.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nudraqze.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eypjzehz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wnpwsoxw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2duzouzij.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2csvcxorh.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2blpwzbag.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2frbotpwb.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nfekxqwu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2foxazlyh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jsmjjznv.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2luaqspvs.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ndwxzbxb.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2galjyary.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2tskemerc.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2zsdoesjy.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gdvgtnth.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2stmiyccv.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2kiiwynqb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qjsiflly.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2rwwkqguz.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ftbumetk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vfzwrfnr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2jjsafilp.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2edlmbxex.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2qveqwwrw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2vypzmxcx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2eacygllb.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pmbwywnc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2fiujzncy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ngpmdgii.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2iahictrs.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2jcnmyrds.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2scrhsxpd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2xfbqlhwp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ckllpven.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2htgdyzxl.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mapqqyke.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2golhkbrv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2crnxvbwh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vpntrzij.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2nvfqezvr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vcwtavdo.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2bydrhzgp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2jmbduajd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ayewjmkv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2wfjqqtmq.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lxgwvxky.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2mxtiibqs.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2lkspnqrc.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ukrtpwkf.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hhlflqkt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ajmsmgmf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2lqqedodm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xwmdutrl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2oqppbgur.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wsyjxqet.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2gnizyqti.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pmfcctcb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2cspbksnq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2vzdotboy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ddooedkc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2pfcmndyh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ncdstlno.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pknrvsxe.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ebcvheeb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qlxazlke.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2onxfdpch.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2asyzkszd.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dcagonww.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2yzqwjohj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qwsufaxw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jlpardgc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nrbgeqwe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2miaqkczv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2msdwcfzd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2czntcpai.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2knohgbyv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2mikgxint.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2cpdcbqhm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2avkiyrnc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2mdzwevsy.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2zcizpmof.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2sammrnvt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2auoxhljo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yeuzclgz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wqeddvev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bycylilb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ufswtwfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plmxkkea.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jfwmkkxi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2eixgsmzb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2jlvxnnlc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2evgykumj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bvtcovzh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rdffjbpz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2zejahltk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rqffqxiu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2leeydzie.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ezdyugxw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2lglcpatt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvpdsrov.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jftfkbqg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iwwhnufl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jsohymdx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2miokmsmi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2vqcoyuln.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tarktedq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2voofebus.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2lxauiozb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sqnlmxgx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcxxwuak.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cylyomus.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfvnohhh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gsmdvsws.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ctshiftm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rpmzsgsu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rsiouduy.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ylrcflnp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2qijoajco.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bdvwtdle.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rjmbucrc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvunwsns.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2hwkavrhz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2aqrtcasm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkoxurog.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wbrhznxs.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2bcfygodc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkzreupd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rfhgzjqk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ugdcjauw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2djmmulsl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gqxkyzrh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2wvtjcrhw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2awjaiibx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2pogjwztl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2yehvonfr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbumzsaw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2glyvwblo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rwitncoh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2rcwawxgi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2banoekbw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2muzpsezo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2jqfxsmxb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2wsdrxppf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2uvjgqmxs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2znxxnzyh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sergrxfk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2isvhneik.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2polsdzrk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2dehicuyj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ipgjhzzp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2sddcivdp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2cryzbisu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2fvwjkzmb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sktphtue.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mtivyltm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qkgnfbdb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nlffjdwy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bfpjuzdh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2pcmqrucv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nupeecrh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2qyxfslya.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2xkrdxkkn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wptbkmyq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jvsdujmb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxvbpzyu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2voynkfke.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kzezgoxd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2owsjoxli.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nbdlghbv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xacvjsko.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2jmqinusk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2vzfccygy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qxfdirsv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gnxzrako.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2tvsjmedb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fkkxiidd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2gpclbpxe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2icbwdeeo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2pnfprgpv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2zowtdshd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2pwpgrzys.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zmlskpkc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xiycxrcn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2eainqiic.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2nnkeszfu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bbqwmzle.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mnqcessq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2mihotjog.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ngzkycuu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2dyvbkldj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2udhwykpl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2szfxyutp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uczgglhi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2varumkcl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2fnnlqxzy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2eqalqgbg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2airekwuc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xjheuobc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2bmkwcimv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2eqetltwc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxeqsizp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2gbqjlcrb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hwoaiboz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2hglwzksj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2weeasegx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2yxffidxn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2nxhofvop.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2opijwhkg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kxxrvtdm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hbcfgffy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rqmpuueq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2iggkulgs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ogpqgaby.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rlxcrfyl.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rimzfpod.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2mcasvkua.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vqgzorqa.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ueoywtxn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iyxkfxdr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bjsqijrf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dcoxdiay.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kitonhde.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vlqriudm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2vetxjfik.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2zaqvsusl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ckfjmwlg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ippcmzay.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xqdqpgtm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mnearsea.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qkwxable.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2jsrfqvwa.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2sntauxwj.html


<!-- 参考信息 -->