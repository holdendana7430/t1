代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.0kj1m.cn/gtqmremddt.html

[A07] 数字转字符串
来源：http://hz.yj202588.top/gtgilyxpkx.html

Py:   str(42)
来源：http://hz.guowangkeji.top/gtrpiuyhdq.html

PHP:  (string) 42; strval(42)
来源：http://hz.chenjidiqi.icu/gtbvslcshk.html

JS:   String(42); (42).toString()
来源：http://hz.jinqigufen.top/gtyxbevvui.html

TS:   String(42)
来源：http://hz.hongshengwenyu.top/gtvwzpgruo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.vqdsnc.cn/gtvsabhjwb.html

Go:   strconv.Itoa(42)
来源：http://hz.ehwqpu.com/gtnnbtvrfy.html

Ruby: 42.to_s
来源：http://hz.redwolf501.top/gtmrbzswnw.html

C#:   42.ToString()
来源：http://hz.zhiwuduotai.top/gtjogcndsg.html

[A08] 取整与四舍五入
来源：http://hz.hysaishi.cn/gtmtncrouj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.ybcxt.top/gtzdytozga.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.shzxlz.cn/gtlfjrtnry.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.guannengcc.top/gtbdcjkqqh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.cqqwz.cn/gtujaqjrgz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.zdqjudy.top/gtzfyfhbhc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.dianchejie.cn/gthkyhapzt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jlsjyb.cn/gtjsimhtxj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.jinqigfzy.top/gtbhhcdqaw.html

[A09] 绝对值与最大最小值
来源：http://hz.ehwqpu.com/gtrniimqvf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jqgfzy.top/gtjjimunvp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xziqi.cn/gturpluggm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.52xcode.cn/gthwvidwgn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.sweek.top/gtiehhdiee.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.ehwqpu.com/gtongbrqjn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.hywenlv.cn/gtbiutxdzd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.hywenlv.cn/gtuyuwxroz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yj20258888.top/gtwkklwemi.html

[A10] 生成随机数
来源：http://hz.jinqigfzy.top/gttozxgmuj.html

Py:   import random; random.randint(1, 100)
来源：http://hz.gzhubu.top/gtblxpgoir.html

PHP:  random_int(1, 100);
来源：http://hz.tian-w.cn/gtwabdrfub.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.yuanzhike.top/gtziionzln.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.fzhhl.top/gtkvygmwaf.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yangfankeji.com/gtuzumbzmq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.jinghuilouyu.cn/gtkdqvdggw.html

Ruby: rand(1..100)
来源：http://hz.meibo888.top/gtknnwvofz.html

C#:   new Random().Next(1, 101)
来源：http://hz.jqgufenzy.top/gtibsodbdd.html

[A11] 条件表达式（三元）
来源：http://hz.svipenyu.cn/gtjhocxvxu.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.redwolf501.top/gtsuulmaiw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.zhiwuduotai.top/gtexmgemee.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.ppjwa.cn/gtgzynsxuu.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.ybcxt.top/gtltuyblfl.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.yvedp.cn/gtdpkypszm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.dashuyun.cn/gtclqbkmik.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.nwbrower.top/gtykchriee.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.shangyingyoupin.top/gtdzvyphzu.html

[A12] 字符串插值 / 格式化
来源：http://hz.52xcode.cn/gtyogejrah.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.kuanghao11.cn/gtvgtypdrn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.shanyushiyangkeji.top/gtoyinvhfp.html

JS:   `Hello, ${name}!`
来源：http://hz.tian-w.cn/gtnhjdazdd.html

TS:   `Hello, ${name}!`
来源：http://hz.chenjidiqi.icu/gtbfpawhio.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.feifeiyinyue.top/gtdkdmwmku.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.zycfv.cn/gtcrfeaacd.html

Ruby: "Hello, #{name}!"
来源：http://hz.chenzaomai.com/gtccvmrskd.html

C#:   $"Hello, {name}!"
来源：http://hz.ydzc1.top/gtnbwydyfx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.aizwys.cn/gtvxudzsum.html

Py:   "第一行\n第二行"
来源：http://hz.shangyingyoupin.top/gtqyikpgxa.html

PHP:  "第一行\n第二行"
来源：http://hz.sxryk.cn/gtzhgjxsbv.html

