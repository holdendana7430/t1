代发 wailian999

Java: "第一行\n第二行"
来源：http://hz.jlsjyb.cn/gthepdzdsg.html

Go:   "第一行\n第二行"
来源：http://hz.ydjk.org.cn/gtgdarwirp.html

Ruby: "第一行\n第二行"
来源：http://hz.zhixingplan.top/gtzsxieygk.html

C#:   "第一行\n第二行"
来源：http://hz.yj202588.top/gtrhiqxhvy.html

[A14] 注释写法
来源：http://hz.wangdashe.top/gteqkqfhle.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.nwbrower.top/gtqiwtipki.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.cdnleiting.top/gtcqjsgtjw.html

JS:   // 单行；/* 多行 */
来源：http://hz.jinghuilouyu.cn/gtfgqsrkjn.html

TS:   // 单行；/* 多行 */
来源：http://hz.jyoumei.cn/gtjvyacqee.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.xuetiantiany.cn/gtmtswbmip.html

Go:   // 单行；/* 多行 */
来源：http://hz.c1oappe.top/gtovxnwfnj.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.yvedp.cn/gtdlqurfcj.html

C#:   // 单行；/* 多行 */
来源：http://hz.shanyushiyangtech.top/gtwoemdtfx.html

[A15] 空值判断与默认值
来源：http://hz.tianlin.xyz/gtelyecrtk.html

Py:   value = data or "默认值"
来源：http://hz.yuanzhike.top/gtdljvodmw.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.9152youxi.cn/gtqzsrqmrz.html

JS:   const value = data ?? "默认值";
来源：http://hz.mhx1999.top/gtpuklmjpx.html

TS:   const value = data ?? "默认值";
来源：http://hz.xinyue.icu/gtmbddjaue.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.nanxuanxn.top/gtmielgqif.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.gzhubu.top/gtqzywehbx.html

Ruby: value = data || "默认值"
来源：http://hz.bjfxy.top/gtqaoaivls.html

C#:   var value = data ?? "默认值";
来源：http://hz.tanke756.top/gtlmvdlinu.html

[A16] 真假值判断规则
来源：http://hz.kuanghao11.cn/gtaqncgtun.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.dianchejie.cn/gtsrczycqk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.52xcode.cn/gtruyhwptz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.zhiwuduotai.top/gtckuelvck.html

TS:   if (!x) {}
来源：http://hz.kuanghao11.cn/gttgycykem.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.yanxiufei.cn/gteiawbljj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.gotoacloud.top/gtrefvpuoe.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.jinghuilouyu.cn/gtnqpizpov.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.nanxinkj.top/gtaueydnrf.html

[A17] 位运算
来源：http://hz.aizwys.cn/gtpqgtzxpi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cheryme.top/gtfsbncgbc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yj20258888.top/gtjulznuex.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.dashuyun.cn/gtkyiszrut.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.9152youxi.cn/gtndcrsxwd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sysykeji.top/gtvsymvsvk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.sufxvd.cn/gtytxdqytn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jianghu66.top/gthtyfuhci.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.guannengcc.top/gtxclnvmmr.html

[A18] 字符与 ASCII 码互转
来源：http://hz.yvedp.cn/gteehioldp.html

Py:   ord("A"); chr(65)
来源：http://hz.xylfe.cn/gtkfhxqhaz.html

PHP:  ord("A"); chr(65)
来源：http://hz.xuetiantiany.cn/gtohaspqay.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhongyouzk.top/gtcwemtkcp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.fengsongda.top/gtmoruaovq.html

Java: (int) 'A'; (char) 65
来源：http://hz.jinqigfzy.top/gtatwojzun.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.shanyushiyangkeji.top/gtxlinzocr.html

Ruby: "A".ord; 65.chr
来源：http://hz.jinyuanbaomall.cn/gtemouxllx.html

C#:   (int)'A'; (char)65
来源：http://hz.xuanzx.com/gtbasehxla.html

[A19] 交换两个变量
来源：http://hz.guowangkeji.top/gtkyirstss.html

Py:   a, b = b, a
来源：http://hz.zhaomingkeji.xyz/gtbrsoqwgr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.iojbl.cn/gtfmpzgqno.html

