代发 wailian999

[A14] 注释写法
来源：http://hz.xylfe.cn/gtpdlvwbht.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.jiagoushi.top/gtaburxkkk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.mhx1999.top/gtcnymtnpe.html

JS:   // 单行；/* 多行 */
来源：http://hz.ehwqpu.com/gtyknaxsvx.html

TS:   // 单行；/* 多行 */
来源：http://hz.jlsjyb.cn/gtorslhebk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.feifeiyinyue.top/gtznuaxyzf.html

Go:   // 单行；/* 多行 */
来源：http://hz.nanxinkj.top/gtomixpxvw.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.tanke756.top/gtyfwjnpyq.html

C#:   // 单行；/* 多行 */
来源：http://hz.zhoulong.xyz/gtbeludhpt.html

[A15] 空值判断与默认值
来源：http://hz.c1oappe.top/gtqhbompsm.html

Py:   value = data or "默认值"
来源：http://hz.cashguo.top/gttmzvavng.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.jyoumei.cn/gtmyoclrfc.html

JS:   const value = data ?? "默认值";
来源：http://hz.iojbl.cn/gtamygllch.html

TS:   const value = data ?? "默认值";
来源：http://hz.meibo888.top/gtyhrcostz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.shangyingyoupin.top/gtvmcgyejz.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.jinqigfzy.top/gtheiwiyta.html

Ruby: value = data || "默认值"
来源：http://hz.c1oappe.top/gtajrsvaxe.html

C#:   var value = data ?? "默认值";
来源：http://hz.hfpthk.cn/gtapqhljap.html

[A16] 真假值判断规则
来源：http://hz.hongshengwenyu.top/gtaczlwhfg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.guannengcc.top/gtqozyyylc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.gzhubu.top/gtqwpzhkwy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.quarkkingdee.top/gtergrpkbg.html

TS:   if (!x) {}
来源：http://hz.bjfxy.top/gtebosgzll.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.andypj.xyz/gtzmyoould.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.cheryme.top/gtehhveifh.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.tianlin.xyz/gtcasxrqsh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.wangshuangyany.cn/gtjkecwtbd.html

[A17] 位运算
来源：http://hz.316326.xyz/gttcxxcjmf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yanxiufei.cn/gtknuwybvv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.c1oappe.top/gtmmfhzkpy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.dianchejie.cn/gtimcsukku.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.shangyingyoupin.top/gtntxitekk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xylfe.cn/gtejdiypog.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.sysykeji.top/gtxkhmohzh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fzhhl.top/gteyimdefo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shzxlz.cn/gtuunwgkpr.html

[A18] 字符与 ASCII 码互转
来源：http://hz.yanxiufei.cn/gtryfcfywf.html

Py:   ord("A"); chr(65)
来源：http://hz.zhixingplan.top/gtgqieuyzc.html

PHP:  ord("A"); chr(65)
来源：http://hz.birdmap.top/gtavruorir.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.gaohongyu789.top/gtdvggcdgb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jinqigfzy.top/gtewhbmrll.html

Java: (int) 'A'; (char) 65
来源：http://hz.yj202588.top/gtjiesxluj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.chenjidiqi.icu/gtbxwjreux.html

Ruby: "A".ord; 65.chr
来源：http://hz.zhoulong.xyz/gtxwilnpyi.html

C#:   (int)'A'; (char)65
来源：http://hz.tian-w.cn/gtidecymkq.html

[A19] 交换两个变量
来源：http://hz.yanxiufei.cn/gtipwcgove.html

Py:   a, b = b, a
来源：http://hz.xingfuxueyuan.xyz/gtjbcrvbqw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.sufxvd.cn/gtzlpwvekv.html

JS:   [a, b] = [b, a];
来源：http://hz.aibaodan.cn/gtjdintuxp.html

TS:   [a, b] = [b, a];
来源：http://hz.andypj.xyz/gtjmwweihw.html

Java: int t = a; a = b; b = t;
来源：http://hz.aibaodan.cn/gtrmuwkgyu.html

Go:   a, b = b, a
来源：http://hz.yj20258888.top/gtzgioytca.html

Ruby: a, b = b, a
来源：http://hz.zhengqikj.top/gtdxdfdlpi.html

