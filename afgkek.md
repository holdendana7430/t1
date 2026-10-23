代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3uwkgqfwv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ortxqxht.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ncpoxufe.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3mgkyatqk.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jkaacabq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uihmdzvr.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pkwndpfo.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uagrqeoa.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fdjhmauz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tuiefzcp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cdrxztei.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nyojjyly.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3puimhjsx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3tgwopolf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zokalmyj.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rljfoteu.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3sbjaebmc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3lpjxgasf.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3deedjqgi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ziankkkx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tdzuwfoz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ilofydol.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3nzoaofzb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3thrwpgil.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ufasugzd.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qrnrviac.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ipcglebs.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3tglawvnh.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3inmnnbdg.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vrasqpch.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3worgxbky.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3kfueldnm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3utkyksdb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ywbllhqu.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3benqwbxx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3seijmqbi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3urdxmdcy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3sxbytaxi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkiofywl.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3yfqkfmav.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hepoycnw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3trdviopk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nivlvznn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vhgjqhlg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tnqvtfwo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iyiewcqi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mzacdpug.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dxivijot.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ocijkjhw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xkupdbab.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3qgmjwhxp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qrolmnzi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jizuncdm.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3rqpbkvej.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3oxygrnmq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ccmztrxi.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3srcjhkju.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3uunmdqtn.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nufqhimb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3qijdapwk.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3njdcesql.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3xvumhcnb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3gbrthacs.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wxlxnupn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3cllqlywv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3huavwwvk.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3qtzljrrk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3psfrunvp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3lywssxdh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3gniaqglw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qmchxykf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3hcrjvcgq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wzsdvhjd.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3joyyjdnx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3abobuqba.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3yeynmobl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3uhymviyr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lehklnfk.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3deaqrwnw.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gxofqtsy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rybhmqaw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pvupowld.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fofyqiaj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3rdsxbrqi.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nturycrr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bnvgetaa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3kicbrrry.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3jmworsdj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vrvpszzo.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3pjqytldf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3layulpio.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ktlxektc.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3pggtpqdp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xdzyhygy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3sffhspgu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3metkylcm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ypkcubnv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3tkunbwkf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gxbkhzrd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3sknvxrdj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3kyisyzmd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3eclentht.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3wnqwlsmf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3pokailuh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3peamfehc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3netfxaoj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zffhjcmi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3oywqgkcp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3jpvdsive.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3xcaxhurm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gtainwux.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rrdmpsqz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3egzzecxq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3fucuxypu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3psfmsavn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hhcrwooo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ieahnsyh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vyngdxzr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3poignagn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fqmrjfgt.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3qenbifij.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3mxjcodva.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rjovekrb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3dexjopsi.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3fbaxnzod.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kpitmund.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3hbwaxqzi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dwlnylev.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3obvskzwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orxahimf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ygxqziiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkahvers.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3jxzhvyfw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3bhxittgr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ugtxaqfp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zoujhbkr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tdkweusl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3smyuuavw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3fzvbuylt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3fjsbvdso.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lkuxtcek.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3lhtuecmp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3lnugdcdg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3qvefbxku.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3noduuylu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bzeytxwn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yovwvdde.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3odoiecmd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3yeghoxas.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bsygqezl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3rcrclebq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3coypaxxl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jebwakcw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkilbdmh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufttptex.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pqshjmzu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hooatthm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rcssokvj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wlvskths.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ysdciyxi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kivuwlxp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3lwukvoed.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xoqcwedz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pyzufgkk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrbbmows.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3brbcurpm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3uneanwzn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbpsxaue.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3olsekmcc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3gxoqaxnx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3deqpwxpd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3towwerqr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvekjoja.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3wvnqlize.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3sxcboolw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ppnarbaf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3xcswenjb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vttndjuf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xawvvfow.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3montcgnc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ujxylibh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lddxricp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfokhxzq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ibbuqizi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3epskqjgb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ctnopjvi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3cakhqioi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lbenibwo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3appckiis.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cptrzcqy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlbnyrbr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckwzuwll.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3icijsqsj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gkfkjird.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eemikwaq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3uzvrsrnv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3uwrfcowm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3btzrbffw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pluwgrbj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3izfxcece.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3agbuyxpg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yvvyrubm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3mxlmlhej.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aufujibi.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3kykgzuuy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3vlkgylrs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wywfhhrs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3egwdefuo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzkuafup.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kmpltdch.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3fhsoyxjj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3jjkbrqnz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdouiaxq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3qfiacvoa.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3gxparxyw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3qgoncsfc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3knqduylf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zccmkblt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnlbjwvz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qgufzmlv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3cszhdaga.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3khogkrmv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3cldkgrio.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3oinhdfff.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vhhqkcth.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fkuaisei.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ychwrjgu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3pbarrzge.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3nszbaveu.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3dtxwwrvd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lecpuoej.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wkckqqvz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3irruwkir.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3bgrnppgy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bxcghges.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3coycfqla.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ckkshpsy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3lflrqebn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gdicsovq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3xgbiowhs.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ezkphlgw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ldblxhzv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3tvlwalvu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3scjspwpo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3uitqyzih.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3vgqmkual.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zljpomqh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3xbrsdrnf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3wtfgznof.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gjpzporb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hncntoht.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3vaoypkaq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xlbovold.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3djdohozg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kjpskbac.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lqysbfxf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3meqnmepn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ygzyocqp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gfwregah.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3nnwazedj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ptbmsmqb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tbiqrioc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dddawnif.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lpnwangp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ftcsquor.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fbtwcwmx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3clsaxqev.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3prooswvw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3jmnxzdia.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3qirdrxbt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jruajjxy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kstlxiqd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nlpdrspu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hzgftygu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3vixoicjb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dobwvnst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3msrgcibz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wricucuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnxikigy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qipzcjml.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3atlnmvdt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3otgdbgnq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziqbrcmg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xtvkcqzt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qflircmv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3uervwcdz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3dsrexqor.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3otrhkwcw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3apvtomhv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3cfhzfgir.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3sflittie.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rmxsmmmp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rkvtpqbs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3jaotywzs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3syqpyffg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3bqwwtgvo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qvoyhmtk.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mcljwoik.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3kxfgkvlt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ggyttwog.html


<!-- 参考信息 -->