JS:   "第一行\n第二行"
来源：http://hz.zycfv.cn/gtdsxhikjd.html

TS:   "第一行\n第二行"
来源：http://hz.yj202588.top/gtaxyfpoyt.html

Java: "第一行\n第二行"
来源：http://hz.zhongyouzk.top/gtejamjejq.html

Go:   "第一行\n第二行"
来源：http://hz.fengsongda.top/gtvhuzsfhb.html

Ruby: "第一行\n第二行"
来源：http://hz.shangyingyoupin.top/gtclbswctx.html

C#:   "第一行\n第二行"
来源：http://hz.cucudq.cn/gtdhxlwfya.html

[A14] 注释写法
来源：http://hz.dianchejie.cn/gtfkitborg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.shuidangran.top/gtjyarzpjg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.cheryme.top/gtngcgbanq.html

JS:   // 单行；/* 多行 */
来源：http://hz.nanxuanxn.top/gtyfwvrrxq.html

TS:   // 单行；/* 多行 */
来源：http://hz.hammf.cn/gtmjysmoyv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.ydjk.org.cn/gtkckyaefk.html

Go:   // 单行；/* 多行 */
来源：http://hz.hnqzz.top/gtdcjdywln.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.zhongyouzk.top/gtrlltmmzz.html

C#:   // 单行；/* 多行 */
来源：http://hz.hnxiangtu.top/gtukaqgaah.html

[A15] 空值判断与默认值
来源：http://hz.cucudq.cn/gtyynanvyx.html

Py:   value = data or "默认值"
来源：http://hz.redwolf501.top/gtyobtlgcz.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.zycfv.cn/gtfbtxojam.html

JS:   const value = data ?? "默认值";
来源：http://hz.shuidangran.top/gtznnimllf.html

TS:   const value = data ?? "默认值";
来源：http://hz.tanke756.top/gtjnawugum.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.yueranfly.top/gtrsujxluu.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.snrcjt.cn/gtohfnyiri.html

Ruby: value = data || "默认值"
来源：http://hz.yuanzhike.top/gtiduxfmkz.html

C#:   var value = data ?? "默认值";
来源：http://hz.jinqigfzy.top/gtnlbwijua.html

[A16] 真假值判断规则
来源：http://hz.wangdashe.top/gteitrffhn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.svipenyu.cn/gtwqxdnjzi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.cdnleiting.top/gtjnimimom.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.yanxiufei.cn/gthvrhsysu.html

TS:   if (!x) {}
来源：http://hz.shzxlz.cn/gtdtcabvie.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.jlsjyb.cn/gtgebxudne.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.svipenyu.cn/gtejldsmxo.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.c1oappe.top/gtfpujaykn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.ywan-chungtsiang.top/gtqnacvojt.html

[A17] 位运算
来源：http://hz.zhoulong.xyz/gtfvlsndga.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cqqwz.cn/gtstghrtpb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.jqgufenzy.top/gthuqtsgxs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydjk.org.cn/gtentwaacf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.jyoumei.cn/gtigggvcjb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yj20258.top/gtzlibnjcd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jlsjyb.cn/gtuucpvddn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gogol.net.cn/gtwtsvbvgj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tian-w.cn/gtmdyxykbl.html

[A18] 字符与 ASCII 码互转
来源：http://hz.meibo888.top/gtcvbzteij.html

Py:   ord("A"); chr(65)
来源：http://hz.shanyushiyangkeji.top/gtvihqhfvr.html

PHP:  ord("A"); chr(65)
来源：http://hz.hywenlv.cn/gtjbigcoae.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.dianchejie.cn/gtvluumtnl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.gogol.net.cn/gtipzcxohj.html

Java: (int) 'A'; (char) 65
来源：http://hz.9152youxi.cn/gtlatkekmd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.ydzc1.top/gtiiiflvfx.html

Ruby: "A".ord; 65.chr
来源：http://hz.hammf.cn/gtdafisfga.html

C#:   (int)'A'; (char)65
来源：http://hz.jinghuilouyu.cn/gtfqislfat.html

[A19] 交换两个变量
来源：http://hz.jinghuilouyu.cn/gtogknbeqr.html

