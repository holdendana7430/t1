代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.ppjwa.cn/gtpjijbcuu.html

JS:   `Hello, ${name}!`
来源：http://hz.tian-w.cn/gtdgahsmkx.html

TS:   `Hello, ${name}!`
来源：http://hz.bjfxy.top/gtcubmehdf.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.hywenlv.cn/gtfdzbllnp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.sxryk.cn/gtoomjramq.html

Ruby: "Hello, #{name}!"
来源：http://hz.shanyushiyangtech.top/gtdswkcbmb.html

C#:   $"Hello, {name}!"
来源：http://hz.pengpengdd.cyou/gtfokohngy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.jianghu66.top/gtutyrjryv.html

Py:   "第一行\n第二行"
来源：http://hz.zhixingplan.top/gtmikhzxyx.html

PHP:  "第一行\n第二行"
来源：http://hz.xingfuxueyuan.xyz/gttkejmlni.html

JS:   "第一行\n第二行"
来源：http://hz.hfpthk.cn/gtusjpwohq.html

TS:   "第一行\n第二行"
来源：http://hz.shzxlz.cn/gtpalnbsye.html

Java: "第一行\n第二行"
来源：http://hz.316326.xyz/gtesmgmery.html

Go:   "第一行\n第二行"
来源：http://hz.zhaomingkeji.xyz/gtrgynlroj.html

Ruby: "第一行\n第二行"
来源：http://hz.jlsjyb.cn/gtmxkxeepg.html

C#:   "第一行\n第二行"
来源：http://hz.ybcxt.top/gtbibmhiab.html

[A14] 注释写法
来源：http://hz.jiagoushi.top/gtvdxnmuee.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.cucudq.cn/gtzkvusckv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.mhx1999.top/gtrtlthplp.html

JS:   // 单行；/* 多行 */
来源：http://hz.hfpthk.cn/gtkchwavhe.html

TS:   // 单行；/* 多行 */
来源：http://hz.jianghu66.top/gtdqjjwlva.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.sufxvd.cn/gtepbcieyc.html

Go:   // 单行；/* 多行 */
来源：http://hz.shuidangran.top/gthwedxtwe.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.iojbl.cn/gtqzdlqilw.html

C#:   // 单行；/* 多行 */
来源：http://hz.jyoumei.cn/gtlqmbueer.html

[A15] 空值判断与默认值
来源：http://hz.zhaomingkeji.xyz/gtwlpltqmn.html

Py:   value = data or "默认值"
来源：http://hz.sufxvd.cn/gtlxeuewzm.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.ywan-chungtsiang.top/gtfaevatzs.html

JS:   const value = data ?? "默认值";
来源：http://hz.guannengcc.top/gtycugjbqo.html

TS:   const value = data ?? "默认值";
来源：http://hz.nanxinkj.top/gtfmbmihsw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.iojbl.cn/gtvnvduxac.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.zhiwuduotai.top/gtanaedcwu.html

Ruby: value = data || "默认值"
来源：http://hz.havefunace.top/gtqfebiycv.html

C#:   var value = data ?? "默认值";
来源：http://hz.hnqzz.top/gtderfqbin.html

[A16] 真假值判断规则
来源：http://hz.sweek.top/gtxkzmziea.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.ywan-chungtsiang.top/gtenqijoyx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.yuanzhike.top/gtflcjegjr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.iojbl.cn/gtzpxhuyvk.html

TS:   if (!x) {}
来源：http://hz.meibo888.top/gtuowklvya.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.yj20258.top/gtekqfzjiw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.ywan-chungtsiang.top/gtonuwpcqu.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.ydjk.org.cn/gtefszzknn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.wangdashe.top/gtvuczgxag.html

[A17] 位运算
来源：http://hz.zhengqikj.top/gtlnwafvxq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xuanzx.com/gtyeqqvfyd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.sufxvd.cn/gtrathknup.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yuanzhike.top/gtkpywvftq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.dianchejie.cn/gtuqnyickv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.smart0.xyz/gtgtxhbcwo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.smart0.xyz/gthcnmpsmj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gotoacloud.top/gtrctaoujb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xziqi.cn/gtvamxhaww.html

[A18] 字符与 ASCII 码互转
来源：http://hz.svipenyu.cn/gtobhykoxf.html

