代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.xziqi.cn/gtncjofymc.html

[A07] 数字转字符串
来源：http://hz.jianghu66.top/gtfrlmnsnh.html

Py:   str(42)
来源：http://hz.yvedp.cn/gtseqeuasl.html

PHP:  (string) 42; strval(42)
来源：http://hz.jinqigufen.top/gtneldtslc.html

JS:   String(42); (42).toString()
来源：http://hz.shuidangran.top/gtorglbacy.html

TS:   String(42)
来源：http://hz.hongshengwenyu.top/gtkhpqejin.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.ivvv.top/gtquemjczc.html

Go:   strconv.Itoa(42)
来源：http://hz.jianghu66.top/gtcgtnfiua.html

Ruby: 42.to_s
来源：http://hz.ywan-chungtsiang.top/gtpelmjoim.html

C#:   42.ToString()
来源：http://hz.zhaomingkeji.xyz/gtoxznexwg.html

[A08] 取整与四舍五入
来源：http://hz.hywenlv.cn/gtgrpnowhd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.bjfxy.top/gtpvmjrsyb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.hammf.cn/gtmddbwlzs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.aibaodan.cn/gtphnulmfo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.yangfankeji.com/gtttawmbkl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.kuanghao11.cn/gtykkwntuv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.redwolf501.top/gtqyogobiu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jinqigufen.top/gtdoqfhmdh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.sysykeji.top/gteesllgbk.html

[A09] 绝对值与最大最小值
来源：http://hz.dashuyun.cn/gtpnnpvnxh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.yangfankeji.com/gtgeywkxdj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.redwolf501.top/gtdnqpzhbb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.yanxiufei.cn/gtfcmbocau.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.shanyushiyangkeji.top/gtjxdwfifa.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.nwbrower.top/gtaemyfgcf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.daria6918.cn/gtinlfzehc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.ywan-chungtsiang.top/gttyvpbfnp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.chenzaomai.com/gtqwxiorfu.html

[A10] 生成随机数
来源：http://hz.kuanghao11.cn/gtwbdjdrkj.html

Py:   import random; random.randint(1, 100)
来源：http://hz.zhijiandao.cn/gtrvjlaqoy.html

PHP:  random_int(1, 100);
来源：http://hz.gaohongyu789.top/gtfxppmyan.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jyoumei.cn/gtxoqkelge.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ivvv.top/gtqzdtgaiy.html

Java: new Random().nextInt(100) + 1
来源：http://hz.daxiang520.top/gtgxjmlnpo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.jinghuilouyu.cn/gtrmphbwgw.html

Ruby: rand(1..100)
来源：http://hz.xinyue.icu/gtckwdzgku.html

C#:   new Random().Next(1, 101)
来源：http://hz.ydzc1.top/gtmedirpeg.html

[A11] 条件表达式（三元）
来源：http://hz.mhx1999.top/gtuxjawfbh.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.jinqigfzy.top/gtdaedzrsk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.316326.xyz/gtijizpecw.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.52xcode.cn/gtoptxmztx.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.xylfe.cn/gtvwsxxxbo.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.chenzaomai.com/gtqdpboknb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.yuanzhike.top/gtemvraoac.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.chenzaomai.com/gtnmmhaqwr.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.9152youxi.cn/gtqkoxxnxm.html

[A12] 字符串插值 / 格式化
来源：http://hz.shanyushiyangtech.top/gthteaynat.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.9152youxi.cn/gtvxxjkwdd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.sysykeji.top/gtqonvkcut.html

JS:   `Hello, ${name}!`
来源：http://hz.kuanghao11.cn/gtnvqmmlhh.html

TS:   `Hello, ${name}!`
来源：http://hz.svipenyu.cn/gtbtjdrcwl.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.snrcjt.cn/gtykhsopim.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.yj20258.top/gtvltushat.html

Ruby: "Hello, #{name}!"
来源：http://hz.ivvv.top/gtpwqyeeth.html

C#:   $"Hello, {name}!"
来源：http://hz.pengpengdd.cyou/gtojefubnd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.daria6918.cn/gtubiqvzoy.html

Py:   "第一行\n第二行"
来源：http://hz.dashuyun.cn/gtktuziomx.html

PHP:  "第一行\n第二行"
来源：http://hz.quarkkingdee.top/gtpfcipnqb.html

