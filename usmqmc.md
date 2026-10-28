代发 wailian999

[A14] 注释写法
来源：http://hz.daxiang520.top/gtkaoqetpy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.yj20258.top/gtnmknlrml.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.hongshengwenyu.top/gtpjlkkgfn.html

JS:   // 单行；/* 多行 */
来源：http://hz.nanxinkj.top/gtbnwwpcrx.html

TS:   // 单行；/* 多行 */
来源：http://hz.jinqigfzy.top/gtwyegprgz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.hnqzz.top/gtowxkkokl.html

Go:   // 单行；/* 多行 */
来源：http://hz.cheryme.top/gtfcgfpzqu.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.hnqzz.top/gtcknblvat.html

C#:   // 单行；/* 多行 */
来源：http://hz.hnqzz.top/gteilfnxsj.html

[A15] 空值判断与默认值
来源：http://hz.ywan-chungtsiang.top/gtipghosdw.html

Py:   value = data or "默认值"
来源：http://hz.yj20258.top/gtymbjmdbt.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.iojbl.cn/gtftpurxfo.html

JS:   const value = data ?? "默认值";
来源：http://hz.xziqi.cn/gthuuvfiqt.html

TS:   const value = data ?? "默认值";
来源：http://hz.chenlongwang.top/gtcwiloium.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.316326.xyz/gtigfgqhch.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.zhoulong.xyz/gtwchtajiz.html

Ruby: value = data || "默认值"
来源：http://hz.jiagoushi.top/gtzxvpecgw.html

C#:   var value = data ?? "默认值";
来源：http://hz.guowangkeji.top/gtrjgplbta.html

[A16] 真假值判断规则
来源：http://hz.0kj1m.cn/gtqkjwdtwb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.ivvv.top/gtxixjwrik.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.dashuyun.cn/gtktowxyde.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.chenjidiqi.icu/gtawhwecsa.html

TS:   if (!x) {}
来源：http://hz.chenjidiqi.icu/gtlvuhaauj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.316326.xyz/gtsflekaxs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.zhaomingkeji.xyz/gtqwxezmpb.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.jinyuanbaomall.cn/gtoymaekcz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.snrcjt.cn/gtynamycne.html

[A17] 位运算
来源：http://hz.meibo888.top/gtsclzthfl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydjk.org.cn/gtnehjkxcu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.daxiang520.top/gtzcalsvuc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hongshengwenyu.top/gtnxjpggom.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.xuetiantiany.cn/gtjyzyddod.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhaomingkeji.xyz/gttrkogwei.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jyoumei.cn/gtyunwubdx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hnxiangtu.top/gtjvrcgjqf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tanke756.top/gtmoypwxve.html

[A18] 字符与 ASCII 码互转
来源：http://hz.xingfuxueyuan.xyz/gtfegdkoxl.html

Py:   ord("A"); chr(65)
来源：http://hz.hongshengwenyu.top/gtpqwhcvyk.html

PHP:  ord("A"); chr(65)
来源：http://hz.cucudq.cn/gtjdssdtkc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xuetiantiany.cn/gtvgaabuyh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.snrcjt.cn/gtdrqzqese.html

Java: (int) 'A'; (char) 65
来源：http://hz.hnqzz.top/gtftnqiart.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.zycfv.cn/gtjfqpwurb.html

Ruby: "A".ord; 65.chr
来源：http://hz.zhengqikj.top/gtkmaqjkcp.html

C#:   (int)'A'; (char)65
来源：http://hz.ybcxt.top/gttoaeilan.html

[A19] 交换两个变量
来源：http://hz.smart0.xyz/gtcxigqsdy.html

Py:   a, b = b, a
来源：http://hz.0kj1m.cn/gtegdnvkft.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.kuanghao11.cn/gtcjmukbvt.html

JS:   [a, b] = [b, a];
来源：http://hz.wangshuangyany.cn/gtstppsodq.html

TS:   [a, b] = [b, a];
来源：http://hz.yuanzhike.top/gtrdxlnkth.html

Java: int t = a; a = b; b = t;
来源：http://hz.sufxvd.cn/gtrldhlumn.html

Go:   a, b = b, a
来源：http://hz.xylfe.cn/gtvbsixzsb.html