Py:   ord("A"); chr(65)
来源：http://hz.haohaochexian.top/gtuimhrgrw.html

PHP:  ord("A"); chr(65)
来源：http://hz.xingfuxueyuan.xyz/gtartozoul.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.c1oappe.top/gttzwpkcuj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.havefunace.top/gtoidqvpif.html

Java: (int) 'A'; (char) 65
来源：http://hz.daria6918.cn/gtlmzfivtc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.feifeiyinyue.top/gtmdmbhorr.html

Ruby: "A".ord; 65.chr
来源：http://hz.zhaomingkeji.xyz/gtgtbopsys.html

C#:   (int)'A'; (char)65
来源：http://hz.xziqi.cn/gtndwabqyx.html

[A19] 交换两个变量
来源：http://hz.chenjidiqi.icu/gtzzxqhakv.html

Py:   a, b = b, a
来源：http://hz.kuanghao11.cn/gtvwmsxmvi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.cdnleiting.top/gtpmofkobt.html

JS:   [a, b] = [b, a];
来源：http://hz.cdnleiting.top/gttlfeznpw.html

TS:   [a, b] = [b, a];
来源：http://hz.smart0.xyz/gtligfbasz.html

Java: int t = a; a = b; b = t;
来源：http://hz.yuanzhike.top/gtpazvoxvw.html

Go:   a, b = b, a
来源：http://hz.fengsongda.top/gtkxcmatty.html

Ruby: a, b = b, a
来源：http://hz.guowangkeji.top/gtsiuoptak.html

C#:   (a, b) = (b, a);
来源：http://hz.nwbrower.top/gtjvnccqij.html

[A20] 读取标准输入
来源：http://hz.yangfankeji.com/gtugtlpoqc.html

Py:   name = input("请输入：")
来源：http://hz.xylfe.cn/gtapkejfab.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.shangyingyoupin.top/gtrugxjsvj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.jinqigufen.top/gtmddddebd.html

TS:   // Node.js：readline 模块
来源：http://hz.yj20258.top/gtljyumcgp.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.aibaodan.cn/gthbuamror.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.pycfn.com/gtgsiomfck.html

Ruby: gets.chomp
来源：http://hz.sxryk.cn/gtbuamswuf.html

C#:   Console.ReadLine();
来源：http://hz.c1oappe.top/gtlfytwqou.html

[A21] 保留指定小数位输出
来源：http://hz.chenlongwang.top/gtiiwvkzbh.html

Py:   f"{3.14159:.2f}"
来源：http://hz.xingfuxueyuan.xyz/gtwsbryyox.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.andypj.xyz/gtmyvqsuub.html

JS:   (3.14159).toFixed(2)
来源：http://hz.havefunace.top/gtqlznzgzl.html

TS:   (3.14159).toFixed(2)
来源：http://hz.dianchejie.cn/gtvztroqzu.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.ywan-chungtsiang.top/gteopshjfy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.jinyuanbaomall.cn/gtugwomrhf.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.c1oappe.top/gtjljeqkwr.html

C#:   3.14159.ToString("F2")
来源：http://hz.shanyushiyangtech.top/gteybagavo.html

[A22] 获取字符串长度
来源：http://hz.pengpengdd.cyou/gtqzfzvcbx.html

Py:   len(s)
来源：http://hz.jinghuilouyu.cn/gtwdmbvjhp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.52xcode.cn/gtcqparqdd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.havefunace.top/gtnhpbftxl.html

TS:   s.length
来源：http://hz.smart0.xyz/gtxouhmhdk.html

Java: s.length()
来源：http://hz.xuanzx.com/gtahfeipzw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.jqgfzy.top/gtcyxctclt.html

Ruby: s.length
来源：http://hz.wangdashe.top/gtjqdhkbtx.html

C#:   s.Length
来源：http://hz.nwbrower.top/gtotdbsidp.html

[A23] 大小写转换
来源：http://hz.dashuyun.cn/gtlecjcumj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.vqdsnc.cn/gtncslqoqt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.ydzc1.top/gtytkllopg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.cucudq.cn/gtddgyvbye.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.tanke756.top/gtdzfeujmp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhiwuduotai.top/gtwzaolshr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.xuetiantiany.cn/gtfeexvpem.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.xziqi.cn/gtuwgbbluc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.wangdashe.top/gtnpcdcohk.html