JS:   "第一行\n第二行"
来源：http://hz.cdnleiting.top/gttgulenjz.html

TS:   "第一行\n第二行"
来源：http://hz.dashuyun.cn/gtdhsrqeme.html

Java: "第一行\n第二行"
来源：http://hz.cashguo.top/gtpynmitzm.html

Go:   "第一行\n第二行"
来源：http://hz.nwbrower.top/gtoklclnam.html

Ruby: "第一行\n第二行"
来源：http://hz.cqqwz.cn/gtocrlygpb.html

C#:   "第一行\n第二行"
来源：http://hz.ydzc1.top/gtzkufbyhz.html

[A14] 注释写法
来源：http://hz.fengsongda.top/gtncwikeuk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.tanke756.top/gtrdgsmheo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.yj20258888.top/gtjdinovbl.html

JS:   // 单行；/* 多行 */
来源：http://hz.chenlongwang.top/gtgjdmhgec.html

TS:   // 单行；/* 多行 */
来源：http://hz.hnqzz.top/gtyldwwmhx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.svipenyu.cn/gtyapjhfbc.html

Go:   // 单行；/* 多行 */
来源：http://hz.pengpengdd.cyou/gtmmjvpavg.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.guannengcc.top/gtemshyxxt.html

C#:   // 单行；/* 多行 */
来源：http://hz.zhixingplan.top/gtqfieiald.html

[A15] 空值判断与默认值
来源：http://hz.jinyuanbaomall.cn/gteqdgchbl.html

Py:   value = data or "默认值"
来源：http://hz.jinqigufen.top/gtttkrculr.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.xuetiantiany.cn/gtvpcbrtfh.html

JS:   const value = data ?? "默认值";
来源：http://hz.sysykeji.top/gtlqrwdezx.html

TS:   const value = data ?? "默认值";
来源：http://hz.jqgfzy.top/gtsjfvizno.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.zhengqikj.top/gtgjhtjlns.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.wangdashe.top/gtnoftagoy.html

Ruby: value = data || "默认值"
来源：http://hz.jinqigfzy.top/gtoysgesvf.html

C#:   var value = data ?? "默认值";
来源：http://hz.birdmap.top/gtlcehufxe.html

[A16] 真假值判断规则
来源：http://hz.0kj1m.cn/gtmxtssihp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.ivvv.top/gtgnuiavbr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.xylfe.cn/gtaskfzvjn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.yueranfly.top/gtedtwuyio.html

TS:   if (!x) {}
来源：http://hz.dashuyun.cn/gtojuhamrc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.hnqzz.top/gtoipnionk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.yangfankeji.com/gtpuveuwpb.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.dianchejie.cn/gtzmpppmfq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.yangfankeji.com/gtnmlddjxz.html

[A17] 位运算
来源：http://hz.9152youxi.cn/gtvtovterl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.iojbl.cn/gthobicmbs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.bjfxy.top/gtjmjosgxp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.nanxuanxn.top/gtisxzyuqt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.sufxvd.cn/gtlxyvslaf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sufxvd.cn/gtxpoeboxy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jyoumei.cn/gtcqvtuctb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.birdmap.top/gtxqtvpbam.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jianghu66.top/gtdumregwl.html

[A18] 字符与 ASCII 码互转
来源：http://hz.ppjwa.cn/gtvcnmdyju.html

Py:   ord("A"); chr(65)
来源：http://hz.ydjk.org.cn/gtephnhgeo.html

PHP:  ord("A"); chr(65)
来源：http://hz.jinqigufen.top/gtawnixmki.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.sysykeji.top/gtocdmrpwy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.0kj1m.cn/gtncufdzvy.html

Java: (int) 'A'; (char) 65
来源：http://hz.xziqi.cn/gtbdbsndnn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.iojbl.cn/gtrxtfgkvx.html

Ruby: "A".ord; 65.chr
来源：http://hz.ppjwa.cn/gttyrauwls.html

C#:   (int)'A'; (char)65
来源：http://hz.svipenyu.cn/gthwwzcmab.html

[A19] 交换两个变量
来源：http://hz.gotoacloud.top/gtapflaqwt.html

Py:   a, b = b, a
来源：http://hz.gogol.net.cn/gtanvgxwne.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.bjfxy.top/gtvjjlhbmc.html