Ruby: a, b = b, a
来源：http://hz.nanxuanxn.top/gtmjbaevbu.html

C#:   (a, b) = (b, a);
来源：http://hz.cheryme.top/gtujxpngpg.html

[A20] 读取标准输入
来源：http://hz.xinyue.icu/gthdzcmkid.html

Py:   name = input("请输入：")
来源：http://hz.guannengcc.top/gtgakaxftz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.9152youxi.cn/gtlbbjpydm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.snrcjt.cn/gtnbsiosoc.html

TS:   // Node.js：readline 模块
来源：http://hz.xuetiantiany.cn/gtbkthjpcv.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.ehwqpu.com/gtotfomxsq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.gogol.net.cn/gtnkayhoxf.html

Ruby: gets.chomp
来源：http://hz.316326.xyz/gtpsshwuto.html

C#:   Console.ReadLine();
来源：http://hz.sweek.top/gtxeyfhnhb.html

[A21] 保留指定小数位输出
来源：http://hz.cheryme.top/gtlltdoode.html

Py:   f"{3.14159:.2f}"
来源：http://hz.vqdsnc.cn/gteyvczbmg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.daxiang520.top/gtyikabwki.html

JS:   (3.14159).toFixed(2)
来源：http://hz.shuidangran.top/gtdrltmbgc.html

TS:   (3.14159).toFixed(2)
来源：http://hz.jqgufenzy.top/gtbxeqqbpd.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.hammf.cn/gtdxmtphmr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.tianlin.xyz/gtofysvphn.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.hnxiangtu.top/gtqxymrtze.html

C#:   3.14159.ToString("F2")
来源：http://hz.yonumen.top/gtcakubfos.html

[A22] 获取字符串长度
来源：http://hz.aibaodan.cn/gteswmavzi.html

Py:   len(s)
来源：http://hz.ivvv.top/gtcyliujwz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.andypj.xyz/gtcbkxpfqe.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.52xcode.cn/gtowhduiyn.html

TS:   s.length
来源：http://hz.gzhubu.top/gtsnoerhep.html

Java: s.length()
来源：http://hz.daxiang520.top/gtpaqfusgl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.zhiwuduotai.top/gtxqrmzmor.html

Ruby: s.length
来源：http://hz.smart0.xyz/gtqjnyxshp.html

C#:   s.Length
来源：http://hz.0kj1m.cn/gtjqmuyyjq.html

[A23] 大小写转换
来源：http://hz.dianchejie.cn/gtmlprmstl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.tianlin.xyz/gtpuzefvmf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.cheryme.top/gtrpuixszc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.snrcjt.cn/gtovgefxnx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hnqzz.top/gtlwiulqzh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.ywan-chungtsiang.top/gtypqarmay.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.andypj.xyz/gtsxulfheq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.sxryk.cn/gtejxpgzyy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yueranfly.top/gthjmdgqvi.html

[A24] 去除首尾空白
来源：http://hz.zhiwuduotai.top/gtypupfcir.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.cqqwz.cn/gtycpybkaw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.0kj1m.cn/gtzvgnkpzj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.pycfn.com/gtskkjluzt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yj20258.top/gttajtbcmh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.vqdsnc.cn/gtabnqgtjx.html

Go:   strings.TrimSpace(s)
来源：http://hz.meibo888.top/gtabkgibjy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.hnxiangtu.top/gtvricpufe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.quarkkingdee.top/gtdfmhvtpu.html

[A25] 字符串比较
来源：http://hz.jinqigfzy.top/gtwsbcbuac.html

Py:   s1 == s2; s1 != s2
来源：http://hz.guannengcc.top/gthfdmhyfu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.316326.xyz/gtzihhyopk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jqgufenzy.top/gtgkndqcuq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.quarkkingdee.top/gtfdzvgcwe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.tanke756.top/gtchvywkwg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.gotoacloud.top/gtagpdunla.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.xylfe.cn/gtjtoogkgb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.xuetiantiany.cn/gtlyiublrh.html

[A26] 类型转换总览
来源：http://hz.jlsjyb.cn/gtjyovnpmv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.pengpengdd.cyou/gtmfkepssh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.hnxiangtu.top/gtlgwiwfmt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yvedp.cn/gtvkgpgofc.html