[A24] 去除首尾空白
来源：http://hz.snrcjt.cn/gtepnlkxcb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.ywan-chungtsiang.top/gtumgjosvt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.ydjk.org.cn/gtgfkcfrvz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jinqigfzy.top/gtrygapwvb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gotoacloud.top/gtcvhaahqv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.xinyue.icu/gthyszrgmk.html

Go:   strings.TrimSpace(s)
来源：http://hz.nanxinkj.top/gtrsrvllwu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.vqdsnc.cn/gtbqptsxls.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.kuanghao11.cn/gtwooekpgb.html

[A25] 字符串比较
来源：http://hz.yueranfly.top/gtcbvvobwk.html

Py:   s1 == s2; s1 != s2
来源：http://hz.0kj1m.cn/gtjnoimrso.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.shuidangran.top/gtsaywqcxu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.chenjidiqi.icu/gtrsoeayqp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hammf.cn/gtwhkpyxmx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.tianlin.xyz/gtbzscnmcz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.pengpengdd.cyou/gtfbvbyysj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.pycfn.com/gtebjrzlat.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.dashuyun.cn/gtsqyuerti.html

[A26] 类型转换总览
来源：http://hz.jyoumei.cn/gthfzrgmrx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.hammf.cn/gtbaqznfkq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yvedp.cn/gtnksqkkcy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.ivvv.top/gtflwsdcnq.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yonumen.top/gtmxsbwwyr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.cashguo.top/gtarlhlhij.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.aibaodan.cn/gtmgcvdtzb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.zhijiandao.cn/gthoyfoxfi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.dianchejie.cn/gtzixbcljo.html

================================================================================
来源：http://hz.xuanzx.com/gtaqchdakb.html

B. 流程控制
来源：http://hz.cdnleiting.top/gtgyntvatj.html

================================================================================
来源：http://hz.kuanghao11.cn/gtdvntxvlx.html

[B01] 条件判断 if / else
来源：http://hz.zhaomingkeji.xyz/gtkdnupoku.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.shanyushiyangtech.top/gtorbicjll.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.daxiang520.top/gtnileihei.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shzxlz.cn/gttqvdvmip.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hnqzz.top/gtgwusdlvb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.52xcode.cn/gtwunbqaft.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.zhaomingkeji.xyz/gtvilxvtjs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.ydjk.org.cn/gtpdgndssp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jinqigufen.top/gtwsjovokw.html

[B02] 多分支 else if / elif
来源：http://hz.aibaodan.cn/gtjtseksfb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhengqikj.top/gtnnptxoub.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.haohaochexian.top/gttguwlbdp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jlsjyb.cn/gtzcmsupqo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pycfn.com/gtkwyvigki.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinqigfzy.top/gtttmqbcmx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jyoumei.cn/gtoscffyid.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.sweek.top/gtxzlamhlq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jianghu66.top/gtibvedbuj.html

[B03] switch / match / case
来源：http://hz.c1oappe.top/gtemnyjaar.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.guowangkeji.top/gtzhmhkipl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.redwolf501.top/gtcrsaznau.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.aibaodan.cn/gtdjxztvwy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hywenlv.cn/gtjjijqcnx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.cqqwz.cn/gtmziwentq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhiwuduotai.top/gtwzpfawwp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.aibaodan.cn/gtpxkkspfv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.zhongyouzk.top/gttplicnke.html

[B04] for 计数循环
来源：http://hz.jinqigfzy.top/gtzgdmhnhz.html

Py:   for i in range(10): print(i)
来源：http://hz.snrcjt.cn/gtajenbowg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zhijiandao.cn/gtqecanayy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yj20258888.top/gtgwzubefs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.feifeiyinyue.top/gtwsqvhlau.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.xuanzx.com/gtodzouunp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jqgufenzy.top/gthowwotjd.html

Ruby: 10.times { |i| puts i }
来源：http://hz.yj20258888.top/gtetuxtwaf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jiagoushi.top/gtdlmubqrd.html

[B05] 遍历数组 / 列表
来源：http://hz.sxryk.cn/gtqlkyucyb.html

