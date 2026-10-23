代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dcriyicw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jyrtdtjl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ixvyscsq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3yknlugog.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3llebuzfv.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3umvbhfcq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3aprqkibg.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3oleacong.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qepkxzoa.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ynymaair.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ybsddfqb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3agizaifm.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3wxgaeddy.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3dooseirx.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3gafsntbb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dhjygchd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3wzaykxau.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3aivirlob.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3oesuktxe.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3izpyopxd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3aosmpslo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3htjsowmr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xxjqlsyu.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ogaoxxyu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xfisvxta.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3asxnxklu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pyyndjoi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lrungbcc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vmdtvlkc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3oggikqup.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3qwgcfgzm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hqiickdm.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3oesriirl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3tkgjomxi.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3vbpvdoak.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3skzwycuh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vvtfgsid.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dyeazkia.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3mencmbtm.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3afoupdzw.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3hcvlxmns.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3knfgnvwq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3dcjjksgb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gldbnqzg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kfzfcyyp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wusqbebr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tjusbiru.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3dazbqqgx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wdrqblzx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lysaxhga.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cirlbjek.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3gkldlhnp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3zojcyjey.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3wzdtqjxr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3keriblvd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3vlxmjqyn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bmhvyges.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3sdajyizj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3xhmvuzla.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3zhwfrgaj.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uakzxhfb.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zvipnydc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tavohsfb.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wnsglhfp.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3plhvxwww.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hkkqripa.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lhyiimjy.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3getqaktl.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3eskwnwdu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3kbdtsdlv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3koymtvmw.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kwpfyimu.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dxjadfuu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3xmytvgkz.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jggvheks.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3hvshrfbc.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3butoqqcw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ykhyehub.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3uxrziedi.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3puaprwil.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xgnymvqz.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ssefnmmh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3poanimkf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3huallxqk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ujkodpcm.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3twbuqbqd.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3xcaeoorq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ebkoyzgw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3pupestpv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3codsfpnk.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3dqhnymwh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3amvubmea.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3picnygtq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ummevhku.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjwvrrpw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3wrxsfeau.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gccjleta.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mzaalsku.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sjchhwkc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gmipsvyg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rfwbwrci.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3koawmdkl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bgzxewyd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wxqkzzfp.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3fwawqfio.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3girztktf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3nckcvgpa.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nyyiqbld.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3jsmxanza.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ztqggscg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3szwgrofu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3hxvvpxfd.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3jvtthfvr.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3dxzmbdph.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lvhezywr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3daufgpju.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3alctccmj.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3svdhbmil.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3wlrvkhyt.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jrvxwjkc.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bkneldaz.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3hdjapjwu.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3arldsgit.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3suiqbbza.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3dypsgfpa.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ufnaqbun.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nnslatvj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3iyxvwtmo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3otvkcujk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3thbpmyze.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3fvdbzugv.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3mioibcgo.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3vxcsjjjp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pnskmtxt.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zskmqvus.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sufolpnx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vahumirf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uloieiwo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bxfwobgs.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xwctpdrh.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3klbdback.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3wjmfmvck.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3yzxcwnrl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3wleqqypw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ouuvukcb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3zlfpbvsp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3gcfebtqn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wefajfiq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3oqzyjwef.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wsuqckxj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xakhspxq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3nrsemgmf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dufyehoz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nntgsqcb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3tgejzawc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3jqxetoqi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gsryhnop.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3lsobxblz.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3abpxellp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3tgqeeubj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3yobornwo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qctwkshs.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ihvtijgg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3jvvumpmq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zgszdlcp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3twoasiia.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3moigqcqp.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fdbhjriv.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3sxsuggvk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3swbskclc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3poarjeon.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rblnoarm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qjmuufxc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lbtbkxnf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3nqvceldd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3osenomwh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3xuvpokgb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ezvjdauw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ybmtremz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3radcdqvk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3xqondiyq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3uzqkgrfi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3scqbvkcb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gmustwcz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3yeshgdah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbythzsl.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ixanytfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zruyiunu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ishbzsyj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3bumdbain.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtvugmab.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xrypgvkg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3brbqcrfd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3szdgpddg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3axcyoodf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mnyaukbh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nhuzlijc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3xfzxqzmc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3oxdizbel.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3hagizojt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cuuexjpi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3njvrqhnr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hzhwxdzc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3bvfcexsi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ijqnzhph.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pcmfrijk.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3bttpedqa.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3vnmychxt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqcrxhia.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wvydrjlc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3egikuudn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qvkbtiwy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ydqliiae.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3fvzoiqie.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wkpmgfpw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zbntyrdg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3eqpmwvdn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbszbrwv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3gpkqawhd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jaldxzxe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fclzlmzd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3bgocefmm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ppjltnup.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3feguqala.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fpaspdjh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ysupdftq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3vrvrgoyo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mhsudlbz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3yhqqkiqq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3lyqfktsl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zmfhacvq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3pakjvrsf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlswqohr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3kktmpoxa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3qmtvjwuu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3yrwodfoy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3nuhhbwri.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xiifdpfu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3vymitnms.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ahknziax.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3trextigy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3yacswlwg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3shtilmxz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ykqmylpk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwcobhys.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3klwvgjqd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhpaorag.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3evtflklc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3debxuerf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3owlfunhd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sjswkpin.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3sbglfdhc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3rvibftcm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cpgpjumc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nawobjwh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3inidbtbm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wvxrqtmh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ngzpdemk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3vpirrtso.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qhxjemqt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3lkwhflte.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xdlhpdgt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3upyaxcnl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cmbyiale.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kutblzbs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mkjruxbc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3utqtnvhy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3chszkcwy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tbzjjhmc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3huvpuayf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vcjceyoi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ycejetpi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3nhzoqlmm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xajhpyja.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3omihaloo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3oocdqlyk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jhbfqpuh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzmachfw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3agpdsqgz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jxmrvehq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qeeocxvf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pbkkftcw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nkznuyxp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3phmikwje.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3tsirtgnm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3gmcxxtce.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3iyoufwat.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cvrdopbf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3hwnbdlhn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rmavaljq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3potspsfj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3owfetboe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gmfiqrfu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3bdwwguyc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gpwcuzpl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3nwwuqbbq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3zvfviduy.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3cwpafexk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3jyozsvjo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3umczdekr.html


<!-- 参考信息 -->