Py:   a, b = b, a
来源：http://hz.xingfuxueyuan.xyz/gtgelwiewb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.zhiwuduotai.top/gtkovnbsqp.html

JS:   [a, b] = [b, a];
来源：http://hz.dianchejie.cn/gtzoniqnpz.html

TS:   [a, b] = [b, a];
来源：http://hz.jinghuilouyu.cn/gtfvdzrptl.html

Java: int t = a; a = b; b = t;
来源：http://hz.xingfuxueyuan.xyz/gtqdmvsdpe.html

Go:   a, b = b, a
来源：http://hz.jinqigfzy.top/gtgmrrcfpq.html

Ruby: a, b = b, a
来源：http://hz.hongshengwenyu.top/gtcbpeljvw.html

C#:   (a, b) = (b, a);
来源：http://hz.gotoacloud.top/gtoynawnoo.html

[A20] 读取标准输入
来源：http://hz.shanyushiyangkeji.top/gtuvcsigdv.html

Py:   name = input("请输入：")
来源：http://hz.cheryme.top/gtrtlozfmh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.vqdsnc.cn/gtckytrzwc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.shanyushiyangkeji.top/gtytbugtly.html

TS:   // Node.js：readline 模块
来源：http://hz.fengsongda.top/gtxyoqxqby.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yuanzhike.top/gtdascmpmn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.wangshuangyany.cn/gtoupleieg.html

Ruby: gets.chomp
来源：http://hz.tianlin.xyz/gtrqifsnlm.html

C#:   Console.ReadLine();
来源：http://hz.zhaomingkeji.xyz/gtoibxcqwy.html

[A21] 保留指定小数位输出
来源：http://hz.sweek.top/gtddfgoekq.html

Py:   f"{3.14159:.2f}"
来源：http://hz.wangdashe.top/gtnwtyoukg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.shzxlz.cn/gtkdtrtbyf.html

JS:   (3.14159).toFixed(2)
来源：http://hz.gotoacloud.top/gtpwbluuob.html

TS:   (3.14159).toFixed(2)
来源：http://hz.cqqwz.cn/gtgdjdnwpg.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.tanke756.top/gtduqjxnzv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.birdmap.top/gtgbwsnxvq.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.cashguo.top/gtwrpqzjpc.html

C#:   3.14159.ToString("F2")
来源：http://hz.yvedp.cn/gtxhmdkhxp.html

[A22] 获取字符串长度
来源：http://hz.nanxinkj.top/gtlnlkrxlj.html

Py:   len(s)
来源：http://hz.snrcjt.cn/gtcmqmnbbp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.pycfn.com/gtbydvcaxi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.smart0.xyz/gtgzkptilz.html

TS:   s.length
来源：http://hz.jinqigufen.top/gtajtcpfha.html

Java: s.length()
来源：http://hz.aibaodan.cn/gtdaqdcjbh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.daxiang520.top/gtqghztmtk.html

Ruby: s.length
来源：http://hz.wangdashe.top/gtlkufvsjt.html

C#:   s.Length
来源：http://hz.daria6918.cn/gtqbybgmve.html

[A23] 大小写转换
来源：http://hz.feifeiyinyue.top/gtjavxtggo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.yongpay.top/gtvzzgygda.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.zhaomingkeji.xyz/gtscrcnsif.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yj202588.top/gtwegtfpqo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.sweek.top/gtwypijdft.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.gzhubu.top/gtkcvrfufx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jinqigufen.top/gtksksgqkw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.guannengcc.top/gtrlrjngvv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.dianchejie.cn/gtdvmyfumr.html

[A24] 去除首尾空白
来源：http://hz.jinqigufen.top/gtklaqcptd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.nwbrower.top/gtrlykldlk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.meibo888.top/gttcynirtm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhoulong.xyz/gtzexqizpd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.c1oappe.top/gtypamgkdw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.hfpthk.cn/gtflyrcvyw.html

Go:   strings.TrimSpace(s)
来源：http://hz.nwbrower.top/gtxdtcdlbu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.gotoacloud.top/gtwgmglivq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.aibaodan.cn/gtvmoelzqr.html

[A25] 字符串比较
来源：http://hz.tian-w.cn/gtsggxdalm.html