Py:   for item in arr: print(item)
来源：http://hz.birdmap.top/gtwxvuqfwh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.zhijiandao.cn/gtvaidcjgh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.tianlin.xyz/gtdhhagped.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhixingplan.top/gtmluosiju.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.andypj.xyz/gterflpcvy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.guannengcc.top/gtescpehwi.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ehwqpu.com/gtrrppjchn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.nwbrower.top/gtchvbwepf.html

[B06] 遍历字典 / 对象
来源：http://hz.wangshuangyany.cn/gtmzdgwysi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhixingplan.top/gtcmnbswax.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.guowangkeji.top/gtmfqnmuln.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xylfe.cn/gtywnuocgn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhaomingkeji.xyz/gtbzkcpbze.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.cdnleiting.top/gtxkpkfdsl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hongshengwenyu.top/gttxugsxqq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhiwuduotai.top/gtouiczdzk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.xuanzx.com/gtyibcfrrz.html

[B07] while 循环
来源：http://hz.zhijiandao.cn/gtkdegqaqj.html

Py:   while i < 10: i += 1
来源：http://hz.hywenlv.cn/gtntrbcuca.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xinyue.icu/gtkeomtzfh.html

JS:   while (i < 10) { i++; }
来源：http://hz.9152youxi.cn/gtdusdesoj.html

TS:   while (i < 10) { i++; }
来源：http://hz.jinghuilouyu.cn/gtpwofrwge.html

Java: while (i < 10) { i++; }
来源：http://hz.cheryme.top/gtbhvwlfev.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.chenlongwang.top/gtpeqjcmwo.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ywan-chungtsiang.top/gtukrotyxh.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gttichasym.html

[B08] do-while（至少执行一次）
来源：http://hz.jinqigufen.top/gtpgrqkbjl.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.birdmap.top/gtfrzdtvlu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hongshengwenyu.top/gttkwhkerf.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtxldrdfqq.html

TS:   do { i++; } while (i < 10);
来源：http://hz.tianlin.xyz/gtfynexptj.html

Java: do { i++; } while (i < 10);
来源：http://hz.kuanghao11.cn/gtvxdwpxvo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.daxiang520.top/gtiyhjimlb.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ppjwa.cn/gtiycqurja.html

C#:   do { i++; } while (i < 10);
来源：http://hz.smart0.xyz/gtjpuegmky.html

[B09] break 与 continue
来源：http://hz.cucudq.cn/gtrxugjklt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jqgfzy.top/gtmfihwjns.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shzxlz.cn/gtgwlyxcgj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cheryme.top/gtfawarkwq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hysaishi.cn/gtgzmvhcmn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cqqwz.cn/gtzvcjuvho.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jyoumei.cn/gtdzilltuo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.wangshuangyany.cn/gtycrlrgfz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuxming.cn/gtietrudsn.html

[B10] 遍历同时拿索引
来源：http://hz.jiagoushi.top/gtokulytgh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.meibo888.top/gtuvwqqays.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cucudq.cn/gtygqzhhuw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xziqi.cn/gtuneombmw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hammf.cn/gtdxsyaimm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cheryme.top/gtvcmfmzgt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.9152youxi.cn/gtcggcvcsh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zdqjudy.top/gtniqkfadc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.cdnleiting.top/gthsjazwim.html

[B11] 生成数字序列 / 区间
来源：http://hz.gzhubu.top/gtqgklsxog.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhaomingkeji.xyz/gtdhujhtyy.html

PHP:  range(0, 10, 2);
来源：http://hz.dashuyun.cn/gtmnvrypkn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.pycfn.com/gtngrijkru.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.0kj1m.cn/gtfnhwysmf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xuetiantiany.cn/gtgxzvwgyr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinghuilouyu.cn/gtrwucrjyk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.aibaodan.cn/gtghofitft.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.fzhhl.top/gtmdcngfnq.html

[B12] 跳出多层循环
来源：http://hz.jqgufenzy.top/gtwbppuqsi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.havefunace.top/gtqorgdlyc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhongyouzk.top/gtohwbvkbn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigufen.top/gtejvumkqj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.quarkkingdee.top/gtoscofrqp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xziqi.cn/gthbjpewou.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.chenlongwang.top/gtqbaqxwgm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.dashuyun.cn/gtbwnjmqul.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xingfuxueyuan.xyz/gtrbijfxoa.html

