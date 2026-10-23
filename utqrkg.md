代发 wailian999

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fzlmbioo.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3rqsumduf.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3gjwwsglw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qshvuwlf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fbtjhpuh.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qcppnxwp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3hzufddcy.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3dxuosofz.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3fottzoel.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3afrroovw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kpslvulp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hpumhzoa.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ilsqdzno.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3opccqjwb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jjesgszj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3fjsqljhu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aydsbaso.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bewrtrdy.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3wccmpirn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3jeqlckeg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3vyxcgefu.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rzyjfybg.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3nmujzfof.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3meowuomm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nauudrsy.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3qqitzkca.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3bjamyqqa.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3gikksnsd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3friytxha.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ojcdkmwe.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jgyvebmd.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3grhaflyk.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3blncztjt.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3brebzrva.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lzmtxwhr.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mxorapkr.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3anurdeoo.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3qcbqdobz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3csrzsoyp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3neirgrxo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vcuzhams.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3dqljprwj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vpnznmmb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3hgrwkpbn.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zkrudthw.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3hpjzqjhu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ghlkhptx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ctvxfnwk.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3edwpbomy.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3crxwpvvt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3mathzwam.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3assogezg.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3qnvkilrx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pwarbdno.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ybpbjtmk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3iemvwbtb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3xhjeokud.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ibuacfnw.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zduqdkhp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmcskjre.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3xthsyksf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3spiqqius.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hqqeldaj.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3rjxyrkdr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qlgodevy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gdtqpkci.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ivojqerv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3grdfgnay.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lhfbfrfa.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dcjszmri.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qnwghnyd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cekahtnb.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ronwfatl.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ivohnlmx.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3xxmcjrjp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3kuousnep.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3eqtbebin.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3zkohiyqm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3wjwdjvgn.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3pbsunlqm.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3xahhagoi.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3fdqsgvdt.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3nfqwkuav.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3trljsics.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3wxjplvqi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3lvanvifw.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3etvatigw.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ftrlrqku.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3vvtarqif.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3xvilfbfa.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3vzrievdk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ajsoruzz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3roiadmjm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ylqwszkd.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3yhncxpqn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3vsztzezg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ocxndami.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3eyrwkggi.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3akeeyyut.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3hlgsykjp.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3zuprynxz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hnesvbcp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljuwuufw.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3atbhpzlv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xpecoyxj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jrhwdztk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vdjqnpxo.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ogmieoci.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3khdvrkzc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3znlhkiso.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3uanqklsz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3steyofee.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ozvcqqsk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3iimmgmoj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3xxifvmgt.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nahpumlr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3owdhxsvo.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mqxmohkh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ktmbhzxh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vqtedntd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yxrefndl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dfcqhemx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3eajcmtpp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oucrheya.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lwxauivb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3lcuxmngz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3wcyukazh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3anqdpzmx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3crvtrute.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ohimtqwm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mcgrgnja.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3cuzuufch.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3guzmksfo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3fknleqsd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hizrnsif.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ejawiptj.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3lmxxjnqc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3flhcjodf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3shghmhiz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lwdmhvbr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3xvxsieku.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3felxgqya.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3vleahifl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3jmhfacvh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ufutfvur.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3vwzaqwai.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3snlfvqdw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3wxxmulok.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3crhhjfpu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ztsqcydy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3hrhgqpjz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3pwzaajzk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3mtovqlat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhatsecx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3wfnggqqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dwduitsx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3efqahqap.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3vuhbtyjb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3wzorfuan.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pxtzmxnp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3shirsxxz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lrfdyanq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3sxmppfyj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xdnxspcr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3unqsgbrh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3rruxtdna.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3antjblbm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjxfnhxd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qyhaiaqf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rlfaowfm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vbgbzekk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3khuhdomj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3hewwflwm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3idghcqbw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ghssxoer.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3itjdnovw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tketjdlq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mtopwdrx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdcozcbs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pckssgpe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wyxhjysd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3xpjbluax.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dgbhvwnf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qckptgsm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tpwbnccc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3zripgkcu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3gvihidxg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjzrwukg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3hgkblevq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3luloahnh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3omhrmeqw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnjpsszg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pszokldj.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3caywduvx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjebfueo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hljtlref.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysyqfskb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrbuvysi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3oskvzolo.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3vfrbcnbh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cytrgzwr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3jpulpbyq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3kuenyzwu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3glfiwkcf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3pqryybzm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zjbekpzw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3gimxrlti.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3zumasbnh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rwsmmwhl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3sbreahdh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3niaolymp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3roatvsga.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykaxgjbl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmsmxbgw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gpslbsrr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3doogzmmb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3yywdojtl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3mgetdset.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoatgfgh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3axdwoezt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3kprafihn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hqtslsuo.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kjdwuazu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mltgftar.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lrasisuf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3woljbkmd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3sjnbmuom.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fmdfhaaq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3hygwriie.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3tntsmxwb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hzxbhjoj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pvbaeopf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3huuwcdfv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sioalasb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3sxpymbfb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3zwkltbze.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgmbjfit.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3qjcqkiuq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3wccxuhtz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcdikgmm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rqttgckx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3aouwfumt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilpwpyco.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3fharixed.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3azplgnco.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3anlupylq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3hsduxwtl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3sbxrcggm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ppgunrxk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dekowzgz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rlahqons.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3fxncnxwq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3nlkcajsq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fdpyqlwl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qehnxwan.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3vtsibhds.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ebrqqycg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3xfcbntxy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zexxnvie.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3frdzpbhy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tgweqyiu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tbxokhwr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3hqmmhanx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3dmgwjzaw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3btfugmsj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3kycutlms.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vjtzqzft.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tcalizrs.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tqbcyzao.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wdakxlxi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3bgsxqsxz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3efhrigge.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3kuoswgjj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3kqxjuago.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3kbefhzbh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3teurcppv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eqxwfglc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pkviesti.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ukqsfqtg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3vpvnldfh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hbyprmcw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mednxqes.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ypktbqhb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ubypfrir.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ugkpqpxb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sskgsdgb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qfohpkfa.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oqpeuwfx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jdaceeih.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tjumqozz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fqduhbtw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dyhbsets.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ohfqfsue.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpqmietf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vmnibcjz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gygvotrz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fbrchlct.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3kjgrhnbc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ppyygedy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hxkmcdaz.html


<!-- 参考信息 -->