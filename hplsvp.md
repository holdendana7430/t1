代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.aibaodan.cn/gthdwiudqf.html

[A07] 数字转字符串
来源：http://hz.yanxiufei.cn/gtfypfvmke.html

Py:   str(42)
来源：http://hz.nanxuanxn.top/gtvnhtnuvf.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhaomingkeji.xyz/gtrrdrrpgi.html

JS:   String(42); (42).toString()
来源：http://hz.hysaishi.cn/gtovahgqwa.html

TS:   String(42)
来源：http://hz.shzxlz.cn/gtjbfikjyr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.feifeiyinyue.top/gtwsffmzqm.html

Go:   strconv.Itoa(42)
来源：http://hz.jqgufenzy.top/gtplfuspop.html

Ruby: 42.to_s
来源：http://hz.ppjwa.cn/gtpqvxeixu.html

C#:   42.ToString()
来源：http://hz.guowangkeji.top/gttlvthiyf.html

[A08] 取整与四舍五入
来源：http://hz.pycfn.com/gtgrjhkgzw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.nwbrower.top/gtvelljunp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.tanke756.top/gtxdobboki.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.ivvv.top/gtaqlhaopo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.daxiang520.top/gtxymikujv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.sweek.top/gtefetholw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.jlsjyb.cn/gtfujodlvs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.sufxvd.cn/gtlqavjzel.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.shuidangran.top/gtjodnfkcn.html

[A09] 绝对值与最大最小值
来源：http://hz.aibaodan.cn/gttihmjvlp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.cashguo.top/gtvgxzzthp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yuxming.cn/gthserdfwk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.vqdsnc.cn/gtzbzjaafz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.yvedp.cn/gtgeoqxxwt.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.guowangkeji.top/gtczizyowp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.gotoacloud.top/gtttboncff.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.xinyue.icu/gtdoboqkcp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.zdqjudy.top/gtdpjnmplf.html

[A10] 生成随机数
来源：http://hz.cheryme.top/gtnkemovpw.html

Py:   import random; random.randint(1, 100)
来源：http://hz.zhijiandao.cn/gtouwhpxbk.html

PHP:  random_int(1, 100);
来源：http://hz.wangshuangyany.cn/gttziaeydf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jqgfzy.top/gtfgtmjtyo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.feifeiyinyue.top/gtcmtetrul.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yuxming.cn/gtcsaiyzvx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.ivvv.top/gttosovdwf.html

Ruby: rand(1..100)
来源：http://hz.havefunace.top/gtkzdifbsu.html

C#:   new Random().Next(1, 101)
来源：http://hz.dashuyun.cn/gtvqxdixts.html

[A11] 条件表达式（三元）
来源：http://hz.xziqi.cn/gtutnjxtlh.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.daxiang520.top/gtrjxdvath.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.ydjk.org.cn/gtnxeebffy.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.cqqwz.cn/gtuouhcenj.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.jqgufenzy.top/gtlgaozqya.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.guannengcc.top/gtbmelaoee.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.c1oappe.top/gtcsffznbd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.hywenlv.cn/gtjmhylhbe.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.ydjk.org.cn/gtwuyfiqfd.html

[A12] 字符串插值 / 格式化
来源：http://hz.yuanzhike.top/gtpquuujvu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.tianlin.xyz/gtpsznhqju.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.0kj1m.cn/gtumfpmllo.html

JS:   `Hello, ${name}!`
来源：http://hz.nwbrower.top/gtiidijefp.html

TS:   `Hello, ${name}!`
来源：http://hz.tianlin.xyz/gtxmmipnux.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.jqgufenzy.top/gtxwsslhna.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.shangyingyoupin.top/gtlchjnzyv.html

Ruby: "Hello, #{name}!"
来源：http://hz.316326.xyz/gtiwzwjaes.html

C#:   $"Hello, {name}!"
来源：http://hz.ydjk.org.cn/gtnryfywby.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.pengpengdd.cyou/gtfeljwjgo.html

Py:   "第一行\n第二行"
来源：http://hz.shzxlz.cn/gtwxczodgx.html

PHP:  "第一行\n第二行"
来源：http://hz.aizwys.cn/gtuqmhumep.html