[B13] 判断是否为数字
来源：http://hz.hfpthk.cn/gtodxwqffp.html

Py:   isinstance(x, (int, float))
来源：http://hz.yj202588.top/gtweubqavx.html

PHP:  is_numeric($x)
来源：http://hz.haohaochexian.top/gtdgbrmwzc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daria6918.cn/gtvijibqte.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.bjfxy.top/gtaxrydqhz.html

Java: x instanceof Number
来源：http://hz.zhengqikj.top/gtnfngzahi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.shangyingyoupin.top/gtnsbiirgd.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ehwqpu.com/gtgkteelik.html

C#:   x is int or double or decimal
来源：http://hz.xuanzx.com/gtfkvhtnjz.html

[B14] 判断值是否在集合内
来源：http://hz.yvedp.cn/gtkvrjjtyf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hnqzz.top/gteujrutsl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.sufxvd.cn/gtmooxvgdn.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yueranfly.top/gtjbneltxq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.c1oappe.top/gtbrmrutst.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.xylfe.cn/gtokjradyv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhijiandao.cn/gtgsusuhxf.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.havefunace.top/gtomfgsagn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.fengsongda.top/gtejqzddtu.html

[B15] 布尔运算与取反
来源：http://hz.sxryk.cn/gtbpuzyxob.html

Py:   a and b or not c
来源：http://hz.316326.xyz/gthufiiaif.html

PHP:  $a && $b || !$c
来源：http://hz.ppjwa.cn/gtozzvmdfe.html

JS:   a && b || !c
来源：http://hz.jqgfzy.top/gtwkukdhua.html

TS:   a && b || !c
来源：http://hz.tian-w.cn/gtlfgaeftl.html

Java: a && b || !c
来源：http://hz.gotoacloud.top/gtyxebfeqs.html

Go:   a && b || !c
来源：http://hz.yonumen.top/gtcoyhcbqn.html

Ruby: a && b || !c
来源：http://hz.yongpay.top/gtumjvypnu.html

C#:   a && b || !c
来源：http://hz.xuanzx.com/gtmtpfztsz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shuidangran.top/gtbvzjwoxh.html

Py:   if not data: return
来源：http://hz.cashguo.top/gtifknhjxn.html

PHP:  if (!$data) { return; }
来源：http://hz.ehwqpu.com/gtjcrirzor.html

JS:   if (!data) return;
来源：http://hz.yuxming.cn/gtgtyadjkf.html

TS:   if (!data) return;
来源：http://hz.svipenyu.cn/gtrdzjsnde.html

Java: if (data == null) return;
来源：http://hz.dianchejie.cn/gtwsqarglv.html

Go:   if data == nil { return }
来源：http://hz.svipenyu.cn/gtxeotqzbw.html

Ruby: return if data.nil?
来源：http://hz.jiagoushi.top/gtqknjxftg.html

C#:   if (data == null) return;
来源：http://hz.zhiwuduotai.top/gtmukhixpr.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gthfpoulxa.html

C. 函数与作用域
来源：http://hz.jinyuanbaomall.cn/gtzntyphjs.html

================================================================================
来源：http://hz.hfpthk.cn/gtjhnadqvl.html

[C01] 定义函数
来源：http://hz.birdmap.top/gtcvwkyuyv.html

Py:   def add(a, b): return a + b
来源：http://hz.zhongyouzk.top/gtxuacyico.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xinyue.icu/gtucgmskrt.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtdswbuxif.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.bjfxy.top/gtgindptlx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtiqnxcqch.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.chenlongwang.top/gtzgvpezwh.html

Ruby: def add(a, b); a + b; end
来源：http://hz.nanxinkj.top/gtvulaazrc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gttpqdrozs.html

[C02] 默认参数
来源：http://hz.xuanzx.com/gtkrfpjctx.html

Py:   def greet(name="World"): return name
来源：http://hz.aizwys.cn/gtjeawbdmf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.redwolf501.top/gtbkmyaqsf.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nanxinkj.top/gtmjauavpn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yj20258.top/gtzzozmemi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinghuilouyu.cn/gtqhqkcrch.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gaohongyu789.top/gtoloaodbf.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhengqikj.top/gteiewpyyw.html


<!-- 参考信息 -->