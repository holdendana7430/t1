代发 wailian999

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qcykslfk.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3aadzaymt.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3tzqsgmul.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vuerybfv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xziypcmf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tziypchy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3pqxmlyfl.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3puyeslrb.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3cspgprdr.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3pddibhrz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3xvncvqlt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lcmfufqi.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yonzdgeb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jrzcgyfj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3scufnzta.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3bkaozbtm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3waiqfngn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wysvlzih.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sdflxoxt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3gvbqtufs.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3xejkegfs.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3wkaixmam.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qxktnzje.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3mvfrtpcs.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3znaqdrsr.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3yjmrzror.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3nuytqbmr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3gtrnalbx.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mdupkjsu.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hkpabnap.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3usjpjdtr.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ldrohyia.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3unjmgfxw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jqqukoxs.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zrshbktu.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lrjyijjd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3pjncjdnr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3rsrqyqdj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lcfnyhdk.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vxmrrpak.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vpjpfsiz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3npycnejv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dihdycab.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3kkqhjqpa.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wydpcasd.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3diirgfud.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qmjjfxfw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hydkfiqc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rgcihjse.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yphrvaho.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3gnrqrkdr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3nsyzxyue.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3obexetae.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cnzyzqjp.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3kciuibvr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3qihiikcb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3sujdtxpc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3samdybmo.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3gavokzvf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3eaksqynp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ggkimjow.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3mhkhacls.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hpalsfjb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3qxxgqjti.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vocpkqhn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ofshknlo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hgdxpfcp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hqrhznqk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wszgnxdk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jwbpjbgs.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hljzjsxa.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3crbpoeno.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3xiadtqyy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jfjdjfoi.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3trhwubhw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wluwetex.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vxyjsrfd.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3svxdzbhd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3gyhhhjti.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3eoiirsyy.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3bploehtk.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3iipmahaf.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kfivuamj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3xgofppol.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3jcfolqmu.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3bsgcjjvu.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3cesznvmp.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3waojdvho.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3imivlnwy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3fsqwkuia.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3fdggyyhy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3hxflbtxr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3boymtohn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3dcvjdkhf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3urzocdgb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3mfpxnrxt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3lfecdkiy.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3noaswnrr.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3drujzlbm.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3rfbkdymr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3zcwlxlbk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3piqtioek.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yugnkpsv.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sgrylclk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wnjucglj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wmdupqum.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ignnchhb.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3okjwlqwc.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cdsagstg.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ksvcozqs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3ajyahxog.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ftsgxzey.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qvekoeno.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kmgwvecx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3bfixlvht.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3pcovualt.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hgemzpfp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nkadqexe.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3klhvdnfr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3tozukiwj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zunsulwj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nmswzqtr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3unhhvjnh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wprojkmc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3sbutjkgu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3kxhbhwsd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3zkrmjlhv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3gbvrgccq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3jgcnvkbl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fgobgjtd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cbqmrrvy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3qlylsmbw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kvaxxdlb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3onnkwddc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bzlrsegq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nualwtsr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3coqvesrs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3kmmgodzl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqzkdfiz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vfiwfmhy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwiccxxx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3quvurhjy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3kzknqqoz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ejdtpxle.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3jpkxpkbb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3nhfydvzp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3larefbmh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3tpymohmz.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ipdikyoi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3cwvvfwhu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3qrkhgdij.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3jdlnslgp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zgduwscu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfsevjab.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3burddbma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwwhbbvu.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3fxscqtfq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3igbwdmah.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3juscfdmv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vnbiybxy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qizqwana.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cucoeadh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3wdhqvbbi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3kfhrqodx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3llcrzyca.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3bqifkynh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3xjeefyis.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3pneudany.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rpxgndoa.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jgfisogd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ztofnhxj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3gamyizfn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3gxzzfekg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mxoybers.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3wqeurzbn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3icqbmzkf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vprxjtdq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kewcnfxw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pmrsewih.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vrkwauej.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dystbllq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3jrjbyhyc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hpzwcfjp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rhpsrvrw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hmbouewh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubcwgbpy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nfrotsoq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xxxpnvfj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrtkqtan.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3yljevexe.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3irsomikv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bahbgoko.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hyhnacum.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3tciwobvi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhduiids.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3beqouega.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzihhkep.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wunfkcas.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3toyzqymi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vqixaptd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3nqhypcef.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3qdvahhmp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3jnvbkyvy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3gksgqxjn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tohnmjxk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3avjokfob.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3eqlozjou.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3xokeejux.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3umilwvez.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3syafcyyn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3hjesskhn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ojrushdj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbknotwz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3okqgwkfw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cmmjgmrb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vayoznjr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3tqwwjeqk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3waaqvtyn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aparciyv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3lecsbnnb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3bwbwodws.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tjnrqcne.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tadladxn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jtaruuhq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bqczqfge.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xobhrpvd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3kuswgepu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ypplsaks.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ktopjvqd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3icqqnlwt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrysgjxt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lfinvrql.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bszhwevl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejgrepjv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3shtdvefk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3sinzfejk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mphywhuh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3fmgmnnit.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3tohpsseh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3puieugkl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vkvwkqlu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ixtripwe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3stmcajgv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3urxxlozp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3vsauuqai.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3krszbvie.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ncwlfbni.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jkuwlzdz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3vrjmfpln.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ypwtilrd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uvzgrmll.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3suvszltt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3xqdjghbw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ygczdfnb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yvqnlfjz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3inxdtqyw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xqmztctw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3wglmfcks.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3buimgzcm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ypuiczao.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rqyrxbfx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3iqnndkfq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3pxzsxwoa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vncreykj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3npnupezm.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3srckvmab.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3xpmkaomb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3pjwedais.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zrhreulj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3pmmfhewy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zpdmdmtm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3knnsljug.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3macynrvl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ybalrpzp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ivkokphk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3wtjesuny.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fhlqroxk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dvyfznyn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qawdsyyt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yyfifpwi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qkuuaymv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sycdbyxy.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3sovxnayw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3zzykhlou.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3abmikvqx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xmnbarlr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zzracopa.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jhexdeyp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wxbvolhl.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3stvlnwan.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3matkpzsa.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fcanszei.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3bwedzfpq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mnvmuyyq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3egjesnga.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3drydhngy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bbdvnqsv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3xrcadvss.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3hxatbqzt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3stnlzdlo.html


<!-- 参考信息 -->