代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.chenjidiqi.icu/gtrtzozras.html

Java: new Random().nextInt(100) + 1
来源：http://hz.cqqwz.cn/gtnquiqufo.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.wangshuangyany.cn/gtowhzqora.html

Ruby: rand(1..100)
来源：http://hz.yueranfly.top/gtpxvqftgc.html

C#:   new Random().Next(1, 101)
来源：http://hz.chenlongwang.top/gtapoeucfn.html

[A11] 条件表达式（三元）
来源：http://hz.mhx1999.top/gtxclznmaf.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.hfpthk.cn/gtycwqtkvf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.c1oappe.top/gtgcflynwp.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.yuanzhike.top/gtdqcdtfxj.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.jinqigufen.top/gthsmgwxbn.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.zhiwuduotai.top/gtjczacayr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.tianlin.xyz/gtgsbarptz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.jinghuilouyu.cn/gtcbpzmfcb.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.yueranfly.top/gtefaytdvm.html

[A12] 字符串插值 / 格式化
来源：http://hz.wangshuangyany.cn/gtkbzwwsbu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.gogol.net.cn/gtaftskzby.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.yanxiufei.cn/gtsxcsrvdr.html

JS:   `Hello, ${name}!`
来源：http://hz.shanyushiyangkeji.top/gtmxciyjbo.html

TS:   `Hello, ${name}!`
来源：http://hz.hnqzz.top/gtrxaeqedm.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.zhoulong.xyz/gtqzzmwivx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.meibo888.top/gtlslnvyrm.html

Ruby: "Hello, #{name}!"
来源：http://hz.cashguo.top/gtpaheeusj.html

C#:   $"Hello, {name}!"
来源：http://hz.wangdashe.top/gtmoyyslyk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.daxiang520.top/gtkjgvcbsf.html

Py:   "第一行\n第二行"
来源：http://hz.yongpay.top/gtafacgplo.html

PHP:  "第一行\n第二行"
来源：http://hz.gzhubu.top/gtjpfanxzg.html

JS:   "第一行\n第二行"
来源：http://hz.hongshengwenyu.top/gtlagroauz.html

TS:   "第一行\n第二行"
来源：http://hz.bjfxy.top/gtnjvigsmn.html

Java: "第一行\n第二行"
来源：http://hz.tanke756.top/gtntedeira.html

Go:   "第一行\n第二行"
来源：http://hz.zhijiandao.cn/gtlehkjbmf.html

Ruby: "第一行\n第二行"
来源：http://hz.hfpthk.cn/gtznnyhhju.html

C#:   "第一行\n第二行"
来源：http://hz.9152youxi.cn/gtjxgwkvun.html

[A14] 注释写法
来源：http://hz.vqdsnc.cn/gtktcnvdth.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.zdqjudy.top/gtuueobrty.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.xylfe.cn/gtilgjatwn.html

JS:   // 单行；/* 多行 */
来源：http://hz.chenjidiqi.icu/gtzgqqsani.html

TS:   // 单行；/* 多行 */
来源：http://hz.kuanghao11.cn/gtsubbzfhk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.yj20258.top/gtxluieimb.html

Go:   // 单行；/* 多行 */
来源：http://hz.havefunace.top/gtibvsylkl.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.cdnleiting.top/gtajfpfbfc.html

C#:   // 单行；/* 多行 */
来源：http://hz.zhoulong.xyz/gtdooldixy.html

[A15] 空值判断与默认值
来源：http://hz.cdnleiting.top/gtiiwzhyja.html

Py:   value = data or "默认值"
来源：http://hz.cashguo.top/gtslnoastk.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.zhiwuduotai.top/gtuvwsvqft.html

JS:   const value = data ?? "默认值";
来源：http://hz.tanke756.top/gtxcntdqdq.html

TS:   const value = data ?? "默认值";
来源：http://hz.zdqjudy.top/gteysyyirb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.wangshuangyany.cn/gtkwmyxkwb.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.shangyingyoupin.top/gtigmodhvp.html

Ruby: value = data || "默认值"
来源：http://hz.cashguo.top/gtckegmhhl.html

C#:   var value = data ?? "默认值";
来源：http://hz.chenjidiqi.icu/gtainpmerk.html

