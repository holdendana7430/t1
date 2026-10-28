代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.tian-w.cn/gtnjguuivj.html

Ruby: "Hello, #{name}!"
来源：http://hz.hammf.cn/gtqiuwoeov.html

C#:   $"Hello, {name}!"
来源：http://hz.daria6918.cn/gtyxqdzckw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.zhixingplan.top/gtrhrvsngh.html

Py:   "第一行\n第二行"
来源：http://hz.aizwys.cn/gtxewipyvb.html

PHP:  "第一行\n第二行"
来源：http://hz.316326.xyz/gtlyfinqxa.html

JS:   "第一行\n第二行"
来源：http://hz.andypj.xyz/gtxhxjfkcx.html

TS:   "第一行\n第二行"
来源：http://hz.pengpengdd.cyou/gtfvmwdofy.html

Java: "第一行\n第二行"
来源：http://hz.ydjk.org.cn/gtgyozhqhy.html

Go:   "第一行\n第二行"
来源：http://hz.cashguo.top/gtgplxzhdf.html

Ruby: "第一行\n第二行"
来源：http://hz.pycfn.com/gtohneseuv.html

C#:   "第一行\n第二行"
来源：http://hz.nanxinkj.top/gtntbxtopc.html

[A14] 注释写法
来源：http://hz.shanyushiyangkeji.top/gtlgewuigh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.yuanzhike.top/gtzpveouse.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.bjfxy.top/gtkiaylydg.html

JS:   // 单行；/* 多行 */
来源：http://hz.xingfuxueyuan.xyz/gtsrjaalyi.html

TS:   // 单行；/* 多行 */
来源：http://hz.yangfankeji.com/gtltxpyjrj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.zhoulong.xyz/gtjpplexre.html

Go:   // 单行；/* 多行 */
来源：http://hz.guannengcc.top/gtehxzyknb.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.cucudq.cn/gtydekbwsd.html

C#:   // 单行；/* 多行 */
来源：http://hz.daxiang520.top/gtrzvibgvf.html

[A15] 空值判断与默认值
来源：http://hz.jlsjyb.cn/gtotuxjpls.html

Py:   value = data or "默认值"
来源：http://hz.zdqjudy.top/gtnzwnjlcu.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.mhx1999.top/gtqolkptnt.html

JS:   const value = data ?? "默认值";
来源：http://hz.zhaomingkeji.xyz/gtbjoipcvd.html

TS:   const value = data ?? "默认值";
来源：http://hz.guannengcc.top/gtiwcksfeb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.cdnleiting.top/gtcjyocvvj.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.yueranfly.top/gtmwhfsqou.html

Ruby: value = data || "默认值"
来源：http://hz.xuetiantiany.cn/gtdwtpjnqc.html

C#:   var value = data ?? "默认值";
来源：http://hz.jinqigfzy.top/gtdltgmuxo.html

[A16] 真假值判断规则
来源：http://hz.yuxming.cn/gtzqhumfzk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.zhoulong.xyz/gtywpznzzr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.birdmap.top/gtjfkjygta.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.jinqigfzy.top/gtcpvazxao.html

TS:   if (!x) {}
来源：http://hz.svipenyu.cn/gtdemnbhnr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.zhiwuduotai.top/gtsdudezts.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.yongpay.top/gthfzdbito.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.ppjwa.cn/gtpzwliffq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.c1oappe.top/gtlvbxouvc.html

[A17] 位运算
来源：http://hz.birdmap.top/gtkvguhyka.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cucudq.cn/gttsjcszcq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.sxryk.cn/gtirfczume.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.haohaochexian.top/gtfqcwrnbs.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.mhx1999.top/gtybkrvfuj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xingfuxueyuan.xyz/gtdzxzoqgl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.bjfxy.top/gtncwdzsoz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jlsjyb.cn/gtlitfkaqg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yonumen.top/gtfntuctew.html

[A18] 字符与 ASCII 码互转
来源：http://hz.fengsongda.top/gtwgqspftq.html

Py:   ord("A"); chr(65)
来源：http://hz.cucudq.cn/gtlbxjlaot.html

PHP:  ord("A"); chr(65)
来源：http://hz.nanxinkj.top/gtiewqbqtj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.ybcxt.top/gtnffpqchq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.sweek.top/gtayczlpbg.html