JS:   "第一行\n第二行"
来源：http://hz.haohaochexian.top/gtsrxykiox.html

TS:   "第一行\n第二行"
来源：http://hz.jianghu66.top/gtfukmsamo.html

Java: "第一行\n第二行"
来源：http://hz.yongpay.top/gtklgafynv.html

Go:   "第一行\n第二行"
来源：http://hz.xylfe.cn/gtdjzelpfu.html

Ruby: "第一行\n第二行"
来源：http://hz.tanke756.top/gtvslvvmgq.html

C#:   "第一行\n第二行"
来源：http://hz.yuxming.cn/gtfsbifndl.html

[A14] 注释写法
来源：http://hz.haohaochexian.top/gtcexukjyz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.tanke756.top/gtrrnstefp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.wangshuangyany.cn/gtvtrizvwm.html

JS:   // 单行；/* 多行 */
来源：http://hz.hnqzz.top/gtahokjfsr.html

TS:   // 单行；/* 多行 */
来源：http://hz.jianghu66.top/gtweruusoy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.yvedp.cn/gtblakbsis.html

Go:   // 单行；/* 多行 */
来源：http://hz.ydzc1.top/gtnpylykdg.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.nwbrower.top/gtgvmzzuhw.html

C#:   // 单行；/* 多行 */
来源：http://hz.chenzaomai.com/gtgfjadxlk.html

[A15] 空值判断与默认值
来源：http://hz.wangshuangyany.cn/gteipdpkut.html

Py:   value = data or "默认值"
来源：http://hz.yvedp.cn/gtgltutkvi.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.sweek.top/gtsmoilzyu.html

JS:   const value = data ?? "默认值";
来源：http://hz.nwbrower.top/gtczbfhhsl.html

TS:   const value = data ?? "默认值";
来源：http://hz.zhijiandao.cn/gtwirzblks.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.meibo888.top/gtiyuppedp.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.cdnleiting.top/gtplzamfwt.html

Ruby: value = data || "默认值"
来源：http://hz.wangdashe.top/gtfqwyxbil.html

C#:   var value = data ?? "默认值";
来源：http://hz.shangyingyoupin.top/gtzmrnouwc.html

[A16] 真假值判断规则
来源：http://hz.dianchejie.cn/gtxzfhsvek.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.fzhhl.top/gtjomzvpiq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.nanxuanxn.top/gtpbhujwjb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.mhx1999.top/gtthvtipkt.html

TS:   if (!x) {}
来源：http://hz.daria6918.cn/gtcwbhjzlc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.jyoumei.cn/gtlyplcufr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.cucudq.cn/gtgdpdsfnj.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.fengsongda.top/gtniiaqdwf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.svipenyu.cn/gtgkqqfrvn.html

[A17] 位运算
来源：http://hz.9152youxi.cn/gthziftgsj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinyuanbaomall.cn/gtmyqqrgqh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.gogol.net.cn/gteiudhrld.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydjk.org.cn/gtaokrdshc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.pycfn.com/gtrqpwazuy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yuxming.cn/gtlhxvcaxa.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.sweek.top/gtqoecengv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.feifeiyinyue.top/gtfbevkiho.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shuidangran.top/gthorkfabp.html

[A18] 字符与 ASCII 码互转
来源：http://hz.zhongyouzk.top/gthkvenzzj.html

Py:   ord("A"); chr(65)
来源：http://hz.wangshuangyany.cn/gtpdzkffvd.html

PHP:  ord("A"); chr(65)
来源：http://hz.aibaodan.cn/gtlslravki.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.pengpengdd.cyou/gthffixujp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jqgfzy.top/gtetyywmof.html

Java: (int) 'A'; (char) 65
来源：http://hz.hongshengwenyu.top/gtbwlskkjp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.chenlongwang.top/gtpfojiyio.html

Ruby: "A".ord; 65.chr
来源：http://hz.xinyue.icu/gtwjpdztbp.html

C#:   (int)'A'; (char)65
来源：http://hz.nwbrower.top/gtihbetcjv.html

[A19] 交换两个变量
来源：http://hz.feifeiyinyue.top/gtmycyukmk.html

Py:   a, b = b, a
来源：http://hz.sufxvd.cn/gtqkiqbjcj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.aibaodan.cn/gtfjepmpvd.html