TS:   Number() String() Boolean() x as number
来源：http://hz.shanyushiyangkeji.top/gtnvxkillq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.hnqzz.top/gtxxpurege.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.wangshuangyany.cn/gtrpzuhdew.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.sysykeji.top/gtxxlkchaz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.sweek.top/gteluqzyzh.html

================================================================================
来源：http://hz.gogol.net.cn/gtmelpagzf.html

B. 流程控制
来源：http://hz.bjfxy.top/gtbabjeshd.html

================================================================================
来源：http://hz.jlsjyb.cn/gtvszrtinc.html

[B01] 条件判断 if / else
来源：http://hz.pengpengdd.cyou/gtczisryqc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.cheryme.top/gtefsceimx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.xylfe.cn/gtpwomgeyz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jqgufenzy.top/gtawhlnaxd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jinqigufen.top/gtnvtrcfnb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.jyoumei.cn/gtwotrigep.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yuanzhike.top/gtkyoqshuy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yangfankeji.com/gteffcyzdc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.ybcxt.top/gtdpeidpas.html

[B02] 多分支 else if / elif
来源：http://hz.sxryk.cn/gtnzoqjbev.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zycfv.cn/gtvwybfeqe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.c1oappe.top/gtxoprooqh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shuidangran.top/gtnyttcqce.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shanyushiyangtech.top/gtwbrkfaoh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xylfe.cn/gtdzvcjqyw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.ppjwa.cn/gtlqcqvava.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jyoumei.cn/gtlgblwvvr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenlongwang.top/gtovbgywnl.html

[B03] switch / match / case
来源：http://hz.9152youxi.cn/gtnfjcyzco.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.gogol.net.cn/gtpcekbzcc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yueranfly.top/gtccoqjins.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gotoacloud.top/gtlklybrao.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.sufxvd.cn/gttujlfkcl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.feifeiyinyue.top/gtnhwzgcjt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.feifeiyinyue.top/gtvmnbdzcl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.316326.xyz/gtukenphvu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.jinyuanbaomall.cn/gtyyojgrro.html

[B04] for 计数循环
来源：http://hz.daria6918.cn/gtaoiotvam.html

Py:   for i in range(10): print(i)
来源：http://hz.cqqwz.cn/gtmvcwdneb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.chenzaomai.com/gtrydbvaig.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.wangdashe.top/gtqatvvojo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gzhubu.top/gtmwjbytyh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhoulong.xyz/gtxmkpeytd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.fengsongda.top/gtrwzqycsy.html

Ruby: 10.times { |i| puts i }
来源：http://hz.aizwys.cn/gtqkgodevh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.kuanghao11.cn/gtwrtonapn.html

[B05] 遍历数组 / 列表
来源：http://hz.jinyuanbaomall.cn/gtsieeeopx.html

Py:   for item in arr: print(item)
来源：http://hz.tanke756.top/gtkxzwfqpy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.cheryme.top/gthzibbalm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.52xcode.cn/gtyigjgvpb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.quarkkingdee.top/gtehkcgcor.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.xuanzx.com/gtrwbttbes.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.havefunace.top/gtiamvwxjw.html

Ruby: arr.each { |item| puts item }
来源：http://hz.xinyue.icu/gtwkfystow.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.shanyushiyangtech.top/gtdeinoxvm.html

[B06] 遍历字典 / 对象
来源：http://hz.ppjwa.cn/gttmwzjomz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.redwolf501.top/gtfamgenkv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hongshengwenyu.top/gtmwtbrlsr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ydjk.org.cn/gtjxijcbqc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.tianlin.xyz/gtwhxjhcfh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gzhubu.top/gthswjcxjt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xuetiantiany.cn/gtpfnlojns.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.cqqwz.cn/gtddadeaco.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.zycfv.cn/gtnplghxso.html

[B07] while 循环
来源：http://hz.svipenyu.cn/gthjrnrttq.html

Py:   while i < 10: i += 1
来源：http://hz.zhiwuduotai.top/gtbdduxyuu.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.ehwqpu.com/gtwanbiwop.html

JS:   while (i < 10) { i++; }
来源：http://hz.havefunace.top/gthuipvuer.html

TS:   while (i < 10) { i++; }
来源：http://hz.jinyuanbaomall.cn/gtqmtmjmzl.html