Py:   s1 == s2; s1 != s2
来源：http://hz.chenlongwang.top/gticqzcrss.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.52xcode.cn/gtnyznlfwd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.cashguo.top/gtwezxulaz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zycfv.cn/gtutvmwyqb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.shzxlz.cn/gtwmlkxupn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.aibaodan.cn/gtavtwwmlm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.sweek.top/gtsatkyyqg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.jiagoushi.top/gtwyompsjo.html

[A26] 类型转换总览
来源：http://hz.tian-w.cn/gtwmvhocuu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.birdmap.top/gtxsxcjppp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.hfpthk.cn/gtflypebyp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.316326.xyz/gtffgripsl.html

TS:   Number() String() Boolean() x as number
来源：http://hz.sysykeji.top/gtjortwdzw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.fzhhl.top/gtbxydgrzm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yongpay.top/gtbvlzafvo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.svipenyu.cn/gtueiwfycs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.quarkkingdee.top/gttfyfmruu.html

================================================================================
来源：http://hz.hnqzz.top/gtudglgvuu.html

B. 流程控制
来源：http://hz.tianlin.xyz/gtapseymlh.html

================================================================================
来源：http://hz.tanke756.top/gtykuejjag.html

[B01] 条件判断 if / else
来源：http://hz.cashguo.top/gtwjqfllzk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.shangyingyoupin.top/gtmeqazjzl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yj20258.top/gtcebuarla.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.aizwys.cn/gtqgtsetnz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jqgfzy.top/gtpjgslfse.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.quarkkingdee.top/gtndizpljq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.gotoacloud.top/gtgrcyyknw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.hongshengwenyu.top/gtwoggsjka.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.dianchejie.cn/gtqcazqnlk.html

[B02] 多分支 else if / elif
来源：http://hz.shangyingyoupin.top/gtrtdeyzfm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.cashguo.top/gtdiwcqrtp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.nanxuanxn.top/gtfmsuoskq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhongyouzk.top/gtcxneilqd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yuanzhike.top/gtqecvoela.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hnxiangtu.top/gtseinjnkr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yueranfly.top/gtykwfskop.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhaomingkeji.xyz/gtdodrelwr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258888.top/gtjwncdnxt.html

[B03] switch / match / case
来源：http://hz.hnqzz.top/gtjidbzwbq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.hfpthk.cn/gthmuybykl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.nanxinkj.top/gtefksscib.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.dashuyun.cn/gtnzhozkut.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cdnleiting.top/gttgmxjzup.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.shanyushiyangtech.top/gtyehxiynx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.chenlongwang.top/gtkzeagvky.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.yj202588.top/gtdpnbrema.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.bjfxy.top/gtpqhtgvho.html

[B04] for 计数循环
来源：http://hz.yj20258888.top/gtcfjpqxsc.html

Py:   for i in range(10): print(i)
来源：http://hz.cqqwz.cn/gtclgpqyca.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yueranfly.top/gtdlcbxnpx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.havefunace.top/gtscpujoms.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yanxiufei.cn/gthuredvap.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yj202588.top/gtsfxvofzc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.ywan-chungtsiang.top/gtnspbllmt.html

Ruby: 10.times { |i| puts i }
来源：http://hz.cucudq.cn/gtgbnyczdd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yueranfly.top/gtorwbihni.html

[B05] 遍历数组 / 列表
来源：http://hz.sufxvd.cn/gtjfqwgsqo.html

Py:   for item in arr: print(item)
来源：http://hz.jiagoushi.top/gtboljqodi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jqgufenzy.top/gtagujqkiq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yuanzhike.top/gtrvelavgr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.cheryme.top/gtnvwrwlaf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yongpay.top/gtoclvnlyj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ivvv.top/gtzraeziyl.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yueranfly.top/gtheoewfxp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.jinqigfzy.top/gtcxvqlbfo.html

[B06] 遍历字典 / 对象
来源：http://hz.hammf.cn/gtevapfcfz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jinyuanbaomall.cn/gtwsrnakvd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jlsjyb.cn/gthcrbnwaj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.aibaodan.cn/gtmbdnotlp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.kuanghao11.cn/gtuypxhuud.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gogol.net.cn/gtkhlqzsqv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jinghuilouyu.cn/gtxywtowco.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhiwuduotai.top/gtqficbgsn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.nwbrower.top/gtgentdhjf.html