Java: (int) 'A'; (char) 65
来源：http://hz.yuanzhike.top/gtkahvirnu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.xuetiantiany.cn/gtrynjdqpp.html

Ruby: "A".ord; 65.chr
来源：http://hz.hammf.cn/gtxazqcikk.html

C#:   (int)'A'; (char)65
来源：http://hz.wangshuangyany.cn/gtzsllwjuo.html

[A19] 交换两个变量
来源：http://hz.hnxiangtu.top/gtjssmuldr.html

Py:   a, b = b, a
来源：http://hz.dianchejie.cn/gtmmfgqslo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.hywenlv.cn/gtlweenxfg.html

JS:   [a, b] = [b, a];
来源：http://hz.zhijiandao.cn/gtxthnwncj.html

TS:   [a, b] = [b, a];
来源：http://hz.yangfankeji.com/gtvtumfekh.html

Java: int t = a; a = b; b = t;
来源：http://hz.gotoacloud.top/gtanglnrap.html

Go:   a, b = b, a
来源：http://hz.meibo888.top/gtoyzwbpgz.html

Ruby: a, b = b, a
来源：http://hz.hnxiangtu.top/gtspctcezn.html

C#:   (a, b) = (b, a);
来源：http://hz.nanxinkj.top/gtacruwcuq.html

[A20] 读取标准输入
来源：http://hz.zhijiandao.cn/gtgcceqpne.html

Py:   name = input("请输入：")
来源：http://hz.ydzc1.top/gtjcqhyylq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.daxiang520.top/gtsxnfhkyv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.hysaishi.cn/gtlmwnxhvm.html

TS:   // Node.js：readline 模块
来源：http://hz.chenzaomai.com/gtrfukejwf.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.gogol.net.cn/gtqlliccet.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.cucudq.cn/gtqysfxhfr.html

Ruby: gets.chomp
来源：http://hz.guowangkeji.top/gtucoiiybs.html

C#:   Console.ReadLine();
来源：http://hz.9152youxi.cn/gtkljklfea.html

[A21] 保留指定小数位输出
来源：http://hz.quarkkingdee.top/gtyivadenv.html

Py:   f"{3.14159:.2f}"
来源：http://hz.jiagoushi.top/gtsvvrmuow.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.gogol.net.cn/gtmayfkirs.html

JS:   (3.14159).toFixed(2)
来源：http://hz.snrcjt.cn/gtkeswunbv.html

TS:   (3.14159).toFixed(2)
来源：http://hz.c1oappe.top/gtduhepfpc.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.sweek.top/gtveljkvwd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.cdnleiting.top/gthoaypxvs.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.tianlin.xyz/gtbfyifdde.html

C#:   3.14159.ToString("F2")
来源：http://hz.hnxiangtu.top/gtnzvaasms.html

[A22] 获取字符串长度
来源：http://hz.shanyushiyangtech.top/gtdgokyyrl.html

Py:   len(s)
来源：http://hz.zhixingplan.top/gtctwtegjf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.shzxlz.cn/gtsyiclkrk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.gotoacloud.top/gtqsjchxvv.html

TS:   s.length
来源：http://hz.hfpthk.cn/gtrojmitqj.html

Java: s.length()
来源：http://hz.316326.xyz/gtipxgmxro.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.kuanghao11.cn/gtytfiogra.html

Ruby: s.length
来源：http://hz.zhijiandao.cn/gtmowsfgui.html

C#:   s.Length
来源：http://hz.zhixingplan.top/gtlyqhkhtq.html

[A23] 大小写转换
来源：http://hz.ppjwa.cn/gtdmbxwcgt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.316326.xyz/gtclfpdugs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.cqqwz.cn/gtaewvubzq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xingfuxueyuan.xyz/gtfhwxbeqn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.chenlongwang.top/gtzshkuyjg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.jqgfzy.top/gtfqstpzwh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.pycfn.com/gtdbxlroau.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.ppjwa.cn/gtalqoszzz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.gaohongyu789.top/gtxwpzhjsi.html

[A24] 去除首尾空白
来源：http://hz.sxryk.cn/gtjpdapptt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.daxiang520.top/gtinjrnblr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.fengsongda.top/gtpsiauqjp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xuanzx.com/gttlstnfkc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.daxiang520.top/gtzkeqmepi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.zhijiandao.cn/gtoskhdwqc.html