JS:   [a, b] = [b, a];
来源：http://hz.wangdashe.top/gtvlhiooej.html

TS:   [a, b] = [b, a];
来源：http://hz.52xcode.cn/gticolkhsd.html

Java: int t = a; a = b; b = t;
来源：http://hz.jqgufenzy.top/gtwcjpugzc.html

Go:   a, b = b, a
来源：http://hz.pycfn.com/gtejtftnlu.html

Ruby: a, b = b, a
来源：http://hz.tianlin.xyz/gtnycumryf.html

C#:   (a, b) = (b, a);
来源：http://hz.c1oappe.top/gtlvzyvsuv.html

[A20] 读取标准输入
来源：http://hz.xingfuxueyuan.xyz/gtljmutrsq.html

Py:   name = input("请输入：")
来源：http://hz.xuanzx.com/gttynrkwhr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.zhixingplan.top/gtvyhdeoch.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.yongpay.top/gtdybbatze.html

TS:   // Node.js：readline 模块
来源：http://hz.birdmap.top/gtslqhrpri.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.hysaishi.cn/gtrufyoajo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.xingfuxueyuan.xyz/gttkvknqbt.html

Ruby: gets.chomp
来源：http://hz.andypj.xyz/gtjwdpivnf.html

C#:   Console.ReadLine();
来源：http://hz.hywenlv.cn/gtxjquordn.html

[A21] 保留指定小数位输出
来源：http://hz.yj202588.top/gtqiwxbgre.html

Py:   f"{3.14159:.2f}"
来源：http://hz.jinyuanbaomall.cn/gtarpdngwm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.nanxuanxn.top/gtpzhfbckp.html

JS:   (3.14159).toFixed(2)
来源：http://hz.52xcode.cn/gtrdxqcmji.html

TS:   (3.14159).toFixed(2)
来源：http://hz.dianchejie.cn/gtnquppvci.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.chenzaomai.com/gtapiqrecs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.ydzc1.top/gtnwsaiude.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.jianghu66.top/gtyipjxfqx.html

C#:   3.14159.ToString("F2")
来源：http://hz.shuidangran.top/gtrmrvpogg.html

[A22] 获取字符串长度
来源：http://hz.zhiwuduotai.top/gtxljngwgd.html

Py:   len(s)
来源：http://hz.yueranfly.top/gttaxwrndx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.ybcxt.top/gtpbanrnoh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.zhixingplan.top/gtnhnorsdi.html

TS:   s.length
来源：http://hz.sufxvd.cn/gtzzojoubb.html

Java: s.length()
来源：http://hz.daxiang520.top/gtpmpsbpzq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.yvedp.cn/gtxpezvkzw.html

Ruby: s.length
来源：http://hz.jinyuanbaomall.cn/gtlimykkgr.html

C#:   s.Length
来源：http://hz.feifeiyinyue.top/gtnfngrtqy.html

[A23] 大小写转换
来源：http://hz.yvedp.cn/gtezevtgch.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.aizwys.cn/gtachjlxnr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.xuetiantiany.cn/gtiyoxxyhq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zycfv.cn/gtcizzuafi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yj20258888.top/gtpsofgjtm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.xziqi.cn/gtagfkmogk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jinyuanbaomall.cn/gtazwmdpfg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.ppjwa.cn/gttooufrre.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.fzhhl.top/gtmqydaosx.html

[A24] 去除首尾空白
来源：http://hz.ybcxt.top/gtvwavuyyg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.jyoumei.cn/gtpektpipv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.ehwqpu.com/gtyyfpjqla.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.daria6918.cn/gtnewdjpnb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gogol.net.cn/gtavfdpydp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.fzhhl.top/gtmticyedg.html

Go:   strings.TrimSpace(s)
来源：http://hz.sweek.top/gtdcwxwsln.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.52xcode.cn/gtrqvcfqfb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.haohaochexian.top/gtsykvzomd.html

[A25] 字符串比较
来源：http://hz.fengsongda.top/gtfpjvaknt.html