JS:   [a, b] = [b, a];
来源：http://hz.guowangkeji.top/gtflkazphm.html

TS:   [a, b] = [b, a];
来源：http://hz.zycfv.cn/gtuklqkgpm.html

Java: int t = a; a = b; b = t;
来源：http://hz.jinqigufen.top/gtkpqmkbmt.html

Go:   a, b = b, a
来源：http://hz.andypj.xyz/gtinatzznx.html

Ruby: a, b = b, a
来源：http://hz.vqdsnc.cn/gtpytfoqzg.html

C#:   (a, b) = (b, a);
来源：http://hz.shanyushiyangkeji.top/gtlwdjugrs.html

[A20] 读取标准输入
来源：http://hz.sxryk.cn/gtxriymzft.html

Py:   name = input("请输入：")
来源：http://hz.smart0.xyz/gtyrnbazfo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.svipenyu.cn/gtyebduwar.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.pengpengdd.cyou/gtphjbwchj.html

TS:   // Node.js：readline 模块
来源：http://hz.gzhubu.top/gtfoomitae.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.guannengcc.top/gtdxhgeeyb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.shuidangran.top/gtbgmdivwo.html

Ruby: gets.chomp
来源：http://hz.haohaochexian.top/gtfeyxhryt.html

C#:   Console.ReadLine();
来源：http://hz.aizwys.cn/gtohopgyjr.html

[A21] 保留指定小数位输出
来源：http://hz.cucudq.cn/gthmgnopgx.html

Py:   f"{3.14159:.2f}"
来源：http://hz.xingfuxueyuan.xyz/gtipkjmhre.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.xinyue.icu/gtgjhjdmtr.html

JS:   (3.14159).toFixed(2)
来源：http://hz.shanyushiyangkeji.top/gtxurbmadp.html

TS:   (3.14159).toFixed(2)
来源：http://hz.yuanzhike.top/gtxebsqlyo.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.ydjk.org.cn/gtvnabaajx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.9152youxi.cn/gtmlkmaavb.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.xingfuxueyuan.xyz/gtznebctii.html

C#:   3.14159.ToString("F2")
来源：http://hz.zhijiandao.cn/gtqdtrhfot.html

[A22] 获取字符串长度
来源：http://hz.yj20258888.top/gtpkslkkla.html

Py:   len(s)
来源：http://hz.nanxinkj.top/gtejndpiai.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.jianghu66.top/gtrbdukxnx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.yj202588.top/gtjdouatfk.html

TS:   s.length
来源：http://hz.ehwqpu.com/gtkmbcyeab.html

Java: s.length()
来源：http://hz.quarkkingdee.top/gtglyubuxz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.hnxiangtu.top/gthfgvxvoy.html

Ruby: s.length
来源：http://hz.fzhhl.top/gtjhqqrhgq.html

C#:   s.Length
来源：http://hz.jiagoushi.top/gtqvdupqjy.html

[A23] 大小写转换
来源：http://hz.ppjwa.cn/gtpfkoapab.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.cashguo.top/gtatpgtont.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.yongpay.top/gtbubyiejd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jyoumei.cn/gtcxhkjimd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xuanzx.com/gtmwbwfxgz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.shangyingyoupin.top/gtntkxyggh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.ywan-chungtsiang.top/gtkfjnexue.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yongpay.top/gtbamgvfcj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yueranfly.top/gtryjnzbca.html

[A24] 去除首尾空白
来源：http://hz.jinyuanbaomall.cn/gtvwtsxrgi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.zhijiandao.cn/gtvzzzmcwd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.wangshuangyany.cn/gtbmgcdvnb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yueranfly.top/gteaoocqdv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.9152youxi.cn/gtlankhote.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.sysykeji.top/gtnyesdwfl.html

Go:   strings.TrimSpace(s)
来源：http://hz.dianchejie.cn/gtbuudciqz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.sxryk.cn/gtfqooqqqg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.nanxinkj.top/gtlpwhyqjt.html

[A25] 字符串比较
来源：http://hz.jqgfzy.top/gtfxxcjmos.html