JS:   [a, b] = [b, a];
来源：http://hz.c1oappe.top/gtvcnskfiq.html

TS:   [a, b] = [b, a];
来源：http://hz.zhixingplan.top/gtoakmmxtv.html

Java: int t = a; a = b; b = t;
来源：http://hz.xuanzx.com/gtsjexvybu.html

Go:   a, b = b, a
来源：http://hz.kuanghao11.cn/gtikkpxvyz.html

Ruby: a, b = b, a
来源：http://hz.jinqigfzy.top/gtbjpbzzpi.html

C#:   (a, b) = (b, a);
来源：http://hz.jinghuilouyu.cn/gtsyebkcxy.html

[A20] 读取标准输入
来源：http://hz.0kj1m.cn/gtwzwiwfde.html

Py:   name = input("请输入：")
来源：http://hz.gzhubu.top/gtlkoxdhfb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.feifeiyinyue.top/gtrvritskg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.mhx1999.top/gtkhngmjnw.html

TS:   // Node.js：readline 模块
来源：http://hz.jiagoushi.top/gttoliysff.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.nwbrower.top/gtmmqpmfog.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.yueranfly.top/gtonqhtjcx.html

Ruby: gets.chomp
来源：http://hz.wangshuangyany.cn/gtekpeeuhk.html

C#:   Console.ReadLine();
来源：http://hz.smart0.xyz/gtlccxeeay.html

[A21] 保留指定小数位输出
来源：http://hz.sysykeji.top/gtmgnvdlqi.html

Py:   f"{3.14159:.2f}"
来源：http://hz.shanyushiyangtech.top/gtimjhxkbo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.xingfuxueyuan.xyz/gtyykvkrur.html

JS:   (3.14159).toFixed(2)
来源：http://hz.yongpay.top/gtpnwopxww.html

TS:   (3.14159).toFixed(2)
来源：http://hz.xylfe.cn/gthwytbowu.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.shuidangran.top/gthpejcbjb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.xinyue.icu/gtsfzmkzkc.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.0kj1m.cn/gthpfdmdey.html

C#:   3.14159.ToString("F2")
来源：http://hz.guowangkeji.top/gtgsrkiazv.html

[A22] 获取字符串长度
来源：http://hz.daria6918.cn/gtdovqllqi.html

Py:   len(s)
来源：http://hz.daxiang520.top/gtqqmywcso.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.feifeiyinyue.top/gtuorvevtl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.zycfv.cn/gttancoxwq.html

TS:   s.length
来源：http://hz.zdqjudy.top/gtksmfbddh.html

Java: s.length()
来源：http://hz.xingfuxueyuan.xyz/gtqqzttvdz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.ydjk.org.cn/gtnklqaovm.html

Ruby: s.length
来源：http://hz.ybcxt.top/gtjvcwbfax.html

C#:   s.Length
来源：http://hz.quarkkingdee.top/gtiirujpvy.html

[A23] 大小写转换
来源：http://hz.yj202588.top/gtjxfhkowg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.fengsongda.top/gtnybsmkak.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.guannengcc.top/gtiprxotsl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.sxryk.cn/gtsdpwowyh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.chenlongwang.top/gtlpnvrqhv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.chenlongwang.top/gtnmplnjww.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yuxming.cn/gtgbmfejfl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.xuanzx.com/gtiyqrqcav.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.fzhhl.top/gtmkyhxkqn.html

[A24] 去除首尾空白
来源：http://hz.jinyuanbaomall.cn/gtobseatbm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.guannengcc.top/gtltvbxoab.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.shzxlz.cn/gtijjzlkog.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jyoumei.cn/gtajsmjxqf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zycfv.cn/gtawmccqbw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.jiagoushi.top/gtovfqtliv.html

Go:   strings.TrimSpace(s)
来源：http://hz.c1oappe.top/gtxymwgzuu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.zhongyouzk.top/gtwgrrepbm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.hysaishi.cn/gttpzjtrie.html

[A25] 字符串比较
来源：http://hz.0kj1m.cn/gttyukpekn.html