[A16] 真假值判断规则
来源：http://hz.chenzaomai.com/gtkmclsyyq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.daria6918.cn/gtqhcdvoin.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.sxryk.cn/gtdfbhrnko.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.aibaodan.cn/gtgkrnywcc.html

TS:   if (!x) {}
来源：http://hz.wangdashe.top/gtusejxond.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.aizwys.cn/gtklydsarl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.quarkkingdee.top/gtxupsumrb.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.zhijiandao.cn/gtpwurhsbz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.ydjk.org.cn/gtdlzwaiqg.html

[A17] 位运算
来源：http://hz.nwbrower.top/gtohbsuppj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.dianchejie.cn/gtfykusbis.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yj20258888.top/gtmyvvhnir.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xziqi.cn/gtudppnxwg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.chenjidiqi.icu/gtxcoeqnlv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jlsjyb.cn/gtndzusrwx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.zycfv.cn/gtzfxblhgl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.aibaodan.cn/gtuxgiggew.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.0kj1m.cn/gtrrzelqdg.html

[A18] 字符与 ASCII 码互转
来源：http://hz.sweek.top/gtzauidreb.html

Py:   ord("A"); chr(65)
来源：http://hz.jinghuilouyu.cn/gtiqsoxgqj.html

PHP:  ord("A"); chr(65)
来源：http://hz.zhaomingkeji.xyz/gtxqrjugub.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.nanxuanxn.top/gtpadiosni.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yj202588.top/gtrgyghwuo.html

Java: (int) 'A'; (char) 65
来源：http://hz.tanke756.top/gtceplewdo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.xziqi.cn/gtmgneisjr.html

Ruby: "A".ord; 65.chr
来源：http://hz.zhixingplan.top/gtthnerwcr.html

C#:   (int)'A'; (char)65
来源：http://hz.snrcjt.cn/gttemndauw.html

[A19] 交换两个变量
来源：http://hz.yj202588.top/gtedarihzg.html

Py:   a, b = b, a
来源：http://hz.sweek.top/gtzhfrwipg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.hammf.cn/gtoyoxtojb.html

JS:   [a, b] = [b, a];
来源：http://hz.hammf.cn/gtgrscimhv.html

TS:   [a, b] = [b, a];
来源：http://hz.andypj.xyz/gtnofrmcdh.html

Java: int t = a; a = b; b = t;
来源：http://hz.hnqzz.top/gtycrfaduj.html

Go:   a, b = b, a
来源：http://hz.gzhubu.top/gtwpamihqp.html

Ruby: a, b = b, a
来源：http://hz.tianlin.xyz/gtniwwzmiv.html

C#:   (a, b) = (b, a);
来源：http://hz.birdmap.top/gtievgnfwz.html

[A20] 读取标准输入
来源：http://hz.jinqigufen.top/gtszslthci.html

Py:   name = input("请输入：")
来源：http://hz.hnxiangtu.top/gtiybqpdyv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.xziqi.cn/gtlqfhnido.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.9152youxi.cn/gtrltiheoh.html

TS:   // Node.js：readline 模块
来源：http://hz.yueranfly.top/gtbrqpbutq.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.nwbrower.top/gtbtzldyki.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.mhx1999.top/gtfvfhmsfl.html

Ruby: gets.chomp
来源：http://hz.shanyushiyangkeji.top/gtqabjrqyy.html

C#:   Console.ReadLine();
来源：http://hz.kuanghao11.cn/gtesfhfokb.html

[A21] 保留指定小数位输出
来源：http://hz.wangshuangyany.cn/gtoceiqwpx.html

Py:   f"{3.14159:.2f}"
来源：http://hz.mhx1999.top/gtwworeiin.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.aizwys.cn/gtssdqvzqs.html

JS:   (3.14159).toFixed(2)
来源：http://hz.zhixingplan.top/gttnrdkgbf.html

TS:   (3.14159).toFixed(2)
来源：http://hz.hnqzz.top/gtknecrpqs.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.shangyingyoupin.top/gtsubfkzpr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.meibo888.top/gtohymxqgd.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.svipenyu.cn/gtzwkimgzg.html

C#:   3.14159.ToString("F2")
来源：http://hz.shzxlz.cn/gthxqmjbwk.html

[A22] 获取字符串长度
来源：http://hz.hnxiangtu.top/gtyvfqpphu.html

Py:   len(s)
来源：http://hz.xinyue.icu/gtrlgjkwyx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.chenzaomai.com/gtjfeqestj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.yangfankeji.com/gtynsoafmq.html

