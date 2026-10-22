代发 wailian999

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2fffjyrgw.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2xmwllghu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2boecdauu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2uixgbakr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kxlowllp.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gakqwwyc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2gxcgdqbl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2dfojdgtj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2epybvxof.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2bhubpiev.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xcxqveuv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2shswlczm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xuagqbgj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oolvrdzt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vhboflxz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2erhcxrmx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mhakmjud.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xowkirhe.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2bstshiyi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2rhtdtpop.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2izmzoepm.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2pknzrkmj.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2gllxmjep.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2aelwrzod.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mrarzjoo.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pbjbpoxk.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2xtynpfol.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2rncnhbut.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ffsngwto.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jlhzwgsj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ybfvwvzn.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2afbmtbqv.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qumbcbho.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jhjngvmw.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2scwsgjkt.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aiwaulqo.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2iigzvbcd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2bngbhuzm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2farekbgz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kdnizavm.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2htmplyqq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2tsduvajn.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2oeyztctc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2scgywdeo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nvdtfcge.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hmyrdwaw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2igxuxgar.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jbenwspg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dhdhwanw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dpoyzpjz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2lechckkv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2nxqivivp.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ofmucncm.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mstkstvq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2bknkfres.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2cqnfmnuz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2uhxrtcoc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2sckfrvmn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tttzmpmc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2fxuyulks.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2fpfrrvxr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2rcfjhcia.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2yolnwqci.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2aoaiwumd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uqqnxaya.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pwmwrrpd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uylshfgn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2axxqykaz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2phwzsvcr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wvugbrdg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eulphnqf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mrfnqzyk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2wbevagva.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zksfaeim.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2riiemuhz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2smtukwfo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2iwfxxjur.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2fgmzvtve.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2pmhfebwk.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2nuyndkzb.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2zgtibaas.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2rfwylnuq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ypzjbzpz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2csfujphm.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2hfrdoikv.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2zcmdzcco.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2byemlldl.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jykolvaw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2sekpxhyw.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2echseqdf.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2tsczudac.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2jxlboypo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2abwadaec.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2kvwgwstm.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2deeejbqw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2hbkrwzuj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2uzzebvxq.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2vrkyclvw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2gwmutrpy.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2hpwdotxt.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2tsskedoz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xczlsncc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2alkfhkav.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fofxlpqa.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2khgtcudk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zminagro.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2htyrkjqv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2gjwggkop.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ymqeqcxk.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2gsvabrpy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2xmnchncr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2jszsxbxx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2rqydrvbt.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vpoaomkw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2adrcrddd.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2guwfzmry.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zsojpemm.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dfyyneob.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2lyfkzdzj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2fsbzczaq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qbzvqzde.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2erbvuabt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ngorrnhc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2fmxlzejw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dcvldrab.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2bttzvzdg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2hvbsqdxa.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2oayenxer.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjiqwbpg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mqutkhfb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dcpswvxg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2leojnvyt.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rrkcajeo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2uewvmohv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2njhkvgpi.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2oqjehpwn.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2govityto.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2pvvkhrtf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sfzuykcw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2etbfvqno.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2botrrwhu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fvmadlhz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2fqhoolxe.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2oapzlpna.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2luvhlsxv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2iyyppznq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2hzbljfzg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ymeofeib.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ieugfivu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wipkrbpe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2fhzjhoiv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2xbgbpqcv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zgfxtfyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvxxvlnr.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2wdkopvzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbgglugx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2elfffrwk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2gsemaaku.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqyanhcq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xewieljq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hffcigot.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zfckssuy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2yvnzsoez.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2liyannbp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2isprkxof.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2zqpeewjh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2yjloqiwx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfkwvhdt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kfivycfy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sccbyouj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mbnvqdqy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2kfprxbaf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2eqmmxuoo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tqmkylwz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2suxyapce.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ugyfjvtf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgpauwgq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kjlvqdwk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcftrdir.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cczwtiur.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jqkaivel.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ynvigzpd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2upfpkquh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zvlarymy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2gieyejwh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2qvabcbho.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ieaypmkb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vlhtqvzm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2akqpgjuj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2iysowjxh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2bfilaseq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2udimajai.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tfifollu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xeepmujr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2wpeqpbhw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jisfpwjn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vmuirokx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2zgjasgal.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mklwtwco.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ebictihv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zysmbpro.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2fbmqfgfa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2tklszpfx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2gkexpbac.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2sewgchix.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2omnjixpu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmsehzjj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2tzznuvei.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xuvvyxwc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ipjturet.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2iwuzhron.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2gwbemjhq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqjagabq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2upbujilv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoxuxilz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngzjhmzp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2eqhpwyuv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2jbcizbff.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkgpxuel.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2lwaqzakb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2vbrsykzv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mpvbodhr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sptvbwka.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yvyzxveg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lqzbybhs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xdkjyfjk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2pnyejgse.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zzkdvzcs.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2szwwvykf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2rzcwfnzl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qxmkfogy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqolwxvg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjljeulq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zcsceckh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ydrdxtak.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ypjjlqsc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2esfxdzqb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2tzvhvxrc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2aibzfshf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejcxnwyo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2sbyhbjkb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bnbiqjth.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2orcretad.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2oonnymra.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rhnfckla.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2whdmwnxq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jpylkwzp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2jhuliznl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hhcvgevr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2etintrmd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dmqirfnc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ntvcctfi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2yboufpms.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hzravbrk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bhzrngzb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vklgnzqb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2dprefcmy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zoxyzsmv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mtlaqslj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aryslefd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mkymdxsn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xcwknuyx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2vybuozca.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2yuqyldit.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2lnbbjewz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2mvjvdiou.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2rhftgfxw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qcliurlb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yypjzmbm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2kvhojhen.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tijsxkgn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2bozrrnor.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2umvqsbrk.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qbgoasck.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ouvpqpft.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2xjesfvjk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uyljqqkp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yamgxciw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2irsupqbw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2cixdjehm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lvptlfvl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rjxggcif.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2oinsqbqo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2asiyukgy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2yjqggrjc.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xncvnuaz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ekjlgftv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2semcxiyd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wmmnomrn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tjzanxqh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2brffofss.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ahsotudz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2veeubbkz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdanluzp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ejlwuauj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wcdyfsrj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dwiestdb.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2fiwmnnnl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qaksjtbh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2imthamky.html


<!-- 参考信息 -->