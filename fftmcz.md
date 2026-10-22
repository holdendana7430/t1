代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fdtfsbye.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2deuwtxql.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2kideonlj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2qyydmvgl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2vxkqquwh.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2gutyxxfh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2mgznejjz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2uaesrhte.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2yfbcagxg.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2khyepsgz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2fuwzcfie.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2sqggpnrj.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xxtnmzmj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qcotijas.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ffpnppjj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lppwoupu.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cqskdpgz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cfquysux.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2atexltes.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uhdzeyfg.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2bwldotkp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2rvqjvnau.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rgtqfkcy.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bvdzncsc.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gdksdrpc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2iigmzhri.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2grxoczpe.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2epqfdicx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mfrxnbgk.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fqocesjn.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2thqnmfwj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cnpqiszb.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gumnzkct.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qtjryvnc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2wiaoihzk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2tnpvfpzj.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2iialskrq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vkkcwmol.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2kchbiltt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2cigxqxwk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2cwkjyrnv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ybwdeawp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxsqnvwf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqahtgef.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2zamsqaez.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2hogdqdzt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vohpisya.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ibecahrk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2krmiiydh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bjtrujzs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hrsvnnby.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2urdchzew.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2eplngrlt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wngmlypd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qoskkbsr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2euekcore.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2yldxkufh.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pdemuykt.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ebngbryz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2qjwwfsob.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rdswbkze.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2emeaazvy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2letennqg.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2fcqfuppl.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2nifsfmsq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2mxphfoyo.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vpplkhrf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ortlqoeh.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2comdtchr.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2eawtvflu.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2mynbezba.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2xijyxkmf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2efnoered.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2lvcsjzfb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2jfducqye.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2xnjonpyw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2zinuojvz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2heqiatcr.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jajxdoqc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2sxxngtou.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2bwxlqolc.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2qeogxyvz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2houcfyyg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2tyijxsly.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2iswmjjqr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zcniwpbt.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2doaraony.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2spdxovoe.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gxvdjvzk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dicbrbel.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zcxlifrh.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2xvvakyty.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cjhgpyfh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jyieskzl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2fuyzpejm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2usvsurbh.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cmhroeok.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dqsvheko.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2srtnnerb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zqvgdadb.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2riiytfkh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hdjcmiwa.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fyqdkshw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2qsyyjwme.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gutmreqq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2dmfrsiuv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ylkmxoum.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zlksunoa.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2udyghzii.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2lazujteu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2vfyshzsp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2muobihlc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2pkbyrxxn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vbmniixd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hyxlzbaw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2pwoluxsl.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2wdytpiyd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2xebzsois.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uqahfwvy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qbbinijw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2dalbggqx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yuikvyqr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jcpuriel.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2sikofcwb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2pnwdryci.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tcyhldeo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2eobofmmr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dtbcmecz.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2keprjknw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2heciwpwt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2jouwqfzl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ujnxhksk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2bhgpfvuo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ngpzytdz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2wgcweckg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2oveapdcf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vlrmcrak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxymmdoe.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2jzamwnvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eusugows.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2kgvjywqt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2veqmdkxe.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2sedmxkxp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zcrvdnlr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ppgjyubj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hlxrwrsu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2fwzjyenp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2rjyjuepk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wmyjuibl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2youlhhjg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2sljguhdp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxaiqwjl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uhekvzrf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2oobuugrz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2agpheuzr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2edgcywml.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2rnmivpqj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yoyisrys.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2zlxmwsdl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2mlhcaaws.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oxdurcjq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dexojuav.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yimnvdje.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2egyxrvdd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ohpzhuvy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hvosrjdf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bsoxmkvy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tqmypzfx.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sakoczcp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2yqikwrtt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ghgmszvf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rzsgyhzd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqjphjup.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2cqtwmpls.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2wgrzryju.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2enuethyb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vyuvuqqz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xuozoswc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgjnzyej.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cqfcbcwj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2pisnbwaf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2tqujcoiz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2epixysut.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2minnekge.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2qigqutic.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2havuzyzw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2eguaalhg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2dwhiyedg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mrpdtvjy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2banbkmst.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ekewxrbh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ageiwavj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vgsbgivs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ghttxgff.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2wrtwnhax.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2osomhomq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ubfftgxw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncioyjtk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftjpikfi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hflhtbyt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2zstlmzmu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2lanmbdzv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dxixttpd.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2pumbgoin.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2iarrhztw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nhczbnns.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xxtsxrmp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cjcinjfz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vppsrckr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2hkcvyayq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2tmxmarge.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2urcgvhrm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2fhdoxmqc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2hxonbfaj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lwzzssfh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nhadroko.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmplqbpy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yenijpmw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kygoqase.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2gxgcwmzq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfgjcdwp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2byegbwqz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2uyheegze.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfprzrrz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2skuegjcb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vtorysra.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ohiwsroa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mkmgtvqo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2plzgxspx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2qwhrtyie.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2byixicqh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2hbdnzjbv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bcdkhvup.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pmjmdkdm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wpomqfzy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2isponsqn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ktlfrtmp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2xjohguno.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tehwbbwq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jsghvotg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2zipkkrwx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2rtlebeps.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qcelzzdc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2swaebczf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jvwdkubr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2hbghgyse.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2plgapgvg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2iwqklkyp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2jmhpcucu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2rjmyvjql.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fyauufns.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ilkgxchp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bwqxmgwb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2lueypwco.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ydbeuxby.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2jxgmbxip.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zitzzkcf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2rljgqhje.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2tzjvdpfp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2acyajoty.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2brreygcp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ouhpeplp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vqquobxw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2fwoptyxe.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dwytvhdw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nzhdfyzd.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2nxlojhwp.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gjysacjw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2zxxwelqu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xmjskenx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ujuhntaf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2boupaoak.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wxoftuua.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zasljhnm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2enzgcpew.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rnizcqra.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2tdipevaj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2dnqwhbxx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qcinukhi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2prqdphhw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kdmkogvm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2gdlpvdxv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2rtoliqur.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2refpeohe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2quppawpy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2wsjhteqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilbqssed.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mvblmzla.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ihzeoilo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mcbvhlxg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tfwxzvcy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2blsgatjj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2stfkbcec.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2labkrfoo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2uqxgqqox.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjoilwaj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yvjuiinw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2jljiuvwk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2gelqpocb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ognktgyi.html


<!-- 参考信息 -->