Java: while (i < 10) { i++; }
来源：http://hz.shanyushiyangkeji.top/gteiflcvkk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.nanxinkj.top/gtdoiiykfr.html

Ruby: while i < 10; i += 1; end
来源：http://hz.chenlongwang.top/gtzfhgwfdn.html

C#:   while (i < 10) { i++; }
来源：http://hz.jinqigufen.top/gtiilpyrej.html

[B08] do-while（至少执行一次）
来源：http://hz.bjfxy.top/gtuqwgceih.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cdnleiting.top/gtuhvpldvx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.pycfn.com/gtqyzwkigp.html

JS:   do { i++; } while (i < 10);
来源：http://hz.bjfxy.top/gtujtejcgy.html

TS:   do { i++; } while (i < 10);
来源：http://hz.kuanghao11.cn/gthzsbdddw.html

Java: do { i++; } while (i < 10);
来源：http://hz.hysaishi.cn/gtqfwghpfy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.chenjidiqi.icu/gtpxkszsli.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.cheryme.top/gtjaadnbhp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.0kj1m.cn/gtianvnnck.html

[B09] break 与 continue
来源：http://hz.chenlongwang.top/gtcykmxphs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.aizwys.cn/gtuocmnrma.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jyoumei.cn/gtwucobcuo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhoulong.xyz/gtswyeqlfw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhixingplan.top/gtjwgydgpx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinyuanbaomall.cn/gtaqdwsghz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.aibaodan.cn/gtywmzhqyv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hnxiangtu.top/gtchfgxwis.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yanxiufei.cn/gtxhhjxpum.html

[B10] 遍历同时拿索引
来源：http://hz.gotoacloud.top/gtotlrjdrw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.svipenyu.cn/gtyrmpeobo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.feifeiyinyue.top/gttopifaxj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zdqjudy.top/gthccvrggs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.sufxvd.cn/gttxwlmcab.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.smart0.xyz/gtuualcuqt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yj20258888.top/gtkxlcxkhr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gotoacloud.top/gtrdqpadzd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yj202588.top/gthtymnvoc.html

[B11] 生成数字序列 / 区间
来源：http://hz.316326.xyz/gtwdnjctqv.html

Py:   list(range(0, 10, 2))
来源：http://hz.yj20258.top/gtchwagqrw.html

PHP:  range(0, 10, 2);
来源：http://hz.sufxvd.cn/gtrodveeps.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yuxming.cn/gtzgrxojnq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.0kj1m.cn/gtpvhjbwnt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinqigfzy.top/gtlstvfwfw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.andypj.xyz/gtnhjncbjp.html

Ruby: (0...10).step(2).to_a
来源：http://hz.fzhhl.top/gtpegscplp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.kuanghao11.cn/gtszfqsrxg.html

[B12] 跳出多层循环
来源：http://hz.shuidangran.top/gtvodhqtxu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.chenlongwang.top/gtiwqhckrz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.sxryk.cn/gtrgbadunt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.svipenyu.cn/gtiftinthh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.52xcode.cn/gtgqeivzmt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.nwbrower.top/gtaxiemvok.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.gotoacloud.top/gtkaptyswk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.pycfn.com/gtnkjqbdvt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xylfe.cn/gtwpqareqz.html

[B13] 判断是否为数字
来源：http://hz.gogol.net.cn/gtykdjwytg.html

Py:   isinstance(x, (int, float))
来源：http://hz.hammf.cn/gtpjlwmdoz.html

PHP:  is_numeric($x)
来源：http://hz.sysykeji.top/gtiyveberl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.snrcjt.cn/gtbvyfsdmd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgfzy.top/gtklfiwxac.html

Java: x instanceof Number
来源：http://hz.jinghuilouyu.cn/gtlduuhntb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.0kj1m.cn/gtgyxabxss.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xylfe.cn/gtunnzamie.html

C#:   x is int or double or decimal
来源：http://hz.guowangkeji.top/gtmtnddayh.html

[B14] 判断值是否在集合内
来源：http://hz.9152youxi.cn/gtqwaqmhik.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jinyuanbaomall.cn/gtgbdekntb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.fengsongda.top/gterantolc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangkeji.top/gtqygrtubl.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.shuidangran.top/gtphsaklgx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.guowangkeji.top/gtndeuhiww.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yangfankeji.com/gtujscbffq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hfpthk.cn/gtayctvcsr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.daxiang520.top/gtqxijpzga.html