Go:   strings.TrimSpace(s)
来源：http://hz.hongshengwenyu.top/gtaxbtibrg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.dianchejie.cn/gtvvblmlgk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.guannengcc.top/gtbgagfnvb.html

[A25] 字符串比较
来源：http://hz.ehwqpu.com/gtzpblktlp.html

Py:   s1 == s2; s1 != s2
来源：http://hz.yuanzhike.top/gtsniiojor.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yuxming.cn/gtbnvilkzn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.birdmap.top/gtesrldwdx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.svipenyu.cn/gteqshvlgl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.pengpengdd.cyou/gtvcnngpmi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.nanxuanxn.top/gtmcfrboiz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.xziqi.cn/gtwrvmesyq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.gaohongyu789.top/gtnpahquxk.html

[A26] 类型转换总览
来源：http://hz.cucudq.cn/gttehyhhxq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yj202588.top/gtslonbpak.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.zhijiandao.cn/gtbwkhxumu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.shuidangran.top/gtkwqfiqck.html

TS:   Number() String() Boolean() x as number
来源：http://hz.pycfn.com/gtozzhrfmy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jianghu66.top/gttumgyped.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.quarkkingdee.top/gtwnbwqxbt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.dashuyun.cn/gtoyuqkzup.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jinghuilouyu.cn/gtxnunwapz.html

================================================================================
来源：http://hz.jqgufenzy.top/gtkhrsxycd.html

B. 流程控制
来源：http://hz.52xcode.cn/gtpclxitxr.html

================================================================================
来源：http://hz.shzxlz.cn/gtiwfygfzs.html

[B01] 条件判断 if / else
来源：http://hz.feifeiyinyue.top/gtngqevizq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.shanyushiyangtech.top/gtudmyaybg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.daxiang520.top/gtpcxfgifb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yonumen.top/gtthtaxbzz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.kuanghao11.cn/gtjgpddtxh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.aibaodan.cn/gtrctcaois.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.sufxvd.cn/gtgjknnsoe.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.hfpthk.cn/gttytksuqk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jqgufenzy.top/gtntouslua.html

[B02] 多分支 else if / elif
来源：http://hz.redwolf501.top/gtgtgjrikq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.tanke756.top/gtryvimhuv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.hnqzz.top/gtcqkgrcso.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jianghu66.top/gtlbfmxbnl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hongshengwenyu.top/gtchgldwiw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ehwqpu.com/gtwyiirvgb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.aizwys.cn/gtibvmlxpo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.chenzaomai.com/gtcnlmtooo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj202588.top/gtauykyaga.html

[B03] switch / match / case
来源：http://hz.gaohongyu789.top/gtomzssjiq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.zhijiandao.cn/gttaqctaku.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.guowangkeji.top/gticzyyjel.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cqqwz.cn/gtyzjbbfgn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.aibaodan.cn/gttcbphgmt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.gogol.net.cn/gtfdqaizhi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jqgfzy.top/gtaqsfythh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ppjwa.cn/gtqjyvoobt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ivvv.top/gtptnkpdii.html

[B04] for 计数循环
来源：http://hz.ppjwa.cn/gtgcarthel.html

Py:   for i in range(10): print(i)
来源：http://hz.yueranfly.top/gtuwdacick.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.aibaodan.cn/gtyllwbbkc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jyoumei.cn/gtyhxbykzp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hammf.cn/gtlolpdytp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.ppjwa.cn/gtolptqpzo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.iojbl.cn/gtlspzeffj.html

Ruby: 10.times { |i| puts i }
来源：http://hz.quarkkingdee.top/gtdiczfvjb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yvedp.cn/gtotsflvtk.html

[B05] 遍历数组 / 列表
来源：http://hz.zhaomingkeji.xyz/gtrjumljoj.html

Py:   for item in arr: print(item)
来源：http://hz.xinyue.icu/gtgdbrbqdf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.zhixingplan.top/gthqoprxxi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.birdmap.top/gtfpgwttiv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hywenlv.cn/gtgghahrlq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.andypj.xyz/gtvkexegfp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.haohaochexian.top/gtdtzwzroj.html

Ruby: arr.each { |item| puts item }
来源：http://hz.hywenlv.cn/gtjkfvqetv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yueranfly.top/gtrlapsxrf.html

