代发 wailian999

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3bhnrcfhv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3awkfsmpb.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3tgavasdi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bnzxooop.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3scrlptbh.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3pngdwtey.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3sikyvdej.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3fnursbzv.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3cdyigcew.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3nuisyynh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3estgesxz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ctmwobgp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jbxpaydq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dzxqobay.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tzjcicnw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3xjgewisj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gcoyvfmt.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ypxzqmme.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dorkajqp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3cieibhte.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3dlohaiqt.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3zzmrkkkv.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ktbkkfnm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3pxpaukzn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ubhmxcqp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3cechutfc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3hogekreu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3cokjpriy.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3syqpvbcy.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eapygfyt.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vbeifmse.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hoccfehx.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3apjomtqx.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jpqcarqm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ahoblwqk.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nhfverct.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3jeecucnr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3vfphfpwd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hedlvoeq.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hufpvqjs.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3veaxvmcm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ulvwqkfy.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qerrjmzb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3wcatfzoo.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kryerjig.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bwtlyzzk.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3oogfmels.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zutcotqg.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eucpcczx.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yazogyjw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3bxwbkfhd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ajiuauvk.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mhbvawbf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rnpirsox.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3zpgkybmo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3qvhrlicu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3gzqqbyvl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3tjrshkwj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3dlrpvmvy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvdgbprc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3emmoypmd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ijdaqcou.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fxyzvran.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3loyqppql.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qtzsztxp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zkohvqvh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ppcsggdx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qesnghem.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ryatdbkr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3egyprtik.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fmxrqhja.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ydbzimrx.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3zequrllr.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3edbnwbyg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zuvtcsoh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wnvybwcg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bgatvmgf.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3otejhbid.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3mkztxzmb.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3fpawarrh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ltrpflof.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3zktauriq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xxxssvul.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3bztypgtk.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hbwtgusg.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qggnvjrh.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3xpzzqiom.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qddggeik.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3htgrjngx.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ofuhrbhz.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ehubxhxt.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3icvjbdsc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3lhqtedmi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3oeoocdod.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nkajyxpl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3czvmitgm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wpphfbge.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3klsinkkf.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3hrotgqnw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3dkzavgdi.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3rcnlerca.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hmhrpkns.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hutelsrx.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3abzcmnkw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3davhbvky.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wkgcbnkd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qqusaetq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3qfflvfjz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nophagsk.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eumziseq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3vxtaacih.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ankcdgtf.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3yyczptaj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jicnmxbq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3absqoskh.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3skovspjw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3rmdwjjrn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pvofmfvz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3iyswvjaz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3aahahkgw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dwiwnqbd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lgiibglm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zgmsqfnf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3xyicavbh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rhqheytr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3fmqsfiyu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3vruuvuto.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3vksrepgw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3wlgqwrdm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3prvfhvce.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3chnjrqyg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3shnzdfvk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3lwagrims.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3rnfuuwlh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mjwqstgz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qqfgcxze.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3izczmuve.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ahbrsykg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wlwcewjt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3axltutty.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3mlupfshn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3chmyppvb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3gcgrjdks.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fkuowkcg.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ocffsapp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3pepchcxr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3bsjcbmss.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3xesmviqt.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3vglffhah.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ccvtfxix.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3lchzrkev.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qjjfwdcd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3mqrzsgzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txkxrnko.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3eshomwiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdovgfou.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3iuyqioxo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3vvkkaynu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3totvkkft.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uvkxknje.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fdsgdcig.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xrcswdpp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3eehoukcm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cxjsbiuf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gpppvctu.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3jdlstwkb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3aujcctzk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3sqefhyfe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3oqzcllzz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tklgtzqy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yxjvtnpp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3bahaqvoc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3juvnztii.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kcbkypvz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3dcdbrkcy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3svfyyhwm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3izirhjhb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dvctsveh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ffxxzdeu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlztrmwo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bzanhsar.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3srinbskb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nmzwjfdp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xhfgonmz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3rmjcokrs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3frdqhnzj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qzlcdpad.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyjwtejg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3claxbmce.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3wlixivwr.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3tweylugm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwgkqvbp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bymspqlk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3gaeoudsp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3sllwtxnf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzvyxcmr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vnvuucvl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ntvpblzr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cyrjvqdw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ledtqpsz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ogvjwigo.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3obdsqmrr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xhwasyei.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgreirrg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3atecdfwn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hebhuffy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkicyhpb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3xwayjajo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3edwgreog.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqbrtwrm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3carylfrh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mbojjnpq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3oxwekwsh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ithwxmaf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfqasuod.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zpnyehbc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3kwkxavep.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3wbuduvzp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hnagxlgo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3bedcstjx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3mwdzcngi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vwumcxsz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3eavoxceg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mehxmjyv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cnntfhtl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ufxmcieh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rlxsnbnq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qctuyjko.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jehbhjse.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3hmwbbmrh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnzcoxwt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcosnyfn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3msextyng.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3voldloru.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3unsxnhho.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3vhxbhaws.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hklftzgf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3dnvgzeax.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3mshwbtcl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3shvcfvkc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bwnxwrpo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xbevzgdb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3dofhdutn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3yxuuluqx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3etljpucz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcffnxns.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3gjrncfti.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3xwcppenf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3jwijjvbz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3azyypfnf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3orzikioa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3emtmypbh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3dhfggsvb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3aobqaxoo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tqhgtqbo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3saisbibs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ftcevmdp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3kkdnjrwh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ufymtqyb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3trnctvrd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pdvrxbvl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ajbhrjgn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3kpjzfofz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3fiuhivxx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3vburqxfj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3vqgssnky.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3xhdlnycn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ktibvbwz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3znjkwbcy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3bjpmhmdx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3nsgiaxbc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3tkraxcev.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ybeqngjr.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ymwdndqr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3fbmshblp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3mclgbjcj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fnysfhql.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uhzbhhca.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nfgtkqzj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yahsieue.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3amtszuxb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3oxvgddgj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qgsylwap.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3brmgsdtm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3uhiyvcak.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kpjqvuge.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tiellyss.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ckgahfnv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iduabxzj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ufnsbptr.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3carjkanr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3npxxsitn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ixlgdyxm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxtcuoyc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qfdotuiw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zakjkgoq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mmwehmej.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zotorxoi.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3maqmbdjs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ybpxcuzo.html


<!-- 参考信息 -->