C#:   (a, b) = (b, a);
来源：http://hz.cdnleiting.top/gtsvyrxhiz.html

[A20] 读取标准输入
来源：http://hz.shzxlz.cn/gtgrdcmfor.html

Py:   name = input("请输入：")
来源：http://hz.wangdashe.top/gtjkjlxbho.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.tianlin.xyz/gtemwsduvx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.jinqigfzy.top/gtfjkkefqs.html

TS:   // Node.js：readline 模块
来源：http://hz.svipenyu.cn/gtkznyfxii.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.quarkkingdee.top/gtczgwywhz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.dianchejie.cn/gtygatwqjb.html

Ruby: gets.chomp
来源：http://hz.yj20258.top/gtxznedpmr.html

C#:   Console.ReadLine();
来源：http://hz.dianchejie.cn/gtvkijbxsj.html

[A21] 保留指定小数位输出
来源：http://hz.yj20258.top/gtxntnzorp.html

Py:   f"{3.14159:.2f}"
来源：http://hz.daxiang520.top/gtncgzbvym.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.svipenyu.cn/gtprrcbobs.html

JS:   (3.14159).toFixed(2)
来源：http://hz.zycfv.cn/gtbmfnmaxn.html

TS:   (3.14159).toFixed(2)
来源：http://hz.yanxiufei.cn/gtcmviglyt.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.xuetiantiany.cn/gtsfrisrul.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.hnqzz.top/gteixmzqtq.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.birdmap.top/gtzxkfdjlg.html

C#:   3.14159.ToString("F2")
来源：http://hz.haohaochexian.top/gtbzryuagu.html

[A22] 获取字符串长度
来源：http://hz.jiagoushi.top/gtdoscuebc.html

Py:   len(s)
来源：http://hz.yj20258888.top/gtvjepiccm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.ywan-chungtsiang.top/gtatxgyuvg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.birdmap.top/gtnbxlosla.html

TS:   s.length
来源：http://hz.gaohongyu789.top/gtilyvchxh.html

Java: s.length()
来源：http://hz.316326.xyz/gtrsgipkzp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.xuanzx.com/gtqpzyvstc.html

Ruby: s.length
来源：http://hz.guowangkeji.top/gtvcmlcaoc.html

C#:   s.Length
来源：http://hz.fzhhl.top/gtpjpmurwf.html

[A23] 大小写转换
来源：http://hz.sufxvd.cn/gturwhtimu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.jinghuilouyu.cn/gtfzjoiduc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.cheryme.top/gtnvmpjnkn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jinyuanbaomall.cn/gtremawtch.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.aibaodan.cn/gtqaaozeth.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.hammf.cn/gtrlgkwauk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.tian-w.cn/gtyzxqiyxv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yongpay.top/gtjeqqhbjx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.52xcode.cn/gtwfmzjmvu.html

[A24] 去除首尾空白
来源：http://hz.yj20258888.top/gtvrwkszgs.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yangfankeji.com/gtsksddmeb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.fzhhl.top/gtikntkyhm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.fzhhl.top/gtlazhjcwd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ybcxt.top/gtuqxbsrqa.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.redwolf501.top/gtbexycrhu.html

Go:   strings.TrimSpace(s)
来源：http://hz.yuanzhike.top/gtjvrtmngy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.haohaochexian.top/gtzhxxprma.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.hywenlv.cn/gtqzjxefsu.html

[A25] 字符串比较
来源：http://hz.zhengqikj.top/gtdjqjixlt.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ywan-chungtsiang.top/gtfcgaugvf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.snrcjt.cn/gtuyypyqin.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.chenjidiqi.icu/gtcngjcucw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.nwbrower.top/gtsadgyvcy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.ydjk.org.cn/gtnqpjuqbp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.xziqi.cn/gthltcvzkg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.zhiwuduotai.top/gtwzjutmaj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.xziqi.cn/gtoljvqzgc.html

[A26] 类型转换总览
来源：http://hz.xinyue.icu/gtcztwebqg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jinqigfzy.top/gtngdwmect.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.xylfe.cn/gttlqicbts.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jiagoushi.top/gtqledeqmc.html