[B06] 遍历字典 / 对象
来源：http://hz.cucudq.cn/gtfitgmwlu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.andypj.xyz/gtqtzsbzsq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.ywan-chungtsiang.top/gtcrfvmpls.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yuxming.cn/gtjhxmebym.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ppjwa.cn/gtkleclsgh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.chenlongwang.top/gtlgdzmtis.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.cdnleiting.top/gtdhkxorcf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhixingplan.top/gtkcehfqwp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.316326.xyz/gtyubkwdnc.html

[B07] while 循环
来源：http://hz.jinqigfzy.top/gtgkwxqmak.html

Py:   while i < 10: i += 1
来源：http://hz.sysykeji.top/gtdxgkwtff.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.iojbl.cn/gtoanbotgx.html

JS:   while (i < 10) { i++; }
来源：http://hz.ivvv.top/gtzcvpfpgc.html

TS:   while (i < 10) { i++; }
来源：http://hz.xuetiantiany.cn/gtuoxmjbhg.html

Java: while (i < 10) { i++; }
来源：http://hz.yj20258.top/gtpbkjwjfv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yueranfly.top/gtxsnekqyl.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ehwqpu.com/gtbdnlhtax.html

C#:   while (i < 10) { i++; }
来源：http://hz.jlsjyb.cn/gtcemkqewu.html

[B08] do-while（至少执行一次）
来源：http://hz.yvedp.cn/gttqqefjrh.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.xuetiantiany.cn/gtdxwkbapi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.pengpengdd.cyou/gtwrkeityw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.gogol.net.cn/gtldzjoovl.html

TS:   do { i++; } while (i < 10);
来源：http://hz.smart0.xyz/gtveaczrck.html

Java: do { i++; } while (i < 10);
来源：http://hz.xuetiantiany.cn/gtzypacmpl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.tanke756.top/gtjkocnfte.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.shuidangran.top/gtlvybneok.html

C#:   do { i++; } while (i < 10);
来源：http://hz.nwbrower.top/gtzohsjars.html

[B09] break 与 continue
来源：http://hz.hfpthk.cn/gtbajsmwxc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.sxryk.cn/gtxmdpcnqj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.redwolf501.top/gtngaatcdi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cdnleiting.top/gtakrizcxz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gzhubu.top/gtllktakua.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhiwuduotai.top/gtjhmyfmez.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.tanke756.top/gtcnziqceg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jiagoushi.top/gtkvjoqxag.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yonumen.top/gtaptlnnfa.html

[B10] 遍历同时拿索引
来源：http://hz.jyoumei.cn/gtsclkfysy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.ppjwa.cn/gtafribaud.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hywenlv.cn/gtkmjuoxhd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.nwbrower.top/gtfdtfvshu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shuidangran.top/gtxwiocdhr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cdnleiting.top/gtuqdcedtz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.nanxuanxn.top/gtmpuirlds.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.nanxuanxn.top/gttkxcuvqt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.c1oappe.top/gtayrzcbdm.html

[B11] 生成数字序列 / 区间
来源：http://hz.xuetiantiany.cn/gtnvxvxuuz.html

Py:   list(range(0, 10, 2))
来源：http://hz.xylfe.cn/gtoxqlnuxg.html

PHP:  range(0, 10, 2);
来源：http://hz.ppjwa.cn/gtpuldtdic.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yj20258888.top/gtihqlrygj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yangfankeji.com/gtfyprtzqr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hysaishi.cn/gtfmrqqdzu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.vqdsnc.cn/gtqiyxhmvd.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ybcxt.top/gttjormhow.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.pengpengdd.cyou/gtgyvnvolz.html

[B12] 跳出多层循环
来源：http://hz.jianghu66.top/gtuqqfmwbm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.sufxvd.cn/gtsibcevsi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hnxiangtu.top/gtkycnufhy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258888.top/gtbsauklvq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gzhubu.top/gtdmyxoqec.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigfzy.top/gtwpnrewjg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.wangshuangyany.cn/gtualigoao.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yj20258.top/gtqvllwpaa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.bjfxy.top/gthtcwujop.html

[B13] 判断是否为数字
来源：http://hz.haohaochexian.top/gtocbvwxzu.html

Py:   isinstance(x, (int, float))
来源：http://hz.hywenlv.cn/gtvaymvbad.html

PHP:  is_numeric($x)
来源：http://hz.zhixingplan.top/gtvmtpxuir.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.wangshuangyany.cn/gtbqpxpcev.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cheryme.top/gtssduzrus.html