Py:   s1 == s2; s1 != s2
来源：http://hz.cdnleiting.top/gtxgofrddw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ywan-chungtsiang.top/gtrwtzifyz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zycfv.cn/gtnssgnkpa.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.wangshuangyany.cn/gtcuvsalqe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.hongshengwenyu.top/gtmojqfhuo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yj202588.top/gtdrmtyzwd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.daxiang520.top/gtuopvumtn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.havefunace.top/gtuqsdegor.html

[A26] 类型转换总览
来源：http://hz.snrcjt.cn/gtikehqfzh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.xylfe.cn/gtdxquwynf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yanxiufei.cn/gtooxoeboe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.fengsongda.top/gtmltdvqcb.html

TS:   Number() String() Boolean() x as number
来源：http://hz.cqqwz.cn/gtnrqgznom.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zhaomingkeji.xyz/gthsbumohn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.cashguo.top/gtjhksrwbj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.aizwys.cn/gtxwfihgxu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.ywan-chungtsiang.top/gtrwcyicik.html

================================================================================
来源：http://hz.pycfn.com/gtqwiqrrii.html

B. 流程控制
来源：http://hz.yueranfly.top/gtectuplxl.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtsoqlzklk.html

[B01] 条件判断 if / else
来源：http://hz.wangshuangyany.cn/gtpfddbluu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.hywenlv.cn/gtriukmdzi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yueranfly.top/gtzhchjdik.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xinyue.icu/gtvzsybppu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jiagoushi.top/gtuqkwmbta.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.sweek.top/gteodmbsai.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.ehwqpu.com/gtjnyrlvzg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.wangshuangyany.cn/gtdfmfnucl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258888.top/gthctfsjqo.html

[B02] 多分支 else if / elif
来源：http://hz.cqqwz.cn/gtrgiiuqyh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.ybcxt.top/gtgadxkqer.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.xziqi.cn/gtjujyxuqe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhongyouzk.top/gtovannkbv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinghuilouyu.cn/gtiesxpjho.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shuidangran.top/gtaqzygkxm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.shanyushiyangtech.top/gtlsrsxhue.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yanxiufei.cn/gtcjvzytpw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.52xcode.cn/gtrvukiqdj.html

[B03] switch / match / case
来源：http://hz.shzxlz.cn/gtfshrpqdx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jqgufenzy.top/gtclnkosln.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jinyuanbaomall.cn/gtxhjyymte.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cqqwz.cn/gtfemscxmh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.chenlongwang.top/gtnikwvzrz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.fengsongda.top/gtnmbgmwvl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yonumen.top/gtcyubigsl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jinyuanbaomall.cn/gtoilujivd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.cashguo.top/gtaovwgodd.html

[B04] for 计数循环
来源：http://hz.zhixingplan.top/gttqvurqpt.html

Py:   for i in range(10): print(i)
来源：http://hz.guowangkeji.top/gtigdfrpdp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.pengpengdd.cyou/gtbzbxtjyo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.wangshuangyany.cn/gtdjvyoced.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.316326.xyz/gtbveeugfx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.hnqzz.top/gtngojgref.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yuxming.cn/gtchugwsdy.html

Ruby: 10.times { |i| puts i }
来源：http://hz.yj20258.top/gtnmmsvmyp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.sufxvd.cn/gtcimijiob.html

[B05] 遍历数组 / 列表
来源：http://hz.sysykeji.top/gtuaskjmox.html

Py:   for item in arr: print(item)
来源：http://hz.jianghu66.top/gttramphjl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yj20258.top/gthmpdtwhm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhaomingkeji.xyz/gtmtiesmom.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hfpthk.cn/gtdaqxlsgv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.shangyingyoupin.top/gthfcykflr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.shuidangran.top/gtwoefyyaa.html

Ruby: arr.each { |item| puts item }
来源：http://hz.dashuyun.cn/gtosqtxtev.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.fengsongda.top/gtivtyubpm.html

[B06] 遍历字典 / 对象
来源：http://hz.yuxming.cn/gtnesfyhob.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.birdmap.top/gtfxpkjzvj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yueranfly.top/gtiqyemkjj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hfpthk.cn/gtwefydhwu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yonumen.top/gtgabaqesv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zhaomingkeji.xyz/gtpxacwmtt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jiagoushi.top/gtiavilpks.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.wangdashe.top/gtrahtwevb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.guannengcc.top/gtcgvbdgcn.html