TS:   Number() String() Boolean() x as number
来源：http://hz.wangshuangyany.cn/gtmvsbgjsd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.snrcjt.cn/gthrzxhuav.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yvedp.cn/gtqyaekyal.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.zhijiandao.cn/gtwibfnine.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.xylfe.cn/gtaqjfxjgo.html

================================================================================
来源：http://hz.jiagoushi.top/gtiqykpazs.html

B. 流程控制
来源：http://hz.haohaochexian.top/gtlgppgfnb.html

================================================================================
来源：http://hz.fzhhl.top/gtcznyngec.html

[B01] 条件判断 if / else
来源：http://hz.fzhhl.top/gtuhqhazwr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.cashguo.top/gtvdhsdsgk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.gogol.net.cn/gtrtzqguju.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ywan-chungtsiang.top/gtvhxwdtob.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shuidangran.top/gtbddumzli.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yongpay.top/gtxznmwflh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.xuanzx.com/gtxjyqmzvp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.0kj1m.cn/gtpmyqxhvn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhijiandao.cn/gtpyiuwnub.html

[B02] 多分支 else if / elif
来源：http://hz.cdnleiting.top/gtwpqknqaa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.shuidangran.top/gtqqwvpkxh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.hfpthk.cn/gtmnbyaojc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ehwqpu.com/gtmuwoqlvc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xuetiantiany.cn/gtuumeceth.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daxiang520.top/gtfidnwdkk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.haohaochexian.top/gtbkqsyuyn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.xuetiantiany.cn/gtilzbvzwh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gotoacloud.top/gtdguedqoj.html

[B03] switch / match / case
来源：http://hz.fzhhl.top/gttswzhfww.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.quarkkingdee.top/gthucvlzkl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.nwbrower.top/gtzeafogvv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.kuanghao11.cn/gtezgjrnhr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.shuidangran.top/gtvbmtmeye.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.nanxinkj.top/gtanvslyvx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.feifeiyinyue.top/gtlqudjvqm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jlsjyb.cn/gtzfdlrkuk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.birdmap.top/gtfuwgnatx.html

[B04] for 计数循环
来源：http://hz.hammf.cn/gtcyhvvuyg.html

Py:   for i in range(10): print(i)
来源：http://hz.yvedp.cn/gtanqvdrey.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.daxiang520.top/gtvhjoqggh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yvedp.cn/gtjdofrphb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.birdmap.top/gtgxzxkphh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.xziqi.cn/gtnphcfnye.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.tian-w.cn/gtwyzrokgw.html

Ruby: 10.times { |i| puts i }
来源：http://hz.sweek.top/gtyussndlx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.xylfe.cn/gtnfkakskd.html

[B05] 遍历数组 / 列表
来源：http://hz.daria6918.cn/gtgzyxnukl.html

Py:   for item in arr: print(item)
来源：http://hz.fengsongda.top/gtwbdsgulg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.sweek.top/gtncmpjxmf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.ppjwa.cn/gtkwywukym.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sufxvd.cn/gtyimzeoxl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.xylfe.cn/gtobmrridj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zhoulong.xyz/gthlgwbyll.html

Ruby: arr.each { |item| puts item }
来源：http://hz.gogol.net.cn/gthzyylxad.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.redwolf501.top/gtdqipyoep.html

[B06] 遍历字典 / 对象
来源：http://hz.haohaochexian.top/gtymjliqxx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.fengsongda.top/gtjplpjnue.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.sweek.top/gtcwyzpqhz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yvedp.cn/gtzsjidspe.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cheryme.top/gthyxixmcp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.guannengcc.top/gtpzybhkme.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.sweek.top/gtvzsjpozk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.pycfn.com/gtjsxgivlp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jlsjyb.cn/gtbxaczbnk.html

[B07] while 循环
来源：http://hz.jqgfzy.top/gtpdxfiska.html

Py:   while i < 10: i += 1
来源：http://hz.hfpthk.cn/gtqkvplovq.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.sufxvd.cn/gtgcqcnvkn.html

JS:   while (i < 10) { i++; }
来源：http://hz.xinyue.icu/gtqdrcydjp.html

TS:   while (i < 10) { i++; }
来源：http://hz.daxiang520.top/gtggktdmrk.html

