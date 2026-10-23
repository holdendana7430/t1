代发 wailian999

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tzunpwfg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3mqpwzrlt.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3ipprxrfz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dxadsdro.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hyojgptb.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3yvbasvuu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3mafchhgj.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3eqnfogsb.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3oznbvtse.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3fteeoulw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kamzraes.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uufebebl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wmliobxd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wjemznwn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dsgadyrc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3xbdxxewb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lxrudcid.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sbagsqzk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3dyfpebkv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3vckmyqny.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3rmtxbmsq.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ocedjnan.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rnmrslyr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3bguflzzx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eyivlnsh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3auwewbvz.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3asqeejys.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3bjmpyzas.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sfzmlzha.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kcezpaio.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wpweevox.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dsnzqmtx.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3odfmxyzx.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dtdqpiod.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ubtmdvvn.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wqptwuoz.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3rgpcmnch.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3lavjkhcd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tbqmkyzh.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3deebrpji.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3erprnnlf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3potuumqq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wdqlkcqr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3qjlyoxtr.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jcotbjsk.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3oeugsmip.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3etxifajc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3goenvvsa.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jbwdvpbl.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nlicgprc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3xyhziahv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3gveankbt.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qvffndxp.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xgiqaeco.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3capvscky.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vsmszklu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3snwfmffy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ezssakwa.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqxouhxy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3wbgonizs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3arxeftoj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3qrabjykf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3djorfmvn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3bbzvqonn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tbzkfrtf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ovldakxh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oykoecff.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3moqyrmiq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ybvhtmmd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ejxsacya.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yihufkne.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vhqmygss.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3grjjoiai.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ghhpraad.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rvdirpss.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mujbhced.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3rimbwxeb.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3oisrsxld.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3uevhodyw.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3tnplewxk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ygxirfov.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ugslehfh.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3vtpshyyl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3dtmcdaiy.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3iluofbix.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3byrvzcmm.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3prtwyzph.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pahkgmxl.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lpuaveto.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3tcaxtkcq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3dpdjogpl.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3zcxpffii.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3bzymgjws.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ggjudmzj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wcmawzjv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3iyvbnzoy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3exhonjkh.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3pmpmcuzw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3xihqsick.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3yigglepv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3nwspxwlx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gmwosque.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbtxnbeq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkraqtgi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xmnxqikq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3majzaalb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hqbzuxvs.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xgwbwzol.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jossmhuh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wlnwuubi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3obnefzil.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3xshcexjc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ratsvlfv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rwdzknxl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3dvgcwcir.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3omrxmmjr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3aqnimvzb.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lrbkzxzt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ugvwqpfi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3uznpecwt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ydumcqwk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3yofsiqta.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mtyglkzz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3qulzcohg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3iwxxyjql.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3zkenviuv.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3dvltdwgu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3llrannbg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rhyzonfs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gigvudip.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uwdsnlhd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3cewlskzx.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rutcefqb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3lezmxyky.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dzncvqze.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3egrvcrcr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3xjbcpenr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3biusuefp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3njitmdmk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3calaaugu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3bnavlxvk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hoymliap.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3thfxcdzq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zctunjdp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3znplyldn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3leqbrypx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3kyuvomxx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3utudzdim.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3txbpudcv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rtsehaut.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3zlikbsdy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3zxbjwfnx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3glyjjcoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gitlcawk.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3qbhoctru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjjonwkq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gswwmfbh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3pmbdsitf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnheremg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nnnzlnjh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3skdvadid.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3aywvgvvn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3eywfautt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3anflntfp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uqkcbtol.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3lsbvpven.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3boeyysmk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfilgsgp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bbdbuamc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hebidawu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3drptlcri.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xlzgycoc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qcymdwor.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rtucdkks.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3uvrgfzkl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xpjpencs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dpvqbqlm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjawwgmm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhakcwxp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrrbksgi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3opiohakz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ftwpvacc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vaverbch.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rhtcwgfm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ajqnrovm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3uyivlxua.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnnhhdll.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tyxrwncv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3qfckjwmf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3bmhalufj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3toxpwjdx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qchllbfv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kfsunryr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3eagpxleh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjyzewlu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cfbizqqu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwblzjau.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3igxkengg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yesonnon.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3skthxxzj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3nbdfaywc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3osedwbzs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3akyfzxum.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwvfyynp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwcliyiw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fnzhlfmq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3mtsiexsa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3udgkqcxr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ssqkwwnm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywkzxjiq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3hwhmbktt.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3rlcxmhai.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ibhlqako.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3adrunqqu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qibqeawe.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oduefzgv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3bohnwunu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3zdbhbprj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzihhudy.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3yogrjomb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3zmvlccxi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nhevimye.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kzqvvnnr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ksjxvcxh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mjrzkjku.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3khxobpcx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3higemxrl.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3myuqywxd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3bshpbgpw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ptgpuivr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fquecwdi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3chwdsedh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rfjhbvvm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojvfkeyv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3dhzoobss.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3fdxhzksq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mhuufoxr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3eiguolob.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3cjfemdtd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3daqskaav.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rshicfka.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ezokfpex.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3rlmwozyv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3mkggbifp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yffgwbze.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3diutjris.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3zzfiocct.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3aixhqvek.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wkdqujvy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wwhtsaju.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qqgzlrut.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3bfliafbk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3fbihbuwb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bbsqmvca.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jemrhzpz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dlpmoncj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3miyebrte.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ygogxvkn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dirbnocp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3flwnrjja.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ltuscpxc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3bhllilje.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3dpwsrywn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3htbjbmdh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ynjjvpnx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3pnsxfsss.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ermsrjij.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rkbngtgo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3basoxtvi.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3dazhyiec.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3gxywevud.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3uviexjmw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3cmtrxznf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3tuuqqltj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3dywpsqkl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3teunpjlb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ukacprhl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eahyxmpj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xtjujels.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ibofnrvl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3pdorgytn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktwjixwy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ahwsawfi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3pmwckysg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3qokqwzjl.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mvmixucl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dotjpopj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bejhejbt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fajnikkg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fumdkcaw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lniksofm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tmaoinzt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3xkkggwsn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygkbolop.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3moftkbwf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kkzlgprt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lyfdclmy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3tlfzfnkk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3elbrcmtj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tiiweiod.html


<!-- 参考信息 -->