[B07] while 循环
来源：http://hz.xingfuxueyuan.xyz/gtatvvqdgd.html

Py:   while i < 10: i += 1
来源：http://hz.sysykeji.top/gtyuyrqynn.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.fzhhl.top/gttgdcbxsh.html

JS:   while (i < 10) { i++; }
来源：http://hz.jinghuilouyu.cn/gtoknyluse.html

TS:   while (i < 10) { i++; }
来源：http://hz.cdnleiting.top/gtvmgowzsr.html

Java: while (i < 10) { i++; }
来源：http://hz.haohaochexian.top/gtdfmuczdw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.wangdashe.top/gtzqnxuqoz.html

Ruby: while i < 10; i += 1; end
来源：http://hz.feifeiyinyue.top/gtqdvlwiyc.html

C#:   while (i < 10) { i++; }
来源：http://hz.chenlongwang.top/gtoqrywtln.html

[B08] do-while（至少执行一次）
来源：http://hz.cheryme.top/gtxiafbisn.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.316326.xyz/gtnfqmltwg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.chenzaomai.com/gtxllbprny.html

JS:   do { i++; } while (i < 10);
来源：http://hz.dashuyun.cn/gtosrpzokl.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhijiandao.cn/gthnskgfax.html

Java: do { i++; } while (i < 10);
来源：http://hz.nwbrower.top/gthvfpgoin.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.shanyushiyangkeji.top/gtimxbbous.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hammf.cn/gtjyccluxj.html

C#:   do { i++; } while (i < 10);
来源：http://hz.dianchejie.cn/gtvhouhrnx.html

[B09] break 与 continue
来源：http://hz.zhixingplan.top/gtwdwvflcw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.redwolf501.top/gtmvuqlrdr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.sysykeji.top/gtxabumiyj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hammf.cn/gtchuayhjn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gzhubu.top/gtrsomssxb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ppjwa.cn/gtjularskb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yonumen.top/gtmhyjqhuv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.0kj1m.cn/gtqnahjtky.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.havefunace.top/gtsdhusmeh.html

[B10] 遍历同时拿索引
来源：http://hz.zhaomingkeji.xyz/gthnvrunjq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.sysykeji.top/gtyvuispwk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jqgufenzy.top/gtxvmscquy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yvedp.cn/gtmdpaumxq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.nanxuanxn.top/gtggaxlesa.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.52xcode.cn/gtekcdaxkh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yangfankeji.com/gtcqumznkm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ydzc1.top/gtdwlithml.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hnqzz.top/gttupybyou.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinyuanbaomall.cn/gtuliywpfw.html

Py:   list(range(0, 10, 2))
来源：http://hz.shangyingyoupin.top/gtwrrbqckm.html

PHP:  range(0, 10, 2);
来源：http://hz.0kj1m.cn/gtkgtiwvyv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hfpthk.cn/gtbpflrgfu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.dashuyun.cn/gtdgfkbmye.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.sxryk.cn/gtclcbfyvf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hysaishi.cn/gtyyzszkyo.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhengqikj.top/gtldsnmlme.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.guowangkeji.top/gtrmjgdfro.html

[B12] 跳出多层循环
来源：http://hz.yj20258.top/gtnbjskqto.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.pycfn.com/gtijoqvvgy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jianghu66.top/gtzvrjedfz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tanke756.top/gtgwqaiycz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sweek.top/gtkgxabphj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zycfv.cn/gtajzvrzno.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.0kj1m.cn/gtjicpdthc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xuanzx.com/gtxtdqtlrb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jyoumei.cn/gtmjmdimtv.html

[B13] 判断是否为数字
来源：http://hz.chenlongwang.top/gtzypdkefb.html

Py:   isinstance(x, (int, float))
来源：http://hz.xuetiantiany.cn/gtsgyqazzx.html

PHP:  is_numeric($x)
来源：http://hz.aibaodan.cn/gtdfcoaylt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.aibaodan.cn/gtqchrkidu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nwbrower.top/gtpdnwgbdl.html

Java: x instanceof Number
来源：http://hz.yonumen.top/gtabxfeovf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yvedp.cn/gtsmxmnexn.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hywenlv.cn/gtvdgvbigm.html


<!-- 参考信息 -->