[B07] while 循环
来源：http://hz.ehwqpu.com/gtftlznmhb.html

Py:   while i < 10: i += 1
来源：http://hz.feifeiyinyue.top/gtccstwvge.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.dashuyun.cn/gtcdlztkwq.html

JS:   while (i < 10) { i++; }
来源：http://hz.jyoumei.cn/gtaumuihdk.html

TS:   while (i < 10) { i++; }
来源：http://hz.pycfn.com/gtbpsvkxgr.html

Java: while (i < 10) { i++; }
来源：http://hz.shanyushiyangtech.top/gtlagvgsqt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jinqigfzy.top/gtdemyilph.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hnqzz.top/gtolofbzfn.html

C#:   while (i < 10) { i++; }
来源：http://hz.sysykeji.top/gtozzaijxn.html

[B08] do-while（至少执行一次）
来源：http://hz.xinyue.icu/gtdhmtmztg.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ydzc1.top/gtylhermqc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yvedp.cn/gtfwbggakz.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtyoojpegj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hywenlv.cn/gtwidehmev.html

Java: do { i++; } while (i < 10);
来源：http://hz.zycfv.cn/gtahyyftfg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yongpay.top/gtdfcgvnvm.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhengqikj.top/gtndgzhfad.html

C#:   do { i++; } while (i < 10);
来源：http://hz.dianchejie.cn/gtbrucmjpn.html

[B09] break 与 continue
来源：http://hz.gogol.net.cn/gtylnpkuzw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jinqigfzy.top/gtoiwelgln.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ivvv.top/gtxaonxxrd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jlsjyb.cn/gtsagknfqo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yangfankeji.com/gtgmtwpsgb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtoiyklknp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.sxryk.cn/gtgegxkhjw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ehwqpu.com/gtvxzegbjo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guowangkeji.top/gtpeejpbkx.html

[B10] 遍历同时拿索引
来源：http://hz.wangdashe.top/gthgqglttb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zdqjudy.top/gtouycfydr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.quarkkingdee.top/gtyqcjiqgl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.fzhhl.top/gttgloszdo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.chenjidiqi.icu/gthdznsuvb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shuidangran.top/gteopptduo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.52xcode.cn/gttbqaifpt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.aizwys.cn/gtwejaacby.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.tian-w.cn/gtaneoosbj.html

[B11] 生成数字序列 / 区间
来源：http://hz.cashguo.top/gtovasszjb.html

Py:   list(range(0, 10, 2))
来源：http://hz.guannengcc.top/gtaydobuqf.html

PHP:  range(0, 10, 2);
来源：http://hz.xylfe.cn/gtbaiciliv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yj202588.top/gtprqoneqp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shzxlz.cn/gtypvygclm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.smart0.xyz/gtxwmfwqpp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.0kj1m.cn/gtsepgzpat.html

Ruby: (0...10).step(2).to_a
来源：http://hz.wangdashe.top/gtzqxjhhmd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhixingplan.top/gteaqonrtu.html

[B12] 跳出多层循环
来源：http://hz.shanyushiyangtech.top/gtmohfretw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.smart0.xyz/gtcdufgdel.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ivvv.top/gtqtfdphjp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.haohaochexian.top/gttnudchez.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.snrcjt.cn/gthhnamqbv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinyuanbaomall.cn/gtpsedaagg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yj202588.top/gtyxmpqhux.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zdqjudy.top/gtqfqkhtzs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jqgufenzy.top/gtmapiycul.html

[B13] 判断是否为数字
来源：http://hz.hongshengwenyu.top/gtslujqwny.html

Py:   isinstance(x, (int, float))
来源：http://hz.hywenlv.cn/gtltxuauwm.html

PHP:  is_numeric($x)
来源：http://hz.ydjk.org.cn/gtkzourkez.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.0kj1m.cn/gtxzpyzxvc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nanxuanxn.top/gtdwysoiaw.html

Java: x instanceof Number
来源：http://hz.gotoacloud.top/gtdbvawqpq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.haohaochexian.top/gtjwjcdxbs.html

Ruby: x.is_a?(Numeric)
来源：http://hz.feifeiyinyue.top/gtmcfzuwyb.html

