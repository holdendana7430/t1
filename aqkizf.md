代发 wailian999

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bghsrbzh.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ihlotuff.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cphziydx.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ucbsuwmz.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ocremcku.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2hzkojuzh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rmocqwxz.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gsxstudh.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ifspekmh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2nhnfdhce.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cgzommfo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2qdmpvozc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vpcjvpho.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2tbxwdjfe.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2srplzcjy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ktuvrywk.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zrhuruua.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2esezhgtf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2budsytoj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2qguylcjf.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2wcbalkpe.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vzrmirkr.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2zftzydsm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2yzytgdbv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2pscjgspo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2vkimlite.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecbnrtyl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvwpbqec.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2qbhyicbs.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2zwmfbgur.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mezykgqe.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2nqkqafze.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uoyfjjqe.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mkzfaosk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ireseinw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aznwwkhc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jtonpaqd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oicougwr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eabpbgow.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kmrvsrxg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2oyeeusip.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2uzjiizxk.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ldbcytkk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2gkdsdgwe.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2qnugrnqt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2aqskjxwe.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2qipigwsk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2mkxmwgkm.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2kdskzaxq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2fhajcsux.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hadhcvxe.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2zutwknjf.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2plccfhdn.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2yicsqkgl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2zxofroie.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2frygimqt.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2byiopggt.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2blmthrai.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2bpzltnse.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2zbycgzcn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2lldjyayz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2zxcugbgt.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jwjohimc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2fujvsqiy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2onmsogwa.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2vfhshudl.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2pqmfgxrz.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2odxhbhnm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2neinobft.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mqqbitdh.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wlktakbz.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fliqxdld.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hgfwqtuh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2myuscono.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jjsahykp.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2hscbisnt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2osgurmsj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cppiehua.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2duwxijga.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2fnqwpprv.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ydnavfct.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2lqrxakxb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2imdmmqur.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2icfezyug.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2lesvkgwk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ioaurtrh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2onmixvko.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2yreciybb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hmmvusei.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zsanmqxr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2klpcfsck.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xvtrhuuc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2abolxfbb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2lbmjyaoo.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2abmhfxhe.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2rjmrarkp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zrimhuem.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ffjheyko.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gnysykgk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2oebuhdvs.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xewqzcgd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lxdubtlw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2txfitcye.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cetjhjkx.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2odococvm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2erhczdge.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ckxaumyk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qfivpefw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2unlhpsij.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fpdhwozb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2klczsmfx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gatpmfmn.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2zjthmoge.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2qgfqduio.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2gcsoskif.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2kpkpxqcw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2steyoiya.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pwpmnphk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2jaytgxxl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xnycjvkp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tjnmwzup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdzlmbud.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2olmyeffd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akhhjyna.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ktiwsnzg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2zluxtnhj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhgydiyt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ilphldmb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2txkdarat.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bddwmdlz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2klpjqbfk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2fyakshvt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2eaiedqsn.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2dxdammmi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xdtacjtt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2urfycikz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nyfbibup.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ewvxjhku.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tirnoiqa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2kafczwxl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2rcuxuwcg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uqisnxab.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2rvimlwtg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2zzsavyif.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bksmiwhk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjdwutgm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2itbtyxrb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzzucegn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2dsauzdnt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2klmuuwcy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2omhugnke.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dcfmrldx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2fjnfhftz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfufqmsm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgmuspbg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2tfwlsfth.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2smctmtqy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2qzbgkkdb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2svpqfrcc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2dqvincur.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gurkipui.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2lafviisv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2fklvvthe.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubmnvfku.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mssdxoab.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvodvact.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2kaitvcyc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2qingphif.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwynvvms.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ezavfuko.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2fptbqgeg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2elixptyl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzpljxqw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tqxsofaq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2frgvyclc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hgpvyyny.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bfazhrcc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmnpgypl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2cjlnsnfn.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2idnunfgi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2isqimdom.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2peroonqu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2opvopebj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iubykazo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2cdezkiar.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2mciuokpa.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzqwmgwo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ishsnnfq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2dgslytbl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ndiewgib.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cjbkbtzg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eyvurymw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2awbucjhn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lizlhxhz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2icriioex.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xmlpqbic.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2rvylsaxy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2vfewylpm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pbmlswxq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwvrcewh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rxevkhdx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uvfehiay.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2timbrdof.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fffthjil.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2npewtlez.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2rllsnprc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2oifqtdcz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdjcmbes.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lvxsulwa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ncofiniv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2djdjtywm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2azxqdhpj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2httnmiaz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2jxpjlqmg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2mzulwzlz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2spwogjgr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fexmgzft.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pxaohtdy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hlnwyxli.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2viasimmq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2gfflvxzr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qhxizvwz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kohpsbid.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zpcnoany.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2affpcejf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2taoxpdwl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mybcoyss.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xfyjdnka.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dokyckwy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xeurnmra.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2dcbtueou.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2btmawmby.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2nyrrvoxo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2drfizybs.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2rjiolqaf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2neioustx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2kyashclz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2bpcpvmjx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2tdfmauqv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vnledxzx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2bdrzutdj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ikcwzonh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rxlqewgx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2qkfprenr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2csyqrdjr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hmpcylvx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qcitdcbi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ptzhsswh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2izdpwvcr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2axywvoac.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ouqtcgqd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2llcnhicl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2sdfjcgnm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fczeghmp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pttpcmdb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2soubtnst.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2amernity.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mxxfuowv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xxlsxnvu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lkrgxtuc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ybgurbzv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ycpduviu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2njovmdeo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tqhvqezc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bemvnprh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vkgbpnku.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2irorpduy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jvvpmqzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uenizbbu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dvefxsdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2etnmgzbk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yynohftv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2pgctphja.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwrgzjoi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywdalvwi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2krvhythy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kroskrwn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2qzmwmojh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2iffhbtwx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lrgnkdqs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hmqbexia.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2htlimvod.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdvyreil.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcerlmid.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyrtovyp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2mxtwdwob.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2wlznvqkq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ahocqbpl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2afqhwspe.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2bemvjvuv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hpxkhhnr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2xzdlptud.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2oplzlzkq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2icscmewr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hhyqcpzg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2udiljzpu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zphxfvwi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2cvdjqzkh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2bozmfony.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2vnqyaowz.html


<!-- 参考信息 -->