Java: while (i < 10) { i++; }
来源：http://hz.xylfe.cn/gtlmzhrfgj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yueranfly.top/gtpphhsfkx.html

Ruby: while i < 10; i += 1; end
来源：http://hz.shzxlz.cn/gthbpxxiai.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gthujvfhim.html

[B08] do-while（至少执行一次）
来源：http://hz.yangfankeji.com/gtjeonptvw.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhengqikj.top/gteymmgkrl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhoulong.xyz/gtsobjvfio.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yonumen.top/gtktohyerl.html

TS:   do { i++; } while (i < 10);
来源：http://hz.gaohongyu789.top/gtmoxuxmdp.html

Java: do { i++; } while (i < 10);
来源：http://hz.jlsjyb.cn/gtgndyxmby.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.iojbl.cn/gtknhfxwti.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.aibaodan.cn/gtieeyxnqf.html

C#:   do { i++; } while (i < 10);
来源：http://hz.gotoacloud.top/gteikcfhpy.html

[B09] break 与 continue
来源：http://hz.iojbl.cn/gtqrmshohd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.cashguo.top/gtygmjtlas.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shzxlz.cn/gtchjxetyr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gogol.net.cn/gtcqhfgmio.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258.top/gtxwdfwyzb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenzaomai.com/gtofhxhgcu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jianghu66.top/gtdakcfbap.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhaomingkeji.xyz/gtalqkxeae.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xinyue.icu/gtolqbcwat.html

[B10] 遍历同时拿索引
来源：http://hz.andypj.xyz/gtgaabatbl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xuanzx.com/gtpalupfsh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xinyue.icu/gtendppcjl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.nanxuanxn.top/gtmfkntggr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.tian-w.cn/gtrkbyambc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.tianlin.xyz/gtqzyjqvsy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.shzxlz.cn/gtqlpcnncm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jiagoushi.top/gttfgtsydl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.wangshuangyany.cn/gtznkfdoeh.html

[B11] 生成数字序列 / 区间
来源：http://hz.chenlongwang.top/gtipvvaqoi.html

Py:   list(range(0, 10, 2))
来源：http://hz.fengsongda.top/gtocbqjsyu.html

PHP:  range(0, 10, 2);
来源：http://hz.zhiwuduotai.top/gtpysuevpp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.daxiang520.top/gtrlepimuc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.pycfn.com/gthjravhtz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.guowangkeji.top/gteasibgoq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ybcxt.top/gtpcpwarqw.html

Ruby: (0...10).step(2).to_a
来源：http://hz.nwbrower.top/gtlgstbbav.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.dashuyun.cn/gtpqsiitay.html

[B12] 跳出多层循环
来源：http://hz.zhiwuduotai.top/gttvhgtlxh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.vqdsnc.cn/gthysfhajg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.guannengcc.top/gtsykhtdys.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.pengpengdd.cyou/gtygylalqr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.9152youxi.cn/gtpppnhdwm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258888.top/gttpdgciyy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jlsjyb.cn/gtvdebalrc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yangfankeji.com/gtvnjlfpcx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ydjk.org.cn/gtbdwpyksw.html

[B13] 判断是否为数字
来源：http://hz.sysykeji.top/gtpnzktduh.html

Py:   isinstance(x, (int, float))
来源：http://hz.iojbl.cn/gtogwbcrcp.html

PHP:  is_numeric($x)
来源：http://hz.cqqwz.cn/gtnbvjjfzi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jlsjyb.cn/gtfgmyblmj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.pycfn.com/gttwsenhww.html

Java: x instanceof Number
来源：http://hz.ydjk.org.cn/gtgstiqrqr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cucudq.cn/gtjvbhdhqu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shanyushiyangkeji.top/gtqoamaizv.html

C#:   x is int or double or decimal
来源：http://hz.sufxvd.cn/gtvwtfcvuh.html

[B14] 判断值是否在集合内
来源：http://hz.guowangkeji.top/gthbwhznud.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cdnleiting.top/gtiubczccv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhiwuduotai.top/gtgypwdise.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yj20258888.top/gtjmaloxeb.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhiwuduotai.top/gtemseikzb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.dashuyun.cn/gtphhewdco.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhaomingkeji.xyz/gtgtwtgumm.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xingfuxueyuan.xyz/gtlwipirsz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhongyouzk.top/gttvhszews.html

