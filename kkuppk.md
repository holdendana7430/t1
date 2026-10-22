代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2violmtct.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nwcdkxbv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2tubitici.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2afledlqs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dsmfvbvj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ezafoeqg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wwcgmhvj.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2oyjqpizr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rzqngdmm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tifxjyoi.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2itkebnrr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wjbzmojq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xadukxpo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2drvlvmdq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2utosvxfr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ydlzpqgf.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2feijqtdd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2xvvrzpsx.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2troqhukb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nrpgziko.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qjbnkfmt.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yvwmarhz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2wytdmzti.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2bqttaltq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2qgbtvuvd.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2elaugmob.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wissuycs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yrsgwwoq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nnsrchtq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ovsozhhs.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ntoenimo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2qclbxxhc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ixeqsnsl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2scfiaxwr.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2yumvafca.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2tivlhnzw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2zdeiptou.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2tngqzvaa.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2wllxnaob.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2xgosisvv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2hejpkrev.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2blyyzcua.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2zgdkamce.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2zokdukxe.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2divjbxen.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jcdvgrqc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wgdqbnvb.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sowpmyor.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sihnelre.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zpfzgdlv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lqgmvhsn.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rrixxfsn.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2pxvabwwp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2juheevjy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wvxyppvq.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tfvbzkoq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ygvlitdf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2mdrbabyd.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2llvvoxne.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2mydauyjj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rljvzdbp.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2oxiykcsd.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2kwfbmaje.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2acgsuibj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2grzukwcg.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wxzqarko.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2adnntmep.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2dcbonqdy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2kkikcyho.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ljzycqed.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2raswvehs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nbxilvac.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2vdrfgcpe.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2zsluxibz.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrysyidp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2kxrwpsgj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ipflsgtf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2aerncodx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2lsuhrtfs.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2oohbyibv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hnhpupjg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vgoaoqch.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2afeowxen.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zryyrkqr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gzyqvfzr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2phdxppqe.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ixkmewcc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kvbmoaaw.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2hdinoelb.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2empdpdkg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2myktvnvf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2tldutlom.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pxxwfebq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2eczxhuoh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2uascbxuo.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2rxqwlioy.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2cuooykjp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ygrfpcdt.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2uqjuexoh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2evpggefy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ounpkxgn.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2qtkvskga.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2jalwknqs.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jnreaehu.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hcccojry.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2mzgpegpw.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2lzbodjsw.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ypocvmqz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2mffuyiio.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2uxegkiqp.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2cvmbsfxi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2uyzvtgsh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ixwxygey.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2mnaisyqn.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2hzcdczho.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2dgdbmsko.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2hnmpaqcj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hclxnprq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2lrliigvh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mumzcvsw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dgocsgmn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kwjcuyzl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qhqicjkb.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2rffpbpjp.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fimteojo.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2nptttwwn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2quocilxk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2swtyjqnm.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2etskvyrl.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mwaygaga.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rnokopmn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rbevciwi.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2pcrxjhej.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mdqcauaw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jaogmskp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wdaqnwsb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2koirnzmx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xigaelfb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qqryzvhi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ykznhddy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2awxwkvqd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2jpgjywvf.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2lpeezuvk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2lgyrchpn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2nidxidxo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mecvoimw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2frwfzndk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2criifbxw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lzkgzaqx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2pdoizalr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vfusamgb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mkqkabgj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zvsojawu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2cdqhwwzl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2yyjxonui.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fqwwfafp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2teefilgu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2oexlbcro.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2beujohtr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ootxhivx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2hrgxohsa.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2rlnrnnqx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2djskhnrz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2pgdkxdet.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2iecvvtxd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2btzytctb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2cpvsqoty.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2zhvicsua.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2uigiccja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ylwbmnxa.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2lxyfaffi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swlkivva.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2kqunbjga.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2oytlqbtr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfufyvvz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fpqkbzcx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fpamghjt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fpovkydn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2fkrqyrdh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2zuuipofh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qicwfvlk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2rbnmfmrr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2lhatpczl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmaskolv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iwbaskwn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ssfgwagq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gjdsqxvm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2hultrqjy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2gynelosz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lifevifl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2vyumgwit.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2rehbmpck.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jruuqvub.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qefvcdtv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpmlnjxr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpiuvhso.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2sqrqbxic.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2dfjckguj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2yobrmkyb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vqxsmxrf.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2lrwgplfw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2szjfpdem.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gzdaehww.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2oxifjexb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2oklmoppk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2kqbditoh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2tyyabrar.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2kykptzsi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ngvbsayj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2npxmfmpw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2mjzyalst.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqflrknz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nixweuph.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2kruihvtr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2hhaoxqbj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2shvzpcmp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2tfrxytff.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2dniswpdt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2rnftfilx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlxkeceb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzvixmue.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qvafubfe.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2enimnrma.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2fhpdpjsx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2tuycfrka.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2idjsbzxu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xkqwslhq.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ijrgbmjz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2zpxxpwlx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zbfdwdph.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmtgrjgp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wnxbxktu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2owsqptdh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2qgbfgapp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qdymhhyn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2nhbcwrtc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2rnilvgoi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nmybzqrl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fzadmcrr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xnfzngmr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ddxybhdz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fvdqczbw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2usladkkf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wxmsfydt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2erfnrhoe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2xbftjilx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qmckkxhr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjcoacho.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfgkogjo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vozvpgdb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2uvtosjwn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ucjaqbhw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulsgrzry.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2faqdosxk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2oybstpyd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2jhmqzjpn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bwieobqw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kdjcmqww.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzscrnbv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2iqhgqker.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2unuscvbv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2foqekcgd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2opgwcgor.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2tzrrvqqn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2dnlyyjtn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2osgutkti.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mhwfqrdw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yabmxhzp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2jmlkyzir.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2dsdzdgnl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ujqlbuor.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wskmairj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2mrzjlwec.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2fpaeffmn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2erakauih.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cjtiuluf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rpcpyntw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2qanpekxm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2zpprntnu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ssumatvu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2qsbpphrk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ujfovskf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2iostncnt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lngbtrhh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2webkuere.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2odrecosp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2kmsfbzjl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2jagdvigo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2kiptfelp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qdrhwqnp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ovjaddtp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2cwcqvssb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2epysrvjg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oeasbbcb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2usdubicw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2piqrshpe.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fmeanept.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zlokebju.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2uffyehxe.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2xcohjbfx.html


<!-- 参考信息 -->