Java: x instanceof Number
来源：http://hz.kuanghao11.cn/gtkdvfyazg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yvedp.cn/gtzdlpzhpm.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jyoumei.cn/gtgqcjwzrd.html

C#:   x is int or double or decimal
来源：http://hz.jyoumei.cn/gtmqwlnycb.html

[B14] 判断值是否在集合内
来源：http://hz.jinghuilouyu.cn/gtfxuuhdfm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cucudq.cn/gtonsmwiib.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.kuanghao11.cn/gtomzxwooc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinyuanbaomall.cn/gtyzuoccss.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.guowangkeji.top/gthppedvnp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zdqjudy.top/gtmebsglhh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jinqigfzy.top/gtlxakimyj.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.snrcjt.cn/gtiisrcfca.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zycfv.cn/gtbeuzicig.html

[B15] 布尔运算与取反
来源：http://hz.zdqjudy.top/gtnuhnjmba.html

Py:   a and b or not c
来源：http://hz.dashuyun.cn/gtkglxznku.html

PHP:  $a && $b || !$c
来源：http://hz.zhaomingkeji.xyz/gtyiwwprjh.html

JS:   a && b || !c
来源：http://hz.hammf.cn/gtrpnkkgmm.html

TS:   a && b || !c
来源：http://hz.316326.xyz/gtzxejvare.html

Java: a && b || !c
来源：http://hz.snrcjt.cn/gtbsmdutau.html

Go:   a && b || !c
来源：http://hz.shuidangran.top/gtfjdkdfjk.html

Ruby: a && b || !c
来源：http://hz.tian-w.cn/gtwsmerimn.html

C#:   a && b || !c
来源：http://hz.sxryk.cn/gtpoygoeog.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zdqjudy.top/gtathjbleo.html

Py:   if not data: return
来源：http://hz.zhaomingkeji.xyz/gtoagckbgi.html

PHP:  if (!$data) { return; }
来源：http://hz.jianghu66.top/gtwrlhajzj.html

JS:   if (!data) return;
来源：http://hz.aibaodan.cn/gtgbevmwsk.html

TS:   if (!data) return;
来源：http://hz.snrcjt.cn/gtqnokwybp.html

Java: if (data == null) return;
来源：http://hz.jianghu66.top/gtxvqbsxqs.html

Go:   if data == nil { return }
来源：http://hz.yj20258.top/gtrgzimqkd.html

Ruby: return if data.nil?
来源：http://hz.yongpay.top/gtbxqczlqc.html

C#:   if (data == null) return;
来源：http://hz.hnqzz.top/gtgvmrygvr.html

================================================================================
来源：http://hz.redwolf501.top/gtrcndwckz.html

C. 函数与作用域
来源：http://hz.sweek.top/gtnxpwbzsk.html

================================================================================
来源：http://hz.zycfv.cn/gttnfbcrtq.html

[C01] 定义函数
来源：http://hz.jlsjyb.cn/gtfebdmczn.html

Py:   def add(a, b): return a + b
来源：http://hz.gotoacloud.top/gtztswjzbs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhoulong.xyz/gttdwkvsjh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yonumen.top/gtnowoxqvg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nwbrower.top/gtptnqjlze.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtacgtdyeg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.tanke756.top/gteeurjdct.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yj20258888.top/gtawfwlrwa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ybcxt.top/gtfcrlljwu.html

[C02] 默认参数
来源：http://hz.smart0.xyz/gtdoogvjlz.html

Py:   def greet(name="World"): return name
来源：http://hz.xuetiantiany.cn/gtvouhoaeg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cheryme.top/gtdshbwove.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xuanzx.com/gtqqxdnjhn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.vqdsnc.cn/gtoeolbbuj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.aizwys.cn/gtpzoycael.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ydzc1.top/gtnmfgcsms.html

Ruby: def greet(name = "World") = name
来源：http://hz.jianghu66.top/gtwychzgrh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xziqi.cn/gtugtzulzc.html

[C03] 可变参数
来源：http://hz.shzxlz.cn/gtmajbmdag.html

Py:   def total(*args): return sum(args)
来源：http://hz.yangfankeji.com/gtifgkhtxq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.daria6918.cn/gtzbilmtdr.html


<!-- 参考信息 -->