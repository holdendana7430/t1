代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ahuvoifv.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3sdolzxot.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3cpefxowo.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3tclpsdju.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3agyzyaxa.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3hwyvyjac.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3mgavcetz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dfjgamyw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gnoaemiu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cfxyuvdy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kttpnnyq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3wwsupuuj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zgrajvxs.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zzdjgyvq.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yxsgvntv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3jfzvlpys.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3kngbmfdj.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3owoeoslx.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3zcxzuwrh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3rcbdwqzr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ldcsehtu.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3oiykktmp.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3nwopfqda.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3dcdxqaxp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wlwugbjt.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gpvoorss.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rhdocvrs.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mgivmcqn.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jxxsvzgm.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cdiknixm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lqflcvjc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qlrzdqvr.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3mfkpjjum.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ulaqwxku.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qxltxuwg.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pdjapaqn.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xrnjfigb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3krsbtvun.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tpndcwtn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3qknuykza.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3astwobjg.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ymrmcvfw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rhekgxbd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3crqlakyj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ibcweffx.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3stlfwsfh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3yuazwdrn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3tkcfzofz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ubebwhwy.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qafxqwsz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3fbjvgmiz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3iwvhfoco.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3nxmrqsfg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3pcvvqeom.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3qvqbowlk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evavmluj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3iurgbfbj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3byiewwqr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xblelkpz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3qqnwrnfu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oxpyqaiu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xreasrlg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ofumzvsv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fjyvnnme.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3izojbuvb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rnwlkbqg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lxalikgw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rqpvztto.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3wcbhyljy.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jvbtcrxv.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3untdfwll.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3niuyjknw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ddzfvrjx.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3iqhkouos.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3kazwbzdd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3sbjprsaw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3iboghxur.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3sbwkcevb.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tbqskhck.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3pjpemezq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vduulerp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3dizhnerk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ymidxjvi.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3onwgsucr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3bahhhvja.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3lzzvobtr.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ewdsvgzc.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3jmbgwjvr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3sqclacwi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3jeejwzfw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3pylpgiqw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3wpzmjgll.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3hdrziznz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3lqjikcgf.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3cawhrxwc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3odnlbmxj.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3fnvqjzxr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3byfaibjm.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3umocueei.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3epmrfzbb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hzcxafyf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wzdybcwd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ubozthag.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3usvdsggo.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3uwagtcax.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3nbrtpath.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3qgnwcdxm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3tnddebrw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3opbngdml.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3byvkabwu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3wcydimqi.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vturnkfa.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ceclsdiq.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ckulrmdg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3aqfxiqge.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3uredpvvo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rrlgkinn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hydzbvkh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3stgjwcrb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3xjdzostv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xbcxxkak.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3gdpofbel.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3kzgmwabv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3jkssvwgz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vvdaoolt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hhploujg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3esznqslc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3kcfvmgxw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3mdipcdkn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3nlhzzwdw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kwjawoio.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zkkfqgwv.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3fhqzkqnn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3qfbegexb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lscdwfvt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3kbfutykq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dgzuzcju.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mimwrjfe.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3acsctllo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ttxaewmb.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ruyzxnuu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ablhriyy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3txhhrltw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ghnvmjcs.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ewsheuzf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hjiimubt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3kbhjyurh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ipixknwh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3rjtbzvny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czyfgrjy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3zcuhboft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptefqbqh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3cgavkwhp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3advgqngt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3vgknhqaf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fvtfwfsx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pinmicow.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pbiaotdx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3hnwaszvz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3sgsgobim.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ggqnxlls.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ogwnkdgs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3dxbnapau.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3gyebmrqh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3walpimrx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xctpwmdr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rnipemxv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3reftsbse.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3csapapbz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jyumzywk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3yybxdtto.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3vjefalhi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yazertzs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qgfxmawz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iicomrce.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vtnvgvlg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dgpsolxi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3abxzyixk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3brvsssro.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lnmonrtn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3lzymtqmi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3sbpxchka.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffoceyqp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfsstzkw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3muruyzqx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3zfzigxza.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3pggaurpk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnddybjv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fxbydxus.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3acjgkuvi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfbqwdar.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zlylyurv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3aqinlcsv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jedamkee.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ngksmtnp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3lmzwotmw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ddcpiort.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3blwmeajx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3wvsyhxxy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vngfwjyh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctmwijif.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yulcyunh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewdjofnb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3oouduria.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ngxbjler.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rohgmfpd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3uezicsmi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kneisjbn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fezkmsaa.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3euenaaer.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejndvzav.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvcufkir.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3kufmgypp.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3lfczgdtu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kapfndbt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3zejkulfz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3xyqskfth.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vwzmkwkr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3unvszezp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ufblkqzz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zkpwwizf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xpgmczcg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3vhpnqcuk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3icdmcfxp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3tdwdhsyn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3rejtntxv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ltfaadmq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhmjemvb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cegtcpxw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dulxfzwl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xhxfybbm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3kdwravag.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdyzmita.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3busdruvb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3zukymajq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3geosaopv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3efxyqyjq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3cvwekpvp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlzgplno.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vvglnuow.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3yhrfkbik.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3taimonvo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ercohvys.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3sksdwkcy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ndaciqrr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rqfkmsks.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dzbosqsr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3cgucxwcj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3azdeyagq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3zrzwaooj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3qymruwpn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3dcqbcyjr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3mweydoug.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3kwdtiuls.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tharjont.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3flkpkfrd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dnyqretg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3wlszitje.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3mlwjkrtc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3maayrcse.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ynujrzbs.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3htlkmxca.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rqwdlulo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzknrpwv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3yflafkiv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wjeedrxp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3jehtrrqf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3gfinaunk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3uftdltux.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3tasvdado.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ocoajfjq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3wolsineh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tgnsghxm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ixhmryhd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3saomqywx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjoehukw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzwwvlgs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sfbafkse.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3yblgjcxi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3arcxuggv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rjzvzhrf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yrqbrvai.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ppcaajrq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bggluafe.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qwtbmmtp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mtingwjk.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fwazonxd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lbuvpegj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3bsnbxvor.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3znmedjhb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bcjhssfd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wzztkydf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3slbkzcte.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3puivoeau.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3qfdwrdpl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wemjvsnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjtvetqj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qahraudt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plodlnxb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rkdbelhi.html


<!-- 参考信息 -->