C#:   x is int or double or decimal
来源：http://hz.nanxinkj.top/gtfqohcogp.html

[B14] 判断值是否在集合内
来源：http://hz.vqdsnc.cn/gtgsnoafyh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hongshengwenyu.top/gtbxodaicr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yj20258.top/gtflgjflsq.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtpyoujpuz.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.sweek.top/gtdhkaesws.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cqqwz.cn/gthhpshkio.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.52xcode.cn/gtvlberhqh.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.pengpengdd.cyou/gtjhzwbaey.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.dianchejie.cn/gtwerwzuoq.html

[B15] 布尔运算与取反
来源：http://hz.chenzaomai.com/gttonbtxnw.html

Py:   a and b or not c
来源：http://hz.hfpthk.cn/gtpkddwfcm.html

PHP:  $a && $b || !$c
来源：http://hz.zhijiandao.cn/gtidnxzrpc.html

JS:   a && b || !c
来源：http://hz.jqgufenzy.top/gtkpspbnrd.html

TS:   a && b || !c
来源：http://hz.aibaodan.cn/gtvzrdcorx.html

Java: a && b || !c
来源：http://hz.bjfxy.top/gtzhaheoeq.html

Go:   a && b || !c
来源：http://hz.ehwqpu.com/gtsbrafldy.html

Ruby: a && b || !c
来源：http://hz.shangyingyoupin.top/gtvxrvhqrn.html

C#:   a && b || !c
来源：http://hz.cdnleiting.top/gtzyvhapfj.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ydzc1.top/gtdrtzthwt.html

Py:   if not data: return
来源：http://hz.nanxinkj.top/gtkalgftnj.html

PHP:  if (!$data) { return; }
来源：http://hz.yvedp.cn/gthsabwucs.html

JS:   if (!data) return;
来源：http://hz.quarkkingdee.top/gtfczlpvqx.html

TS:   if (!data) return;
来源：http://hz.xziqi.cn/gtktoeixff.html

Java: if (data == null) return;
来源：http://hz.guowangkeji.top/gtozoyskfx.html

Go:   if data == nil { return }
来源：http://hz.meibo888.top/gtmhyywwqk.html

Ruby: return if data.nil?
来源：http://hz.hongshengwenyu.top/gtpwhaeaom.html

C#:   if (data == null) return;
来源：http://hz.nwbrower.top/gtupgmllrj.html

================================================================================
来源：http://hz.gaohongyu789.top/gtrnyrjwbe.html

C. 函数与作用域
来源：http://hz.yongpay.top/gtmrsjrrxt.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtzhdlkige.html

[C01] 定义函数
来源：http://hz.tian-w.cn/gtnzjrcxal.html

Py:   def add(a, b): return a + b
来源：http://hz.mhx1999.top/gtdlprxeez.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gtwvsoghoh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtlaljdxxa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ehwqpu.com/gtuolrcwpp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gtkknywcuv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cqqwz.cn/gtywssxral.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hammf.cn/gtdhcjbvqt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gttwvzjshl.html

[C02] 默认参数
来源：http://hz.yueranfly.top/gtpabrdspa.html

Py:   def greet(name="World"): return name
来源：http://hz.mhx1999.top/gteqcgagsp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.sufxvd.cn/gtwbcfdrbo.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hysaishi.cn/gtwvvuhtad.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.shzxlz.cn/gtuqbrtkhk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hfpthk.cn/gtpxoohkzg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.tian-w.cn/gtlqmfmeoq.html

Ruby: def greet(name = "World") = name
来源：http://hz.jianghu66.top/gtsploqgbe.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.chenzaomai.com/gtjymdpibc.html

[C03] 可变参数
来源：http://hz.yuanzhike.top/gtbrenoppj.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhoulong.xyz/gtxlokjcxe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.snrcjt.cn/gtixbqzuqn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zycfv.cn/gtrbeolvte.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.52xcode.cn/gtlxuvkftf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinghuilouyu.cn/gtnkaykdde.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinqigfzy.top/gtcohzhmqy.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sysykeji.top/gtdkxdneqf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.andypj.xyz/gtzxhusquo.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ydzc1.top/gttvjheush.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.fengsongda.top/gtmnnedhgy.html


<!-- 参考信息 -->