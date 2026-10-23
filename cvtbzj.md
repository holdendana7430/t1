代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bffdznaw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3myjfumre.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fapaslek.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3zjivrzad.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3dwhigxja.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3yvcpkrwr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3hliizxib.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3rfptuxuk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vvpwnuxp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3gswzexui.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wgalyvmn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3xvkmzszq.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sseuzyky.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eaaslcar.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3usmnjvih.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qfedofuw.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3knqrbrxn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sebhhjxg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yklituqc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mqkqzcnu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3nplhdksi.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3cgmrckmu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ahqpbplw.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3iwdedpni.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fdlqyabn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3niqjykjc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uofjjqff.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3gkkjxedh.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ncugjtnk.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3bpsgkwhb.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ujommcog.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tvzmkomk.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rmhuvjpu.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3moelwhqz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3dhfuwtrj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3benohgfs.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qaqliaqq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jnmvvlrl.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3eleaklva.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cyixdkkr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3yjopyyjs.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3inxijaud.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftpcfaqd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3mjmuirgf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3gpcuayal.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3pvjifosq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3icgbgbyl.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3gmksnuea.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qgkrcmlj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fvdbrsix.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dfvbqfjl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3febohhsg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kcdiqrhf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3udlxtssd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lcgdqnfe.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cuslcfxx.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3avcjrdae.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ofswptce.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jkkflhji.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ydzhsgan.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3puwhuhgt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3szrrmjzn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3pwhzaoou.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3oictjxdx.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3upoaowyc.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3sdjwipqt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3llzzqiwu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3pudihshq.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3dqnktryl.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ixynovwl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3qyrafpug.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lynqvhiw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3swndzyio.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3uidjkuaq.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ekqquprf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3rraslgec.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3shjdcosm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3rvnuglye.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bzfdmmxe.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ghvcqjzt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3qujupytt.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3uubgfgbt.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3lvumpedj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3moxoomwc.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3mbgmqxrn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gwflaeqr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ycovabvd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypwieqtn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xesvbdgu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ufzfumbk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fqmrvzvf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3famyylsj.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yrrtxpvq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eqkbpdph.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3zfvurgjy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3oqkkdmlv.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vrwdveed.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3lxehcofq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hnmhjzmb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wuvcmtbg.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lytfbfkn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wjifnixz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nagvbwni.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3dtewvpsq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tapcrrlp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3eeflddyu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3grhowfmv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jkuuvwhz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3sdtibqzx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3gaajhyer.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3spdzwdrg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3jbhdybue.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3msqbyvpl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3livoegpp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zjhcqoui.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3tpbwmiuc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3nqhqrdqv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3uajrwvcl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bfjerlav.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3imrlixmm.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3nquyguan.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3prsgzmjd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qiqowhsp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pyuyorwu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3eveyglpf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ecpyzajo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3jqxapslw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3sutrekrc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3nubecntj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3tmjlbpho.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3rqvfdofp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3nthgqgog.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ldljunfx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fymdxwly.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ahqeasis.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bymsiexo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3mlniviuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uotfxnba.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3kssolzan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ymmbembh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3joeeporv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3pwlswkjg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhzsfzeh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yludjrug.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ospmjejf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ukmlihvs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qqjcsaqn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3cixyzswu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lvsbpezx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3lhespvod.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3fcaosqhc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivtxikxs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3egmozltl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3greohrfh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lcclakvx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3jxpashgs.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3tiynnkzh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3petilini.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3shnceylp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3yllwmyjq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjtzbzsk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fnsnvyqz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uiolrcpn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cdxaeqda.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dmoorvgq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3jnwckcna.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jzharxip.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cvwptotb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ltqtjowo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnjwinqm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gweubskh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bamgdspd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3yxyifeok.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3crwvhvlv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3fhfuvqqh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3tssuxodp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3neskovwk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3hkqxgdrn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vamszocm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqccplke.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxrwtizr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3skjlancx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3axqwjgvt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3pafvreja.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3iytupxum.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3yhzosbfg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3hiszwkho.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3efpajwhe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iqbwepxf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ruafiofs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3xidppavv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3obtzxsyo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3yayfyrho.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmohdxlw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3nmdhbhmy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ptsadict.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3evhtbsej.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzktbajm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbpyvdyd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3juethikq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3khxsreke.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3nmekudou.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rlekkhtj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3gafymokp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3lvplgdxb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vtwpsbjy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3locslayv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3txaawsgd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aybdcgml.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3roirpzwg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3makbrdnz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iljrgksu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3dnvqklvo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ipbougzm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vemzutlp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zlzvjjqy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jpalgsce.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xcnrauxp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wfeboksv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3hpmmrujg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mibxqhwt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3mvnjkwdz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3odlqjdcw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fochjmby.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3getqjvvy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hhnvtlsj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3foektalp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3hozxnotd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3bhlgfhar.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghrgbbmq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3phgerpbx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3idtiapiv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hhkcboib.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wdbdznoe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lzydzkzg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3urlpehga.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3zoivbcvz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3flvocaoz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3fjgvtkas.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pgeyjiiw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3hfhfftwj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bnwuferf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fthmqifh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3whgwweeq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lqukousk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3dfwtrphv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ujqgsqoz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3zoodrvdh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3wbyvnhvp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3birmhpoh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mopfhlxl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3sksqqjuh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3njjohhgp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3zualbtny.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3rpjjyldz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3qsprqrpi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3fhikpivy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3etbrrtiz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3cnhpcwck.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3iokrceqp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ygeykvgf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nblkpmtr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nyimiabi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yrsedvby.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mxrqvjru.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wohaikci.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3bburjixq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3mjmiljkl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3eqjljzov.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zpiccjil.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ujcorflv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yzrwpnvq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mhosjxlf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xtzvdbsw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qmonmdag.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dgozqqvy.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3nsbqsuze.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwidhabz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3eenzggqd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3optkgbic.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3behpnwfx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3xbdcchor.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3yssymipn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rppfhbrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zggnsrxp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wonpzkzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uakxnwvn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lellfeac.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ndkasezm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucmoqtpy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kusozexb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3owwdnqkt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydluwbsq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3iflxrhee.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hvwemglz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vpxktltx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ripserbe.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3kfvyamde.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3tttkybtr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtyjgvzz.html


<!-- 参考信息 -->