Py:   s1 == s2; s1 != s2
来源：http://hz.hammf.cn/gttqmffodk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.sweek.top/gtsbovrjrq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shuidangran.top/gtkpxbhjjt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.meibo888.top/gtnoulfzxp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.tian-w.cn/gtqpalxktv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jinyuanbaomall.cn/gtfucrytux.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.quarkkingdee.top/gtffiveyyc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.316326.xyz/gttufvyztq.html

[A26] 类型转换总览
来源：http://hz.smart0.xyz/gtitocqdhb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.cdnleiting.top/gtbcbzargd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.cashguo.top/gtpfohtkow.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zhixingplan.top/gtpdpearzy.html

TS:   Number() String() Boolean() x as number
来源：http://hz.jyoumei.cn/gtjlzuijcp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yueranfly.top/gtrpiltdlo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.tianlin.xyz/gttoqicnce.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jinyuanbaomall.cn/gtpluortot.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.ivvv.top/gtdiasiqxy.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtgurlnkpd.html

B. 流程控制
来源：http://hz.vqdsnc.cn/gttitcafws.html

================================================================================
来源：http://hz.cdnleiting.top/gtpzqkwhqv.html

[B01] 条件判断 if / else
来源：http://hz.yuanzhike.top/gtamramppw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.quarkkingdee.top/gtwnrnuadi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yangfankeji.com/gtyxqmomwg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.cheryme.top/gtvlkxonvy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258888.top/gtgrgtftva.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.snrcjt.cn/gtljkmaced.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.316326.xyz/gtnpcevkdp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.hfpthk.cn/gtggwfwhom.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jianghu66.top/gtexnhzvag.html

[B02] 多分支 else if / elif
来源：http://hz.gogol.net.cn/gtxelbcsqq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.hfpthk.cn/gtnkickszd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.bjfxy.top/gtcjhmxlna.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenlongwang.top/gtcucjyftu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yanxiufei.cn/gtgfoxciwj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhixingplan.top/gtqcdzruar.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yuanzhike.top/gtdftifgds.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.redwolf501.top/gtvrdstghq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.9152youxi.cn/gtaharoxqm.html

[B03] switch / match / case
来源：http://hz.guowangkeji.top/gtmqtgdidl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yj20258.top/gtkdjnktkn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.hywenlv.cn/gtqmvwllzo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.nanxinkj.top/gthywmelpj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.quarkkingdee.top/gtaezewpjk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yj202588.top/gtwmfufudy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhengqikj.top/gtpqjlkwhg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.fzhhl.top/gtanaqbmci.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.jinyuanbaomall.cn/gtgsbzlkzl.html

[B04] for 计数循环
来源：http://hz.xinyue.icu/gtrupgolil.html

Py:   for i in range(10): print(i)
来源：http://hz.aizwys.cn/gtnhzdwaef.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.xziqi.cn/gtjxzbubwu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jyoumei.cn/gtcsqcbnag.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xinyue.icu/gtmbomyagf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.xuanzx.com/gtxnqhivrf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhoulong.xyz/gtnvtmthtu.html

Ruby: 10.times { |i| puts i }
来源：http://hz.jinghuilouyu.cn/gtehlfhjht.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.ivvv.top/gtgbnppepi.html

[B05] 遍历数组 / 列表
来源：http://hz.shangyingyoupin.top/gtgddmrmwg.html

Py:   for item in arr: print(item)
来源：http://hz.hfpthk.cn/gtonrqcbtf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.ivvv.top/gtwqjosbxc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.wangshuangyany.cn/gteetimedj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jyoumei.cn/gtdodoxvyd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.316326.xyz/gtmuzrctzv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zhijiandao.cn/gttfuytbfd.html

Ruby: arr.each { |item| puts item }
来源：http://hz.sufxvd.cn/gtiaxxdlho.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.0kj1m.cn/gtleggevld.html

[B06] 遍历字典 / 对象
来源：http://hz.yj20258.top/gthqyvhhdy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.xingfuxueyuan.xyz/gtacnauqda.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yj20258888.top/gtcyzbhlmh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xylfe.cn/gtzfkikurx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.bjfxy.top/gtbfmdaeeh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.tianlin.xyz/gtvyufcbur.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jinqigfzy.top/gthwphcfre.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xingfuxueyuan.xyz/gtnpktajyd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.wangshuangyany.cn/gtnayybhsm.html