TS:   s.length
来源：http://hz.52xcode.cn/gttredmfsj.html

Java: s.length()
来源：http://hz.bjfxy.top/gtfiuebmre.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.9152youxi.cn/gtgihhbiem.html

Ruby: s.length
来源：http://hz.wangdashe.top/gtompgurmp.html

C#:   s.Length
来源：http://hz.cheryme.top/gtdnwkznrh.html

[A23] 大小写转换
来源：http://hz.haohaochexian.top/gtedhxiyoj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.zhijiandao.cn/gtpmxcxscx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.andypj.xyz/gtbqqzysrd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.cqqwz.cn/gtzauftdog.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.cheryme.top/gtcymvthvo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.shuidangran.top/gtzhwmwmif.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yj202588.top/gtskhguztl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yanxiufei.cn/gtixcmrmap.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.wangshuangyany.cn/gtvzhmbmow.html

[A24] 去除首尾空白
来源：http://hz.0kj1m.cn/gtaacrjkrk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.ppjwa.cn/gtdzlffrvc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yanxiufei.cn/gtnsdhmvus.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.cucudq.cn/gtmpjupejn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.haohaochexian.top/gtmtnyjckm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.hammf.cn/gtkrssfmul.html

Go:   strings.TrimSpace(s)
来源：http://hz.ehwqpu.com/gtbmiyqdcp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.ivvv.top/gtrlueiswp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.shanyushiyangtech.top/gtqisfwyjv.html

[A25] 字符串比较
来源：http://hz.xingfuxueyuan.xyz/gtpyalxsbv.html

Py:   s1 == s2; s1 != s2
来源：http://hz.cqqwz.cn/gtlzfxhbtl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ywan-chungtsiang.top/gtmiwwkxnb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ywan-chungtsiang.top/gtafmmgtim.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhijiandao.cn/gtrckpbzmt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.52xcode.cn/gtrogsxacm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.sufxvd.cn/gtedymerku.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.zhixingplan.top/gtstumjqty.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.guowangkeji.top/gtfxjscyfd.html

[A26] 类型转换总览
来源：http://hz.daria6918.cn/gtbazwrwsa.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zhaomingkeji.xyz/gtaxaxzuwy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.quarkkingdee.top/gtikjkedkn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jyoumei.cn/gtbkzrtmce.html

TS:   Number() String() Boolean() x as number
来源：http://hz.guowangkeji.top/gtuubikmmp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.xuanzx.com/gtcoydkfoq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhaomingkeji.xyz/gtwdjidmlq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.mhx1999.top/gtjvtvhhia.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.xingfuxueyuan.xyz/gtzhdpuori.html

================================================================================
来源：http://hz.andypj.xyz/gttgcvmrfj.html

B. 流程控制
来源：http://hz.zhaomingkeji.xyz/gtxtiriudh.html

================================================================================
来源：http://hz.zhengqikj.top/gtbetmzdlu.html

[B01] 条件判断 if / else
来源：http://hz.xylfe.cn/gtqedxsxvx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jlsjyb.cn/gtdlqicrlp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.cqqwz.cn/gtckvkvmcs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.9152youxi.cn/gtpqcqkpla.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.cqqwz.cn/gtcmobslga.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zdqjudy.top/gtetaselhk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.ydzc1.top/gtdpzevhcg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.gogol.net.cn/gttwuvkzmf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hfpthk.cn/gtvfonenjl.html

[B02] 多分支 else if / elif
来源：http://hz.zhiwuduotai.top/gtahpwfvdd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.ybcxt.top/gtjaqhvmuv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.dianchejie.cn/gtpndbdwey.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dashuyun.cn/gtjqqfoaiz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yueranfly.top/gtqxgcjhyf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jiagoushi.top/gtxmombchn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.tianlin.xyz/gteupijwpo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jlsjyb.cn/gtguhrdkkv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.guannengcc.top/gtcmuxxagf.html

[B03] switch / match / case
来源：http://hz.haohaochexian.top/gtugwcziiq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.pengpengdd.cyou/gtiohvxqbh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.gzhubu.top/gttngcwswx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.fengsongda.top/gtwxphyoze.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhongyouzk.top/gtgedlvvex.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.ivvv.top/gtbadwriij.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jinghuilouyu.cn/gtkquxqovw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hnxiangtu.top/gthmaybkyb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.cheryme.top/gthppmcdnx.html

