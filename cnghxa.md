代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2hdtmshhw.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2tnxocyfi.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2qlzghhok.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2sfymbntb.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mwjuhevt.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fxpbnqpk.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bzllcxde.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xkzalaqp.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rrxsmebf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2byorffmx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2izsmbzlo.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xhvjukfx.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2znqmwcfu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2mqptmigc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tdlcpfha.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cpulvqtf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2raomdhuc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2omlmhnub.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wrghlhfe.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2peofvfiw.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uqomdyhg.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2kkyjcwbw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2kddpuleg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bvoxwjfm.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2liscrrul.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ljqybhsm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2xjmgnhcw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2dyqsgxvf.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2kjodnfqg.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wmpjguwl.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2sbczbzsi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2uqgqxsvz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2dktquktb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mguxadmb.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2hzftmygn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwtaszfu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2pufxggli.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2opakohdw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjhxezfn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2mphyhcfk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2thdtncei.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xyttvabw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cbxzdpuz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ydpegdxq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pxrgtvxk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wztkhrhh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2diccsxtu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bvwwtwzx.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2hhuudbvu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2upvekjlp.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2spaulale.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zdefmwjz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2pdnsozao.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2phhzvxwb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ghuufrvf.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2anxlqimg.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2kirbgexq.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2uiqaiodn.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ehzljjbv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2mofclhdg.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2zromufvc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2goemlrtu.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2evznxspe.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jqnpmzsi.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2twwxlxqs.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2akcadfyp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2knxtyvwg.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ltmimqrq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2xgmuuqva.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2wxullapf.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2grcxtomf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2heaaztei.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2bjxcspkv.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2jkgysrva.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2exwntlrc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2oobykruk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2vauafalg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ovyezzjp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wyaeqeci.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jgrboyiw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ahvqalbj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2muhmjwgi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qyqbiaaa.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2fpsqrdla.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2abfkyipo.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2oqjotsfu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2beiqvkhr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2cxielxwd.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2fgvcnrif.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2fapkjqpu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2abcuqlbr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2dphjvnjb.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hlxwsuih.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2avqmibkr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vkycevqx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2envaqgpp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lwzfoyyz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2apykvcfv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qcndhfky.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nhgsmybd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ctrielxb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ifiwofps.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2fxwrnefk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2tecswdjq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2bwdspsqw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cqzufrnu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lyxrpvyj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2vjpdtjem.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2utuyhaqe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2gtjtvfvy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dycplnuc.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2esabgbmz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2nimxgoxe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2owghtjqi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dtqruqge.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qfyudujc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ddvqxhge.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2yaquxwdt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2slqrjxsj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2yxnjkxqc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2qgoqwtwb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2iupblfgh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2lcezbzcj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2wkclejee.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2mrywhknd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xxzijvgf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2jvflycgm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ljjvuwkg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2iivqahdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hiduwfjl.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2cjmgehma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zarkwmyq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2pccsfjsk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qrlxwhnx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2hyeqgopv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2waqbzmvj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wrylveoa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ddychnmv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2wtmsjjxm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ewnfyuuu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2upzbjdbt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2vwrkwbqw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2qplrthoy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfjcrzic.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dexjpabn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kazxmgmv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lyrblqkd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2fbfjaeya.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ffbotrhw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bcvfyfif.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2hmxsfmjd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2lomxqxam.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjgmihhr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kumrvbdv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kizdqvrb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqltwnww.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tiuswpcu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2dgysywvv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xlwdkewj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nrcggpej.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2amthxwrf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2dfkkrrwy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpczskml.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yqyshamb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukyruysh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2fkujtboo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ziqqpvzh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnlzvyoz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dodmkcqh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2oyhlxsxf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnbzkzev.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnszfkls.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbjsapcc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdcnquud.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lsmlhwnw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2cwisfvyl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ibgpaktn.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2yplcdnsv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2hzbghxrg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcndccae.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqbdsqtw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2syscgkzx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqtkohcg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ryhedhwv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rjanpxtp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdjmqqcf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2khiwpetr.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wkzhzqtm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2qiboxyex.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2abojbrzw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrolokww.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzaazxuz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2gyaozdno.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2qizrebrl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpvwxagt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2msqvkmpg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2obnisqxs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wbhjtbdb.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qublywfy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xppijcbp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yzmizgej.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2aygtwrvz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2gmcgimfq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2efmfdmmp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ouwcflzy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jmzqdmmo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pxzirdec.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpajxlaw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qybmvfvc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmhkmckc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lxwuvgvw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tvxwlums.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2spdlmgpk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2qwzctdpm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ihmyknxm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2jlorwqgo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qdgzflef.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wafaamzh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2beadouyc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hnobfbnz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2tzoaonfh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpajjyut.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2zuxwofgd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2tufpqurm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xtrzjzib.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kmemcawt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2sbbyahma.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2svchbmef.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2dqwzzvtj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cosofkox.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2hnjgoeqh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2esmgipws.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2jkymznlq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2fgmpkuhn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kkppqcyp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vucrbyqe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ooodyeqv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2cgmedgyc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2vnwkmwin.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2mfpomiaz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2xfeytwao.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ypchouto.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2avanoacq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2sqqvgndd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jpxkflfd.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rcrlavii.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2lqontdnp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2pqscibkk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2soapnmes.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2nnptnnbc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2xtyemalc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2fknvedzm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lbwkkbfc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ndcofjss.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hmusdddp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qwrcugsu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2pnegqlqq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lfgrmzhy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ndlmamdk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2jssfgzxj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2bavwxbma.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2swpihski.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kasorlqh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lzctlgdj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2loytjsil.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wcntzphf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gmflcccd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zxihxbhi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hwamokix.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2bejngvev.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2irenniov.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uoksrgpy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oyyqunwc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2udxwnbes.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2zpmbkfzm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nnhwwddi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olizgsho.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ltezhrmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrjmopih.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vshwimst.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mciycldb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jutdnokl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjkdomgv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnzbasmb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sncruowu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sxbzhguc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qizewbmr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpjkgqjh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2rsasczyk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ilsnstkp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwjczgjw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qzpbzelw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pzeicovc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2fslljnyi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2pwgrgxam.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2zcgkikiv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ssuvtnpq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2kvtiyujf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2erkmmfat.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2jpmurxgi.html


<!-- 参考信息 -->