[B15] 布尔运算与取反
来源：http://hz.yanxiufei.cn/gtzskmsdjh.html

Py:   a and b or not c
来源：http://hz.redwolf501.top/gtkgkpdbax.html

PHP:  $a && $b || !$c
来源：http://hz.fzhhl.top/gtfcjmwchb.html

JS:   a && b || !c
来源：http://hz.yvedp.cn/gtqetoebdt.html

TS:   a && b || !c
来源：http://hz.daxiang520.top/gtpzovompi.html

Java: a && b || !c
来源：http://hz.jinghuilouyu.cn/gttrizipcp.html

Go:   a && b || !c
来源：http://hz.zhoulong.xyz/gttflevsnf.html

Ruby: a && b || !c
来源：http://hz.mhx1999.top/gtjqospirt.html

C#:   a && b || !c
来源：http://hz.ehwqpu.com/gtugygistf.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.andypj.xyz/gtrgjxzela.html

Py:   if not data: return
来源：http://hz.tian-w.cn/gtvbqazqsp.html

PHP:  if (!$data) { return; }
来源：http://hz.gotoacloud.top/gteawdnqgu.html

JS:   if (!data) return;
来源：http://hz.xuanzx.com/gtkeszoids.html

TS:   if (!data) return;
来源：http://hz.jinghuilouyu.cn/gtvvwqflrq.html

Java: if (data == null) return;
来源：http://hz.zhiwuduotai.top/gtoauquivo.html

Go:   if data == nil { return }
来源：http://hz.xziqi.cn/gtgfepsytv.html

Ruby: return if data.nil?
来源：http://hz.chenjidiqi.icu/gtbzdsqsfv.html

C#:   if (data == null) return;
来源：http://hz.zdqjudy.top/gttrmnezvg.html

================================================================================
来源：http://hz.gaohongyu789.top/gtjtvidhob.html

C. 函数与作用域
来源：http://hz.cdnleiting.top/gtyjkgqkqm.html

================================================================================
来源：http://hz.dashuyun.cn/gtshzxssdx.html

[C01] 定义函数
来源：http://hz.chenjidiqi.icu/gtzumfxuuu.html

Py:   def add(a, b): return a + b
来源：http://hz.ydzc1.top/gtbkiwamui.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.vqdsnc.cn/gtpwenqiib.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tianlin.xyz/gtkfouvthk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tanke756.top/gtmebtftln.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtjvsmgdey.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.aibaodan.cn/gtimnynwez.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gotoacloud.top/gtrzwqoubb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gotoacloud.top/gtnucunero.html

[C02] 默认参数
来源：http://hz.iojbl.cn/gtgohmwsva.html

Py:   def greet(name="World"): return name
来源：http://hz.snrcjt.cn/gticzsrhhr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.gaohongyu789.top/gtuotyuuof.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xziqi.cn/gtyvmjjkvl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.meibo888.top/gtmcnrvhwr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.redwolf501.top/gtasvjrerm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yangfankeji.com/gtxxjwzyzt.html

Ruby: def greet(name = "World") = name
来源：http://hz.smart0.xyz/gtwiozuctu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.vqdsnc.cn/gtpfborvtx.html

[C03] 可变参数
来源：http://hz.wangdashe.top/gttxbgfvnf.html

Py:   def total(*args): return sum(args)
来源：http://hz.snrcjt.cn/gtzntityvv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.tianlin.xyz/gtnraqhiny.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.birdmap.top/gtdbxvtipu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.vqdsnc.cn/gtarmkgtqk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shzxlz.cn/gtapizenim.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shanyushiyangkeji.top/gtkntmbzro.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hnqzz.top/gtbmyznaev.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.haohaochexian.top/gtadodqczl.html

[C04] 命名参数 / 关键字参数
来源：http://hz.52xcode.cn/gtyczysxwv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.fzhhl.top/gtechrwudh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.pycfn.com/gtadwufwea.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cqqwz.cn/gtkqiubytj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jianghu66.top/gtakesixrx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jqgufenzy.top/gteeluzgwe.html


<!-- 参考信息 -->