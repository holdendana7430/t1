代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3hxlewlsi.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3apqblxke.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3myyqoyhf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3masenjwb.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ntnmueda.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tdiodutw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bshvtvjy.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ceqyaovj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uppkfjbn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gegzqvxj.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ihswqxuu.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mifilcyc.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3dmhmhimg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3rlpkhzzs.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cnmqxinx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3txlzphrw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yodgpvaj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3kpdxrjar.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kftmvszl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3peedtcym.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3molylkgg.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3fbfgjwzs.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qyudzotb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lehmvzyr.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ktdetocr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ddomyulc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ylxuumkw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ieblhfxw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3bxvdxyat.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dnfwiqrj.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3npricdoq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cnkcsieq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3osnktxve.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3skalxlzh.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3obphafnv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulpcfngc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3chogabos.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3roybkrbr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mezvlmly.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ofsosjui.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rsfgycrc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3siayrlnv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uxkagmvl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3knzugpyp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fsidtity.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3edxxvvqj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cluxvest.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zmojeflu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ebaaqfsd.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hihpbjzk.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vmgszbdt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3gzabydjg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gjdprsed.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3vccrledl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3hujywsfq.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3nfkuqexp.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3eaxiuoyo.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3qzhjruue.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ijnuvwbt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3nzloxytj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3dnximgck.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3craxszcd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3tegmionu.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3obmuvvmm.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3yjlcwrlh.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3wtyikwgc.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3uuqcqxeq.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3vgmaymeb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3gjianfox.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3aunzyjbl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3gnmpepfk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ivtnwwgy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3tdmgdmfs.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3svucxqqf.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3hxssutyt.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3lviemhwh.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3syqqmnox.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tdfaiaud.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jjvumucr.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3aykabvgr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qodxpccu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lsomhlas.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3racfsmdi.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3xaanyowc.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kzbjyhnv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rtswbxuo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3lkjpswku.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3soklfvju.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3gnlnamev.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3htosuvtp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3hmmeoyga.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3snlbdmct.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qyigdnzd.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gkjthnvn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3zpjlbfaq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3pvngkgfh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hqezopkd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xamxqglt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3myphesme.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3aerttsic.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ckhlkhss.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3gvcsbhfc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3yzuhjybo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3wzgukfyz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3kciidaau.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zgdnwrwn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uuomejyz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3dsjflwaf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3egvalkwl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ofseadit.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3edxxftdr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vgevlnvp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3vnzasgdk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hznpwskh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xwzwcmjd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3uhixfcph.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ihzsqyez.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ngsteylx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3vlwnkjtf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wmsgwiga.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3dwtklths.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3wnzydaet.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3zhwszajs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3gclszksi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ogewtwfn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3btjfotna.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3cfexkkxz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fnhjknjw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3optzrxyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxwjmfay.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3bsqbgahc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttlhvepp.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3fxyuodue.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wsjjtxjl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3isxpzoio.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3awzjjfgw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xczpnzmr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vgodtmdm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3lpfrsjhb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3fwypewku.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gnhsxdff.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ccwhuvli.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3xrftetse.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3rmkteamr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xuytkjmx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rxwyeemt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3umtrmytu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3lzrbwcus.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3gyiitbmc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3enibcepq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3rodqyhpq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3zkczxosr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qqtwaffy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tesrstap.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3upotztwz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcjsjeac.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ltvubvhg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3idvgedly.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rmismbow.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vujsmffd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yjnwdwok.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3viutbagi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bmxjbhcz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3oblqrcea.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3mugnjgwb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3grvbxikr.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3zzdadgxm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyggioih.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kqkglblf.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3xeegmnqq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3abzpzdae.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xvchnrdp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3elcsjave.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3qcfmttig.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3lwhxmenw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3tybfgkkp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyaezsvv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3yvcryocp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3alruhdna.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3nuruvdlk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gjjgpgxf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfwejndi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3vuzygtni.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3djtgexep.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vkzpmfvj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozilgoih.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3owazmzll.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kxmivcxi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3vcilkrtl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3trhniufc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rwoyewur.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tvstwmjq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3pjxxernb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ndpferrr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxicmxfo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3kzraswhp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ttdgazlw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jaanjyyv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3suqjhhla.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gjhcbroc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vnnuzlzh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qiperowg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ngaghjir.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wpcaovpz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3barvcppf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jnexwpys.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hgqifquq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mptibkqa.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ktklkjyj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ctepnenl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rputfdfi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3dreoxcni.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3opfauuiq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3vxmekcad.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vasgaztg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouvjtfqs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3mskjzrpf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3csdrlkpz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3uldqhqdc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3shohpumy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fcqosfuc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3pzbvdxni.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ngvqhdkg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3aqmgvrgj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ynhctslc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3kbygarxv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3oeowjpfm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qnlvtrvm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3pfzydnto.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3lvnuixdc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3xymiieez.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ctgdllws.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3bfkiidbo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3goxiedba.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3baustxwk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sslndkxv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ghygynzb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ocofcfck.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3wtekdmlm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3gagqgmdb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3npvkeazg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3pfdffxtc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hhcydclg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ilsgsioi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yaxwnbuz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3vmwmamgr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3tiuhuges.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3gcyohqor.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3gpxhzrbd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3jvmxwecx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3aojoymhx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ywfamnhp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqbvgecs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kgyyhqpy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3whbfftjo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sxgfigjn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qlpyckzk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nikyozam.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3caisueyq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3wlmgtmnz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3cyznxcnp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fsegjpwu.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hcwjxtno.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ymtnycvm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zxpyqubl.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eojboqgd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fzqjfzlu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3zdsdgoap.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3eqscnzpj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmoxiyge.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kgcrveqa.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3auoiiwyr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ybrjzlys.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3dgjzwibg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3lnrbixrr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3snfkfnor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jydnpoyn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ykmkyctz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwagwiwv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ukdkmczi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3edwhdtlp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pqabyfny.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gobaguew.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3emakjyrd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aivzlegt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3onndehvq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3cdcfjqvp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkcenobu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ccljvnxw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3cwrfzqei.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvdpbpwm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zrlgtlpi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dbttvdht.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3qbxgsfaa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3hsnvxadv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xqogzega.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3xtetgxsh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3xophtvao.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3oiwnueat.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cdmcnbva.html


<!-- 参考信息 -->