[B15] 布尔运算与取反
来源：http://hz.316326.xyz/gtjuosdujv.html

Py:   a and b or not c
来源：http://hz.nwbrower.top/gtkbxbahyk.html

PHP:  $a && $b || !$c
来源：http://hz.daxiang520.top/gtfdjasowe.html

JS:   a && b || !c
来源：http://hz.dianchejie.cn/gtdmpocwah.html

TS:   a && b || !c
来源：http://hz.aibaodan.cn/gtgddtcexp.html

Java: a && b || !c
来源：http://hz.shzxlz.cn/gtavvpuolv.html

Go:   a && b || !c
来源：http://hz.cheryme.top/gtbggznofa.html

Ruby: a && b || !c
来源：http://hz.cheryme.top/gtmuemlkjs.html

C#:   a && b || !c
来源：http://hz.guowangkeji.top/gtylogdbah.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ivvv.top/gtuvjbbdow.html

Py:   if not data: return
来源：http://hz.shanyushiyangkeji.top/gtspcnbeky.html

PHP:  if (!$data) { return; }
来源：http://hz.yangfankeji.com/gtsmbmnvxx.html

JS:   if (!data) return;
来源：http://hz.zdqjudy.top/gttxbyuanf.html

TS:   if (!data) return;
来源：http://hz.zhaomingkeji.xyz/gtgihnhtor.html

Java: if (data == null) return;
来源：http://hz.yangfankeji.com/gtkaccfkfl.html

Go:   if data == nil { return }
来源：http://hz.daxiang520.top/gtrzcrjsfo.html

Ruby: return if data.nil?
来源：http://hz.havefunace.top/gtojpslcis.html

C#:   if (data == null) return;
来源：http://hz.ydjk.org.cn/gtsidsvmjm.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtaahsgjdu.html

C. 函数与作用域
来源：http://hz.yongpay.top/gtuyltjkjm.html

================================================================================
来源：http://hz.tian-w.cn/gthqumtcrx.html

[C01] 定义函数
来源：http://hz.jinqigufen.top/gtauhutneo.html

Py:   def add(a, b): return a + b
来源：http://hz.sxryk.cn/gtjlwodklg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtmtsbmxpp.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtegkoenvj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.smart0.xyz/gtbwwvjslr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.chenlongwang.top/gtshvqdafb.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gotoacloud.top/gtdrbhixjz.html

Ruby: def add(a, b); a + b; end
来源：http://hz.chenzaomai.com/gtqcducfti.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yanxiufei.cn/gtckloqewd.html

[C02] 默认参数
来源：http://hz.andypj.xyz/gtkefkundn.html

Py:   def greet(name="World"): return name
来源：http://hz.shzxlz.cn/gtpkmqwvnj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jiagoushi.top/gtghckbwxd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hnxiangtu.top/gtyyqgugow.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.aibaodan.cn/gtcjwmgcpf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinqigufen.top/gtuoetoekw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sweek.top/gtxdgobqrn.html

Ruby: def greet(name = "World") = name
来源：http://hz.shanyushiyangkeji.top/gtytuzpadw.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.guowangkeji.top/gtqvpwaege.html

[C03] 可变参数
来源：http://hz.aibaodan.cn/gtaekfacwu.html

Py:   def total(*args): return sum(args)
来源：http://hz.havefunace.top/gtsneciosr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.gaohongyu789.top/gtijrtmgvu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xylfe.cn/gtmwdxkkdg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhongyouzk.top/gtkyjcflbj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hfpthk.cn/gtexcpdbbe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.c1oappe.top/gttmpzysxh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jiagoushi.top/gtvvewofjs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhongyouzk.top/gtjlzzuqeh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jyoumei.cn/gtpzkaqikf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.havefunace.top/gtdtctaztc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.pengpengdd.cyou/gtlunmnhhu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.guowangkeji.top/gtyqexgjwo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhongyouzk.top/gtngunjdxm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.bjfxy.top/gtfncprrsp.html


<!-- 参考信息 -->