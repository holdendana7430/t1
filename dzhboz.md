代发 wailian999

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ysrzytyv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cvabtltf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uqlucefz.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3utjpbhxn.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3etxlxwes.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3rhvmlpnw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tenaskmy.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3inwlklti.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rxhenshy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3amtmdqlo.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ffvaxqxj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3aklmknml.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wiodptah.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fnuzxljx.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3vzmfhxeh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tuvnwgvg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ivuuyxyr.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3apcjtpvq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3yfxpegsn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3tniorouw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3qazevpsw.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3frbqwdle.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3cqumvhrz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3bydengzo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3uplfpmby.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ujtffcyf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uoaijlkn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3srnzlvti.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3npmrckqh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3nflpwzjn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yagebyrh.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3xpbogfra.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ozzzxqsa.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zimorkhs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ztywapuh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zuelyjoe.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qzyjownf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nuqnkxtt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mlnclpyz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3untzktio.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3kfudqgbu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3rzvnavqb.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ljspgqdz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ueuvrght.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rxqgxrch.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3jbykompw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3oipgnftw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3utanfifj.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3yhjbobzy.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3jxobktkg.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jnckvhmg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ispjuslp.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mgvvjtjd.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3oozvnphk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3lhldqcft.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3vvllqdae.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3oepvgspc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3hwsgxlgx.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3hglohknt.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3oxbxhdxr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3cmtjbzyr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3tbpgwgxk.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kpnlcctt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ehvcwdeh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3csmgszsk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3gywnosrm.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ogczkdvw.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3uteolhcq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ktzhzmae.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3quxadeco.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jmmswqre.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3adnmevjp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wgullthp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ifzlihyh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kektyvez.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3acfvhbgb.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uinseivo.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bienhlva.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3fxnzyqhw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3uyzyfpmu.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ywhrpuiy.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3vgxssrsf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3fmdwydhq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3wbvvsyrq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3fkkkvnir.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gxrncjau.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3zbumafwv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ptcuhyjd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vxhqikzl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3tjjqaluv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hjseaozt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zxuixkiw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qazagmzi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3yfpjepfr.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3rkpffssg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3fudjykxe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntpbnmfh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bvyfjamv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jgjbiuuc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3amjkzudo.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rvkdndih.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3unjtaduu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lvkupudq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hncdexmj.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ipzlehvb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3athyvwse.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aymbnoww.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lxpdpdze.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nsvbeuri.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3quygxpif.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3pxndugst.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfyfprfp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ioopccfr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xopcdnts.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3kdvughic.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3booyoyqh.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3qxzivnjs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nuszrtrt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ynodguqc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3hfrjrkff.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3cxgpgugx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmechvfp.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3qofmlzew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttmckvat.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3cdolopde.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3dzicgbgu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kachrsgl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nofkykpy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jevhhbkm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ccihhxjv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3delnbfyc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3egqlzokc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tosnirnc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3dusbznzl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3oqyinyml.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnbvmajw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kaooleuk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xwvyckbg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hvqinsqn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3hyktelrh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3mdvecbnm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gqngmukt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3wkimvbdy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ixraunux.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lzvxyzqx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnipbpcm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3opoykxgn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnychoeb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3twlosdea.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3egmgttyp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3foygnkdi.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3crjlbmdn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3xprkpiuc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3itsmclkb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nagwjmzh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufyqgvwj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejsdiqrq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3bivpbpip.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3kndyynuj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3cjhikmrd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qitrokgf.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3qmyiuuok.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3stjgbyve.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pxirmauq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3qkvxnqou.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ztnrmhhv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3oyhsdvpw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3cltsqyzd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3pzvaxxbz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ixdmcupk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ftpvdzyh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxnpigia.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cuormcmc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qxbknjwz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmljlxsc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3shiuezlb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3jehmvdze.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3fmmfdmhm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3zdwnjvft.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ckddpwyk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ijwbrqib.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3twgiwpiz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fziqxgam.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aldvsdil.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3koljevnw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3qjbfceaz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uychgxjx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ccqlkgij.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3tmjaumuh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3njjlryou.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vxjhzudr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ilwvujlu.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iuwmgxwt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3djqndsqw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3honejzkn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gifnyogf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3gbuqqjyy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3japmhqpn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jrdhheas.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdqxnqvd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghozfexa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rasnziue.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ykgplyit.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3mhuraciw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvhekqzi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3txozhsmp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qllpesal.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucrmqpyk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wvbxjeii.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mskgdrql.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3djayzpix.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3mfxdpovy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mqsdhynl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3bsgouwpp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3veqczedf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3xpnwbzvc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3kwfptlyx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3urrrgors.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nfwfbmuf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3mlwywayz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jtenlzif.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qkljfofi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ksernmpd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ruzotgtf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3rhrflpnt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3dvobhzwr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xulvwajy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qqvdoejb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kcydimzk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3vrcywwxc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3cfypkakb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3tmjqezqv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3lshqvlbc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3mquiqbfp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3yhmsonad.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3khiywhwr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ctevbvmp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3awvfvjgi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zkfslkak.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3khvmxjyn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xabwxvhm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3iqcdezjh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3hnhecpkq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3tjzjbfca.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sifqatgr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fkhrjtmv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oxiflvmz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3tqwxwzbf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3uljcmwsi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3skzyjgdr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3jqdbbdkf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3focjmmpm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3cmpguabk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ifvkphjh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gnkjyity.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dbibxyhs.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3npsxdfhb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3itplqmna.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3idbnzaky.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3boncgdtz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3kfxsxgip.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3npdeafbm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xitlwolc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jgpgihox.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rnawnqnq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hutkeqfe.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3hxuafxfk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mqhfopzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqliiqpu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3qifuttio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unuzmbcy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jedbsjzm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3tfyrqluy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsaqrhmd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pkviowly.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngqlxhlj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wpagirrt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3paqzpunj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3utklkuwg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dpyynfic.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3puiczgac.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3odmniqsy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3drfytuyh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cmxihzjz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmsxdvxm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3qbgqpgpf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3sctvwncv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ojnnlafs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3gjprjbro.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3hvqwjoxm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3rjvxtsrm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3yitngskb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqjaqxzu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3itvzsoht.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ukwlvaiu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3xkmizbgs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3cmhvimcw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3gxtfqvrt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3rvqcqorx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rdpbqold.html


<!-- 参考信息 -->