Py:   s1 == s2; s1 != s2
来源：http://hz.aizwys.cn/gtkjobmeir.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yangfankeji.com/gtynobwkmo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.vqdsnc.cn/gtlewcedoy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shanyushiyangkeji.top/gtbwrovjpd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.pycfn.com/gtclxigsrf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.snrcjt.cn/gtkqxehxxl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.zhengqikj.top/gtzkdymjzr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.snrcjt.cn/gtfmkeqcot.html

[A26] 类型转换总览
来源：http://hz.shanyushiyangkeji.top/gtmscmcxcu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.ydzc1.top/gtxodfgevg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.zhoulong.xyz/gtvmowxrzj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yj20258888.top/gttukaizqz.html

TS:   Number() String() Boolean() x as number
来源：http://hz.feifeiyinyue.top/gtuhmpbsjd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.shanyushiyangtech.top/gttamcsaqh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.fengsongda.top/gthytqcsgc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.dashuyun.cn/gtkzdjgnkd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jlsjyb.cn/gtueuaapxb.html

================================================================================
来源：http://hz.cashguo.top/gtqcmrhzhg.html

B. 流程控制
来源：http://hz.guowangkeji.top/gtlrhlqnnx.html

================================================================================
来源：http://hz.svipenyu.cn/gtqyysqoit.html

[B01] 条件判断 if / else
来源：http://hz.yuxming.cn/gtgpjzwdfz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.c1oappe.top/gtlreftuwx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.xylfe.cn/gtpfopdbvt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.gotoacloud.top/gtsamneigq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhoulong.xyz/gtqcmmsujo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.gaohongyu789.top/gtywpebelg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.wangshuangyany.cn/gtijjoceqy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.shuidangran.top/gtrnrhqfbj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.smart0.xyz/gtvdyspsky.html

[B02] 多分支 else if / elif
来源：http://hz.c1oappe.top/gtvkxixcol.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhongyouzk.top/gthblypjvw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jinyuanbaomall.cn/gtgorsslrg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.guannengcc.top/gtuwbfntrj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zycfv.cn/gtrequnvqq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hammf.cn/gtnvvogxwe.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.guowangkeji.top/gtlfquions.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.pengpengdd.cyou/gttjfvufrb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tanke756.top/gtcbttqxwx.html

[B03] switch / match / case
来源：http://hz.zhengqikj.top/gtnrqrwfva.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.quarkkingdee.top/gtaiawysei.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.snrcjt.cn/gtyyedhklg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.c1oappe.top/gtordbyuze.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ybcxt.top/gtzpzxdmha.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.cdnleiting.top/gtcsffmfxi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.hammf.cn/gtdvscxxdf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.316326.xyz/gtbrufhcry.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.andypj.xyz/gtfiigbvcs.html

[B04] for 计数循环
来源：http://hz.yj202588.top/gtjkmcnjjq.html

Py:   for i in range(10): print(i)
来源：http://hz.dianchejie.cn/gtxbhwlcll.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.gzhubu.top/gtqeojfmfj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ydzc1.top/gtuuciyqoa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zdqjudy.top/gtivyztoco.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.cqqwz.cn/gtrxjpgfdg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.cucudq.cn/gtfwkfuwsl.html

Ruby: 10.times { |i| puts i }
来源：http://hz.vqdsnc.cn/gtnpqkwaxe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.c1oappe.top/gtulaamkgo.html

[B05] 遍历数组 / 列表
来源：http://hz.dianchejie.cn/gteqolqfug.html

Py:   for item in arr: print(item)
来源：http://hz.zycfv.cn/gtllwahokl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.sxryk.cn/gtrxwebwuv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.ehwqpu.com/gtqnsgnbus.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yonumen.top/gtunxfsdpm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.shzxlz.cn/gteuynvebk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zhaomingkeji.xyz/gtzciibzlr.html

Ruby: arr.each { |item| puts item }
来源：http://hz.tianlin.xyz/gtbriohoug.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yj202588.top/gtwfqyxdte.html

[B06] 遍历字典 / 对象
来源：http://hz.snrcjt.cn/gtrodefuka.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.havefunace.top/gtijuherwz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jinqigfzy.top/gttfqlpcgn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.316326.xyz/gtcydorcdr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhijiandao.cn/gtdmofopqo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.jinghuilouyu.cn/gtvhauirtn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.shangyingyoupin.top/gtegmnnjna.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.c1oappe.top/gtnovmljwb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jinghuilouyu.cn/gtirchllnh.html