[B07] while 循环
来源：http://hz.ybcxt.top/gtjlgckqyf.html

Py:   while i < 10: i += 1
来源：http://hz.nanxuanxn.top/gtgvuopsql.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.shzxlz.cn/gtdgunelkc.html

JS:   while (i < 10) { i++; }
来源：http://hz.yj202588.top/gttioewdqj.html

TS:   while (i < 10) { i++; }
来源：http://hz.ywan-chungtsiang.top/gtwcjiblcn.html

Java: while (i < 10) { i++; }
来源：http://hz.aizwys.cn/gtgdcoegsg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jiagoushi.top/gtklubkurw.html

Ruby: while i < 10; i += 1; end
来源：http://hz.aizwys.cn/gttwnnvlza.html

C#:   while (i < 10) { i++; }
来源：http://hz.pengpengdd.cyou/gthkcwvvlb.html

[B08] do-while（至少执行一次）
来源：http://hz.gzhubu.top/gtahsvcvxj.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jiagoushi.top/gtdookebbc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hfpthk.cn/gtqzrduxtz.html

JS:   do { i++; } while (i < 10);
来源：http://hz.tian-w.cn/gtaxmiavyr.html

TS:   do { i++; } while (i < 10);
来源：http://hz.svipenyu.cn/gtxwuwoyzp.html

Java: do { i++; } while (i < 10);
来源：http://hz.xylfe.cn/gtgoqzetcj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.nanxuanxn.top/gthefkuirg.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ivvv.top/gtxeduldie.html

C#:   do { i++; } while (i < 10);
来源：http://hz.ehwqpu.com/gtvnqlknxs.html

[B09] break 与 continue
来源：http://hz.daria6918.cn/gtjqhaogyf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.kuanghao11.cn/gtgghjqoff.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.pycfn.com/gtyeplknge.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ppjwa.cn/gtefquqrcg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gtbdsllxmv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtbytqhvmu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ybcxt.top/gtlccysmya.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yj20258.top/gtfgnapikb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxuanxn.top/gtqnhweovm.html

[B10] 遍历同时拿索引
来源：http://hz.tian-w.cn/gtpwkhwebv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhixingplan.top/gtpjlhaczx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.vqdsnc.cn/gtdmwqclcq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhongyouzk.top/gtqzlzeyvp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jqgfzy.top/gttgpfklyw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.fengsongda.top/gtumqfitqd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.aizwys.cn/gtbuhcsapd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cdnleiting.top/gtxclkkiyi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shanyushiyangtech.top/gtsfcwzgpq.html

[B11] 生成数字序列 / 区间
来源：http://hz.aibaodan.cn/gttnhaiifz.html

Py:   list(range(0, 10, 2))
来源：http://hz.iojbl.cn/gtcpgkytut.html

PHP:  range(0, 10, 2);
来源：http://hz.pengpengdd.cyou/gtcxcgqgoa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yj20258888.top/gtkixbrszi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhengqikj.top/gtuqmblfhb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinqigufen.top/gtxzzqrlup.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.shangyingyoupin.top/gtedbmpguq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.nanxinkj.top/gtnxynlsbb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.sweek.top/gtrqixqoqd.html

[B12] 跳出多层循环
来源：http://hz.chenlongwang.top/gtpdohvdfk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ehwqpu.com/gtnzyrpfbl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.mhx1999.top/gtonhelpzz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj202588.top/gtthfwsoyx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yueranfly.top/gtxxzuqygi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenlongwang.top/gtbvlwuayj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jiagoushi.top/gtsnjovyun.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhengqikj.top/gtrvzfqlmg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.sweek.top/gtkofqyzpe.html

[B13] 判断是否为数字
来源：http://hz.shanyushiyangtech.top/gtiygrafcl.html

Py:   isinstance(x, (int, float))
来源：http://hz.xuanzx.com/gtislptnqr.html

PHP:  is_numeric($x)
来源：http://hz.0kj1m.cn/gtittbesgb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ywan-chungtsiang.top/gtkqzjtyye.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shanyushiyangkeji.top/gtsrqxdssz.html

Java: x instanceof Number
来源：http://hz.hnqzz.top/gtmfzdaruv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.smart0.xyz/gtqfhajpcu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.nanxuanxn.top/gtfvnmhekt.html


<!-- 参考信息 -->