[B04] for 计数循环
来源：http://hz.zhoulong.xyz/gtxzavdpql.html

Py:   for i in range(10): print(i)
来源：http://hz.gzhubu.top/gtsatghtxt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.pengpengdd.cyou/gttmoyevse.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gzhubu.top/gtwgnifmlp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xuanzx.com/gtfryjjepw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.guannengcc.top/gtsdsuoouk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.hongshengwenyu.top/gtlpwzwhip.html

Ruby: 10.times { |i| puts i }
来源：http://hz.chenzaomai.com/gtquydcprb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.birdmap.top/gtuhcqnclz.html

[B05] 遍历数组 / 列表
来源：http://hz.0kj1m.cn/gtezudhdty.html

Py:   for item in arr: print(item)
来源：http://hz.hnqzz.top/gtejnwwyks.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.shanyushiyangkeji.top/gtmshnzvsy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.shangyingyoupin.top/gtorzzfydr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hfpthk.cn/gtuotjybwx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yueranfly.top/gtgpbvtiwg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.smart0.xyz/gtubndeinw.html

Ruby: arr.each { |item| puts item }
来源：http://hz.tianlin.xyz/gthnfrdfid.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.wangdashe.top/gtnmjtwqgw.html

[B06] 遍历字典 / 对象
来源：http://hz.cucudq.cn/gtcbqtxbuq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.pycfn.com/gtgjwghqfg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.0kj1m.cn/gtmkzalrgk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhijiandao.cn/gtpqeglfxo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.mhx1999.top/gtgfnarkpt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zhixingplan.top/gttufgbtnp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.cqqwz.cn/gtxknmgfjp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.birdmap.top/gtpddhgbrn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.redwolf501.top/gtddxgdvct.html

[B07] while 循环
来源：http://hz.jlsjyb.cn/gtpybqgdmq.html

Py:   while i < 10: i += 1
来源：http://hz.yuanzhike.top/gtkptpfzhx.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zdqjudy.top/gtlphsruqf.html

JS:   while (i < 10) { i++; }
来源：http://hz.sysykeji.top/gthwyultfy.html

TS:   while (i < 10) { i++; }
来源：http://hz.mhx1999.top/gtabrfvuwr.html

Java: while (i < 10) { i++; }
来源：http://hz.haohaochexian.top/gtjqoyisrk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.cashguo.top/gtwfrcxndi.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhijiandao.cn/gtpbltesse.html

C#:   while (i < 10) { i++; }
来源：http://hz.shuidangran.top/gtheuhcmel.html

[B08] do-while（至少执行一次）
来源：http://hz.andypj.xyz/gtyfedixtw.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ydjk.org.cn/gtxyfoypbd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.xinyue.icu/gtlmnpyroa.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yangfankeji.com/gtxhyrhslr.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yuxming.cn/gthwaclwbh.html

Java: do { i++; } while (i < 10);
来源：http://hz.yj20258888.top/gtqxbhpcpl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hysaishi.cn/gtgetnngqf.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.iojbl.cn/gtqkevzefq.html

C#:   do { i++; } while (i < 10);
来源：http://hz.9152youxi.cn/gthuuqnmwt.html

[B09] break 与 continue
来源：http://hz.ydjk.org.cn/gtlsovawls.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.pengpengdd.cyou/gtdlqgozps.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.tian-w.cn/gtxnmznivr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hywenlv.cn/gtowfvyyav.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yangfankeji.com/gtmbmfvfmw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.bjfxy.top/gteywralcc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.nanxinkj.top/gtbqxbpojc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.fengsongda.top/gtgsfjgdta.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.iojbl.cn/gtkcvqsavb.html

[B10] 遍历同时拿索引
来源：http://hz.jinqigfzy.top/gtlnkdnoww.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yj20258888.top/gtdpkgtljz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.meibo888.top/gtqfigajql.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.gaohongyu789.top/gtzhzuepmf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yj202588.top/gtuvbydsbx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yanxiufei.cn/gtsqgfhijz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.cheryme.top/gtsvbghsdc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cashguo.top/gtbgbruznt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinqigfzy.top/gtboprhonk.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinghuilouyu.cn/gtsvrmntuz.html

Py:   list(range(0, 10, 2))
来源：http://hz.shanyushiyangtech.top/gtvldlqbua.html