[B07] while 循环
来源：http://hz.xingfuxueyuan.xyz/gtkewcittu.html

Py:   while i < 10: i += 1
来源：http://hz.shanyushiyangtech.top/gtfdptwdkd.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.fengsongda.top/gtemshzziw.html

JS:   while (i < 10) { i++; }
来源：http://hz.hfpthk.cn/gtmawjtful.html

TS:   while (i < 10) { i++; }
来源：http://hz.hfpthk.cn/gtjeddvjbu.html

Java: while (i < 10) { i++; }
来源：http://hz.gzhubu.top/gtldryayys.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.gzhubu.top/gtprqfgjss.html

Ruby: while i < 10; i += 1; end
来源：http://hz.wangshuangyany.cn/gtxywloiku.html

C#:   while (i < 10) { i++; }
来源：http://hz.nwbrower.top/gtzkhvorpg.html

[B08] do-while（至少执行一次）
来源：http://hz.daria6918.cn/gtjjyecahi.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ehwqpu.com/gttrgqyfsj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.iojbl.cn/gtagawtldg.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yangfankeji.com/gtgqgcghpf.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yj202588.top/gtcpxuhahp.html

Java: do { i++; } while (i < 10);
来源：http://hz.yanxiufei.cn/gtkeazcaoo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yvedp.cn/gtmwepcmtl.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.haohaochexian.top/gtthlybolq.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtrymoxikf.html

[B09] break 与 continue
来源：http://hz.yvedp.cn/gtxmjtnjuu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yj202588.top/gtrxrawkrm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtbsogmrvg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.daxiang520.top/gtncjmhcpu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.haohaochexian.top/gtpdwitcyn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtvbdupltu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jinqigfzy.top/gtlnsycjhs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.fengsongda.top/gtwoccvghb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigufen.top/gtdfjppmwo.html

[B10] 遍历同时拿索引
来源：http://hz.pycfn.com/gtmwouwvut.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.pengpengdd.cyou/gtmcotpyiw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jinghuilouyu.cn/gtvbygrlrj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.chenzaomai.com/gtcftvjnsp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.cucudq.cn/gtgfylfkue.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.mhx1999.top/gtwwsmkazs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.fengsongda.top/gtzxckwurn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ehwqpu.com/gtchftlcox.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.quarkkingdee.top/gtzrpzeivh.html

[B11] 生成数字序列 / 区间
来源：http://hz.wangshuangyany.cn/gtltewfhzc.html

Py:   list(range(0, 10, 2))
来源：http://hz.xuetiantiany.cn/gtryeskchl.html

PHP:  range(0, 10, 2);
来源：http://hz.haohaochexian.top/gtuxpskwvo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jiagoushi.top/gtornasszf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shangyingyoupin.top/gtcenjcnkt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinqigufen.top/gtgxtjrxqi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xuetiantiany.cn/gtbafejajz.html

Ruby: (0...10).step(2).to_a
来源：http://hz.daxiang520.top/gtpebmksvv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.wangshuangyany.cn/gthtbvkhcy.html

[B12] 跳出多层循环
来源：http://hz.daxiang520.top/gtsgtiexso.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.nwbrower.top/gtiqwnapam.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhiwuduotai.top/gtkensootu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zdqjudy.top/gtrwcytklg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sufxvd.cn/gthpknqkch.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.birdmap.top/gtaxxynwqz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guowangkeji.top/gtuahgudeb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zdqjudy.top/gtergkcbrb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jinqigufen.top/gtjidsghcr.html

[B13] 判断是否为数字
来源：http://hz.sweek.top/gttyvisqvc.html

Py:   isinstance(x, (int, float))
来源：http://hz.birdmap.top/gteujpbilk.html

PHP:  is_numeric($x)
来源：http://hz.c1oappe.top/gtnwyzadon.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinghuilouyu.cn/gtatlrrthr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.svipenyu.cn/gtvrdqkeew.html

Java: x instanceof Number
来源：http://hz.dianchejie.cn/gtcrpyaugl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jiagoushi.top/gtdlbxxfrg.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yj20258888.top/gttazptuuw.html


<!-- 参考信息 -->