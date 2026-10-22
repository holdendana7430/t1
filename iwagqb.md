代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rqwbxvco.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hggajqnn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2rdgyzpop.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2kwppuqpb.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2jxoetciu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2mdjtaoft.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2obastlyu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xrrmwlww.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rsyesrvs.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wejujgre.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cieiywgm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2zzfhvdyi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rkzqrbft.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fkthfhfl.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2jqtfertj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2erwieoyx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ekuvxkms.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2mevnmzwb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2dhpnleux.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2uvprmmbs.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2eyhdgdhe.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2dvtytbnw.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2fpwavbsc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ugrpnhjv.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mcvahipo.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tvzrxane.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xuzzqobv.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xpluymwl.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qkwjjbbv.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xbndmlat.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2usqesdvt.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nbzzlyey.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2jwwivotl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ucxcxddz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2asvrkzej.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qzunknqf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nxmnlsko.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2galftpsq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2umkflddv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2fdjgekgw.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qtknknbq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ojpgcvav.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2emgeercw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lslmwxjk.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qmuibqzz.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ayewnnsy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2zlwmuvsj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2vnwqmnwt.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2klglfugi.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2plbkjfzw.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2nwyhqmnz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pgbewjzn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2jxgfiver.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2calrgffi.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejbflnww.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfadvzru.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2dxqfotat.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2cgqtknfn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zltwvrrg.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2nufgcvxx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xnvaaahq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2caxigdps.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2homyzzah.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vxjgimeg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mlruuquj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2myhijndj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iqjdihfx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wbdlknrt.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ibrafexh.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2iptaczfh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jcfrgjtm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2fgxclasf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qifbrqmr.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2mxreubdg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2khzkqmbh.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2nkgjxrty.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2fexcqtgb.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ynockzuw.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2uggwuayf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2bytcydhc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wiizamch.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2auuxhxwo.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2codbcrce.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vonhlptn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2iidrgvfj.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2viapcnbj.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ooaylxct.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2dcswmgoa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2mtitdnxq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ivznxxjn.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2cvcfbdgq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2lhhhpfdu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2phrjboet.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ctjatuoh.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2euvoxrky.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2djhacwzp.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2hjngehzm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hpmaaqsi.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uskmncif.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wgtxhzwi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2oyqwfktw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vkyffcop.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2eyfrkbct.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2pufewwam.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vpgdoqqo.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2piutlhtl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2hmmwzisx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2fmvmuagy.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zypdxdeu.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ydcnklro.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bbquvjly.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vfsvivdq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2liwqgfmh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hmnltmrf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2bcpjcknt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2oewgmmjn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rgygigui.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zbhdfhji.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xkxbtxky.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2nzvhgwui.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2kvltutry.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2xltsewys.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2odcdrqhp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2hwbbkoxg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2hwhumzyz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rspvadyt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zmfpissp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2xwnltmsw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2awamdhzt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2uvvckzet.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hvuzfnda.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kezzujtv.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2uiktctpy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2nrmnajbp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gumphbcv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pbubguwv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ppmojucu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2aozetcmn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2wgihmjwz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hebygaqe.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2nfonoage.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ifixiwmt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2fqtqaibi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2cmgimvij.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2lolhoson.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ngsgzxgr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ebwpvvzg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2rucfxxgy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2imlnuvxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtpxtoqt.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2uhixxcfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ecpznelk.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2onjbhecp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2raygmquk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2tdwmqdcb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cbbhnrvb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cbehqgjp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kuthlddd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2fophdzns.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2phshhigq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dcpbrihx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2wnvvdvrp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2rqvenqkz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2zfwlvpdh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qxjjjbqn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kzusadpx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vfzghexq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2jvgotaij.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vhrppnym.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jmqoyqfm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2eneughwo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2bzqwywbh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2djdlasqp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2muykrrdw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnwlweha.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yumlprne.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hnmwrzcs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2fpvpfmzv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2caplxyfe.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2uphxdhop.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mlzdjook.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2scsecuht.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2okprrntb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2esfllskz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2rsmnnkjg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vswdqlin.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2unhvaeax.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjkxdpxr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lvdchspo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2yggcszsp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ykiqbsre.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bqwjjfow.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cwqcqmis.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2kgpqhfex.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bsgrdfka.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2hlpiuarb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhrxumyp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2cvusxgoc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2iobymbea.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2klwwsqvy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrinflni.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtvhycch.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2movbogek.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2tupdldkv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2mmuyiuwd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2qztyfwyz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2yizeiptl.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2saqjmrkm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpergmni.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcekbjre.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrctazoy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lvblmynu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2bztjulae.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2klztrirh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ebbpmjtm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mjjmorea.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2dunzxtlt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tgdtnygr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ffhrvxtu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bxfvigee.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kjizdgoa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rvyntueb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ulbhnqkn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ygmljnmj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ustqfvsg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ugvmzhtu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ndtqixrq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2euephxlg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2owsoniok.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2abwrjqpv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tlmrjwnx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2wgcayknv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2weycfzda.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2jahsienh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2sdwnrwbp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2jbhowiio.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2yeoasfdc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zpgcwgfh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvkeohqc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2wiaytrhc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kdnwvmfe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2xpurrbcl.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2kdgqtzcb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2haqcfjef.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hbwuwylm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qhlnpolw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2krywflnz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2owmzimpd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2yffftqzi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2coldfqgi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2pxzrzuko.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2mvhvgmyj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ljkfhzqe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2fxwxlrbv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ddeawpkz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xaffgrds.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2firnpqfl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2yysfwgvt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2gmuydkwv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2dgkzzjnq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2upbjbcnq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2tlvbolpr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ewwjfnbq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gwkiuigz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hapuirrb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bggmssio.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2usjixydw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2opzfdyna.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2vsgpekpm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2avgipbbv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qisligam.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2jlflpkxu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kzbwdykp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lojgdehc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nqfovgxa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ojvuqvva.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ntkvzmqy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lgajkkqt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rxjlctzy.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2yesluvvf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2zliuhdxr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ixohmfqr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kvszqmoa.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ehpwjjlt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oeobjbvj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hdbbiigv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ptdukioh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2mysdqccq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2jydgadia.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2suxosxvr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2akwxyggw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dxcaenys.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xcqwsgmo.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gnitnfkf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rpmhstvr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mxumprzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iomtgspl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vqezfrmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmxjbqls.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2itjvxepp.html


<!-- 参考信息 -->