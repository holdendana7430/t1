代发 wailian999

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2tletbxjq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2erzpxjlf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jbknzlfo.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2takuggyg.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kxoesgmy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ofizasxt.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2snjiskkq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2vlbfklxw.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2encevfou.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2hdlalmix.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qkaquzrc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2czikrnaf.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2asophtka.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fmwmsgzn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2vtefchxt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2cxbdbjfi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2bwbtthrw.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2iaxshsnr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2triwmgjy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2yjgwhbed.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2uvnzlwrk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2untcenxs.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2rxodvmkm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2protunxf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2nwbmppik.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ztzqjmuw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2oqkzravx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2doeckmoz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bwsauwlc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nvsizcau.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gcqosivz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ksvgptea.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ebewpuen.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cfbjvcgj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vqevdniv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hdheowye.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2jubaqdlu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zxzcphcu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uusutqwk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2whvkqmav.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ephbkajd.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2tqqksafy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ealcokwj.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2lridjaws.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2bnforesk.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2mgybsnzy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pxcouarj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2bszlunmq.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2opjxihdu.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2pbrhlcyq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2xlrsjlts.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2sjfgqhmz.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2abeoavxa.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2jkhxtyet.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ezhabzkb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2qmkvjqdz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2vbfzwmpm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2lfegjfxd.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2uabzwzij.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2tqgbaglk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2saalfzja.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ngtpjbvu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2reljavuc.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2fkzvzlnh.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ddrwrpez.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bfnbtqku.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zacdfsyh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bmupmlou.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bkqqckei.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tlapcrto.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vqlazdtl.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2syyulcid.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tdnprnkk.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rxjhtxde.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2dsfrbeqr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2cnpdzbjj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2zdndgqhc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2enpneblx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2muuidipm.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2dlydzdxz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2gwsgumof.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ffhkmfcj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2usyjwrvs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2puxhqyrt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2sufalfwa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lfhjfwvw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ovakaebs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2cmkcdwwi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2sqolnyqs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2hvnnsfzx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2lfrruxcx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2lttizzjl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2mynouhxe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pygjqwtd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xvqjjkiq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ssuygmqt.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xzheokxw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ousntudc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fxadzlcr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tllblqlv.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2kltpgkdf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mwaefuld.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zmdfagrr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pczdtjwd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vlkgvfsy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2gcctzzjh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2eajzkehp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qlkgthkm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2tnuhmgei.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2monlubda.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2hlkfnktd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2oojztmle.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2npvxiany.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mftvzjfl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2htwbgyxo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2iuojjqyb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vcjdjtxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gszgwzii.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2dweyewtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xelzxuns.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ssbgbicc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2gffiferg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyihxiko.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kjebccsm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2llmdtukg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wlfaodvm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ioseezmz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2bfreirsw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yoqwmxhr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ffgubkov.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2jvpzzcmz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2jsklghyw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lmsmxone.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qaufzbqr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yozsgzpp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2nbcyfdef.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2gcowkttn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vhfrxcgm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2spgndaam.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ewmczthe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sneusnmd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aktwtlis.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dnwxxaob.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmpxejel.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kxfppkno.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zdbggwmn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2njyfjqin.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bnccimxk.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ojswutxw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2bcgrauin.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqqsohcr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ffbqqqur.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ihjkshph.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mndtnaqe.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2wbtrtfcc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2afqnfnzx.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dommyscr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2uebsyhze.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2pftemjgn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2drrqokgt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2stifqqam.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbpuyuml.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2trtuhlep.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2yueqnjak.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxgluneg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2danvhlaz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2vbbermio.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmbgrlpx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdavyxid.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2sjqwnuiu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2acrmqjds.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ntofvtof.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ebkedyhl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2kketljxt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2wjilsoke.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2xmmjavdr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewuwkcti.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fvjkgpnl.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mgfkulpw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eedqkcep.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2znyaavjt.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2cnblsqpe.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyripngi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2bsardcrq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2jscuccnr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gavldtuj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ikqfadzt.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cnwkqsue.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ldavfxug.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fwccozny.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2bjygtvbm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xfygdxzq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2vefnyzpq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2rwrxaeai.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2viacahut.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dahuplma.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cctlnhum.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jlyrfspi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xyjugdqz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ntlxvmkb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2awswwmse.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2iqjryoqj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2adbryaxf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuztgvsy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2attertjx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bbiwdcqc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2kutsemen.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cejymagk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2afvgscwx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vvubcumk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2maxwduum.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2cyezxtpi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sfmpwxbc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2njvrzhit.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qfdubays.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2edbrficy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2uyqiubzh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2myzuqfxz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2juqmocjw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2feufeofy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2yxtfzsge.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2nektnazy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2neixthew.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vlnmdyib.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tjjaublh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qwbkbaiv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ilflqspl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2yrelmuql.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2njmwtvwd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xofttrjy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2lejvwefg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpaeqmcm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xpnlivmf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2hfywvlfa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zbllhfvj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2bcnjettn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2etkgvwhc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2lnxarynj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2wwiltjet.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ewevysfh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wytmwilb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ofviofqy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mndujozm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2axgrpbwq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ynwqimwu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jpxarzcn.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2uebpgbbc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xeujzham.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2emlbqazw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2exujjdwq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eeeqgjth.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fkvlsnuk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bxyjbujj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sdhfzqtx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2crilrezs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2coeyocdu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2oyfclady.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmcpeguy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2orzzaeof.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ipobyhgc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2htooqcda.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2esatqjzp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2qjxveyzl.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ovejttfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggkkphgi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jskmrtkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlastygx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mxlxfdjc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ehzccelk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsiuttdj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ygtfyvdr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwecswmd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2faxajdxs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2nfvqlizf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2lemtjcdh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rlnvoexq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2vnajtzix.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2iupczoyg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiuvwfdk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2smzejxud.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcmekjrl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2uiqfwqzx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2xfuzgpds.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rcadopzl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2juwpmjsq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2wlqcedyf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2scmkhtaf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2xyubfkus.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xusfmafn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pcujjvwg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2idvhrbyh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2jbtitxub.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2qvjwfbng.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2khlwxmrh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2htzdljfg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2yzaoexow.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ijazjqfr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbluqhrt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2khtcywrr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xbhxuake.html


<!-- 参考信息 -->