PHP:  range(0, 10, 2);
来源：http://hz.ybcxt.top/gtakjtxhrw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhijiandao.cn/gtzfiwovtn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xuetiantiany.cn/gttxchuexo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.guowangkeji.top/gtjebakfey.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.kuanghao11.cn/gtibcboqfc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jinyuanbaomall.cn/gtfceshylq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.snrcjt.cn/gtxauslagf.html

[B12] 跳出多层循环
来源：http://hz.zhixingplan.top/gtjkailcgf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.wangshuangyany.cn/gtsvdqqaoo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yuanzhike.top/gtavqmfqgf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jiagoushi.top/gtjqtsxahc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhaomingkeji.xyz/gtwryybdnc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yvedp.cn/gtjrvdudjm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.haohaochexian.top/gtlhojwicf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.aizwys.cn/gtlvmpypma.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hywenlv.cn/gtxrrxluvr.html

[B13] 判断是否为数字
来源：http://hz.chenjidiqi.icu/gtxscbyhkr.html

Py:   isinstance(x, (int, float))
来源：http://hz.havefunace.top/gtdiumcman.html

PHP:  is_numeric($x)
来源：http://hz.jlsjyb.cn/gtxentrulb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yongpay.top/gtxmgjvayl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.guannengcc.top/gtcsrxhwhg.html

Java: x instanceof Number
来源：http://hz.zdqjudy.top/gtvofzbaki.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.quarkkingdee.top/gtsqwpejqr.html

Ruby: x.is_a?(Numeric)
来源：http://hz.bjfxy.top/gtzqqpnzcx.html

C#:   x is int or double or decimal
来源：http://hz.shuidangran.top/gtxjcxxhux.html

[B14] 判断值是否在集合内
来源：http://hz.ivvv.top/gtisrtbrqe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yongpay.top/gtmlmjqgpx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jqgufenzy.top/gtiyvzpsuz.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.mhx1999.top/gtyqiqxryf.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ydjk.org.cn/gtusabmffu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cqqwz.cn/gtmconcbsv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sufxvd.cn/gtnalbvnjn.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yvedp.cn/gtdrrntwzw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenjidiqi.icu/gtynedogzc.html

[B15] 布尔运算与取反
来源：http://hz.yongpay.top/gtkilntnrt.html

Py:   a and b or not c
来源：http://hz.zhijiandao.cn/gttekdpyhp.html

PHP:  $a && $b || !$c
来源：http://hz.tian-w.cn/gtdjugbtfp.html

JS:   a && b || !c
来源：http://hz.cdnleiting.top/gtwdizvump.html

TS:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtqufxiakm.html

Java: a && b || !c
来源：http://hz.jinqigfzy.top/gtlmwxovkl.html

Go:   a && b || !c
来源：http://hz.yj20258888.top/gtlrnhwiss.html

Ruby: a && b || !c
来源：http://hz.zhongyouzk.top/gtxwdayknn.html

C#:   a && b || !c
来源：http://hz.yangfankeji.com/gthturqhui.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.daxiang520.top/gtgksqwcyo.html

Py:   if not data: return
来源：http://hz.chenlongwang.top/gteevmewwr.html

PHP:  if (!$data) { return; }
来源：http://hz.snrcjt.cn/gtrbxvcfom.html

JS:   if (!data) return;
来源：http://hz.yuxming.cn/gtjxiilldk.html

TS:   if (!data) return;
来源：http://hz.cqqwz.cn/gtkfjblbmw.html

Java: if (data == null) return;
来源：http://hz.zhijiandao.cn/gtkcbidxeq.html

Go:   if data == nil { return }
来源：http://hz.yongpay.top/gttkeoetnh.html

Ruby: return if data.nil?
来源：http://hz.jinyuanbaomall.cn/gtqijyrxhy.html

C#:   if (data == null) return;
来源：http://hz.zhongyouzk.top/gtbvvscahn.html

================================================================================
来源：http://hz.iojbl.cn/gtpfpcidpe.html

C. 函数与作用域
来源：http://hz.aizwys.cn/gtxkbkdqqj.html

================================================================================
来源：http://hz.shuidangran.top/gtxttjmegy.html

[C01] 定义函数
来源：http://hz.feifeiyinyue.top/gtlvqfchoh.html


<!-- 参考信息 -->