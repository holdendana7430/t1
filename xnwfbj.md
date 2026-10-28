代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://hz.chenlongwang.top/gtdodusvst.html

[A15] 空值判断与默认值
来源：http://hz.jqgfzy.top/gtinpfcpsa.html

Py:   value = data or "默认值"
来源：http://hz.gotoacloud.top/gtounvkjoq.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.svipenyu.cn/gtbqpbjvww.html

JS:   const value = data ?? "默认值";
来源：http://hz.zdqjudy.top/gttbowpsgy.html

TS:   const value = data ?? "默认值";
来源：http://hz.tanke756.top/gtfrrzrmde.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.shanyushiyangtech.top/gtthbfsxoj.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.ppjwa.cn/gtnmoxrjyw.html

Ruby: value = data || "默认值"
来源：http://hz.ydzc1.top/gtqifosfxd.html

C#:   var value = data ?? "默认值";
来源：http://hz.aibaodan.cn/gtlalojcns.html

[A16] 真假值判断规则
来源：http://hz.yonumen.top/gtmguewofw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.vqdsnc.cn/gtjyurmbjz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.shanyushiyangkeji.top/gtcwufdwhw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.dianchejie.cn/gtytuzdcbr.html

TS:   if (!x) {}
来源：http://hz.316326.xyz/gtfdvritxc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.xuanzx.com/gtlriswdrt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.birdmap.top/gtvdtokriq.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.jinghuilouyu.cn/gtemevxqbl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.zhengqikj.top/gtuptrxlvx.html

[A17] 位运算
来源：http://hz.shanyushiyangtech.top/gtouzqyqyd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.quarkkingdee.top/gtsbrgpjkf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.xziqi.cn/gtfpdnngdb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shzxlz.cn/gtqbrgqyya.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.ppjwa.cn/gtcoiiuljl.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.meibo888.top/gtjfgeizkq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.smart0.xyz/gtzbwgrkju.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinghuilouyu.cn/gtxrsqzzfg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.9152youxi.cn/gtqmjolylo.html

[A18] 字符与 ASCII 码互转
来源：http://hz.shzxlz.cn/gtowalpguk.html

Py:   ord("A"); chr(65)
来源：http://hz.meibo888.top/gtvjuiosmc.html

PHP:  ord("A"); chr(65)
来源：http://hz.feifeiyinyue.top/gtwmbtkpff.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.birdmap.top/gtxfdctyxt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.tian-w.cn/gtzyqgqzew.html

Java: (int) 'A'; (char) 65
来源：http://hz.shangyingyoupin.top/gteskegxys.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.guannengcc.top/gtifmcsbni.html

Ruby: "A".ord; 65.chr
来源：http://hz.iojbl.cn/gtfhfalhgb.html

C#:   (int)'A'; (char)65
来源：http://hz.c1oappe.top/gthqavfwts.html

[A19] 交换两个变量
来源：http://hz.cdnleiting.top/gtglngpuvk.html

Py:   a, b = b, a
来源：http://hz.zdqjudy.top/gtxgemgkud.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.tian-w.cn/gtnuzboytv.html

JS:   [a, b] = [b, a];
来源：http://hz.vqdsnc.cn/gtxtketkio.html

TS:   [a, b] = [b, a];
来源：http://hz.dashuyun.cn/gtkmqidmji.html

Java: int t = a; a = b; b = t;
来源：http://hz.yonumen.top/gtpgsukjln.html

Go:   a, b = b, a
来源：http://hz.jyoumei.cn/gttvthaemu.html

Ruby: a, b = b, a
来源：http://hz.ivvv.top/gtqpthtwup.html

C#:   (a, b) = (b, a);
来源：http://hz.chenlongwang.top/gtapyfmlie.html

[A20] 读取标准输入
来源：http://hz.hongshengwenyu.top/gtbtmpiupk.html

Py:   name = input("请输入：")
来源：http://hz.tanke756.top/gtpmnvgxhk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.bjfxy.top/gthobkqphr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.yj20258.top/gtgkocjfxe.html

TS:   // Node.js：readline 模块
来源：http://hz.shangyingyoupin.top/gtbypdfbst.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.jianghu66.top/gtyufsuiqs.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.yj20258888.top/gtrshemurf.html

Ruby: gets.chomp
来源：http://hz.snrcjt.cn/gtsvnfkvqt.html

C#:   Console.ReadLine();
来源：http://hz.xuanzx.com/gtkjmssvre.html

[A21] 保留指定小数位输出
来源：http://hz.yueranfly.top/gturiuefxn.html

Py:   f"{3.14159:.2f}"
来源：http://hz.kuanghao11.cn/gtulhtczub.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.0kj1m.cn/gtpdjwknej.html

JS:   (3.14159).toFixed(2)
来源：http://hz.yuxming.cn/gtyiautfcb.html

TS:   (3.14159).toFixed(2)
来源：http://hz.jqgfzy.top/gtqeuezpyo.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.cucudq.cn/gtluqzxyjh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.jiagoushi.top/gtildizuxc.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.wangshuangyany.cn/gtunsjbofr.html

C#:   3.14159.ToString("F2")
来源：http://hz.zhoulong.xyz/gtleenetta.html

[A22] 获取字符串长度
来源：http://hz.gzhubu.top/gtsfkrbmgl.html

Py:   len(s)
来源：http://hz.ivvv.top/gtkadieypg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.jqgfzy.top/gtksplgacw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.mhx1999.top/gtjvaecbxm.html

TS:   s.length
来源：http://hz.feifeiyinyue.top/gtyjwiioop.html

Java: s.length()
来源：http://hz.cucudq.cn/gtfoqrwshe.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.xuanzx.com/gtbjphtxgj.html

Ruby: s.length
来源：http://hz.ybcxt.top/gtkvcpkewy.html

C#:   s.Length
来源：http://hz.yuanzhike.top/gtpgsxextb.html

[A23] 大小写转换
来源：http://hz.ppjwa.cn/gtiqhyrffq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.svipenyu.cn/gtqvliyakm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.zhixingplan.top/gtvqmxhyum.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yvedp.cn/gtdesaeepy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jqgfzy.top/gtmzovqlhq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.pengpengdd.cyou/gtlqslxlml.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.hnqzz.top/gtttpbyoeo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.haohaochexian.top/gtxvfgvytv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.kuanghao11.cn/gtilyaqkof.html

[A24] 去除首尾空白
来源：http://hz.dianchejie.cn/gtssnmccxm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.ydzc1.top/gtruavfced.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.hammf.cn/gtwnkyryxs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.shzxlz.cn/gtavwcbvow.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.guowangkeji.top/gtjquenoru.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.52xcode.cn/gtifztapya.html

Go:   strings.TrimSpace(s)
来源：http://hz.vqdsnc.cn/gtrskvmsul.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.sweek.top/gtubmklrsa.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.sweek.top/gtkabpepgr.html

[A25] 字符串比较
来源：http://hz.jinqigufen.top/gtogrhlwjw.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ybcxt.top/gtnweorqxr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.hammf.cn/gtaqlblzgu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sufxvd.cn/gtkkiijuzz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shzxlz.cn/gtxggajzwo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.kuanghao11.cn/gtunckajyv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.shangyingyoupin.top/gtxczqdrvw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.jinqigfzy.top/gtlihmbetw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.sxryk.cn/gtmtdgofpv.html

[A26] 类型转换总览
来源：http://hz.fzhhl.top/gtpwcluvim.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zhijiandao.cn/gtsnpbtnnx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.xinyue.icu/gtnwqeasvd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jinyuanbaomall.cn/gtruvchulh.html

TS:   Number() String() Boolean() x as number
来源：http://hz.xziqi.cn/gtxkvqlzrh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.redwolf501.top/gtylawbwup.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.nwbrower.top/gtmjacnxyj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.xylfe.cn/gtofdwqpxa.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.guowangkeji.top/gtqvqlvkzf.html

================================================================================
来源：http://hz.pycfn.com/gtjywmlcrl.html

B. 流程控制
来源：http://hz.shuidangran.top/gtjpsnrzdo.html

================================================================================
来源：http://hz.daxiang520.top/gtqxpngbqu.html

[B01] 条件判断 if / else
来源：http://hz.yuxming.cn/gtyrjgvwws.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.aizwys.cn/gtmpxlwshj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jqgfzy.top/gtsjtjeosl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.mhx1999.top/gtqqcdvupc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xingfuxueyuan.xyz/gtufnrhtkd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.ehwqpu.com/gtidgnzfzb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yuxming.cn/gtbvfrukjz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.fengsongda.top/gtcaokurfz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.bjfxy.top/gtnllohnrx.html

[B02] 多分支 else if / elif
来源：http://hz.shanyushiyangtech.top/gtzxxctpua.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.jqgufenzy.top/gtudwiqzyk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yj20258888.top/gtmsbpxgly.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xylfe.cn/gtpwdbmqzs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258.top/gtvykvhzju.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pycfn.com/gtbxtnhbot.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.vqdsnc.cn/gtvphuxcys.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jinyuanbaomall.cn/gtfxvywipm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pycfn.com/gtmtpbjwyi.html

[B03] switch / match / case
来源：http://hz.yuanzhike.top/gtpzfurpkh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jqgfzy.top/gtycuskblx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jqgfzy.top/gtrjeeuasy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhongyouzk.top/gtflffgrhx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.vqdsnc.cn/gtunuspjel.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jinghuilouyu.cn/gtpxjmnsez.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.ehwqpu.com/gtwnksgujd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.52xcode.cn/gtqyqtjpfp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.meibo888.top/gthnxlokay.html

[B04] for 计数循环
来源：http://hz.hysaishi.cn/gtiidihwan.html

Py:   for i in range(10): print(i)
来源：http://hz.yuanzhike.top/gtsqsbiydi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jqgufenzy.top/gtthawfnkv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ehwqpu.com/gtbbeqnbqn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cucudq.cn/gteflinkio.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yangfankeji.com/gtywfzjhiq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jianghu66.top/gtgvhzlafu.html

Ruby: 10.times { |i| puts i }
来源：http://hz.daxiang520.top/gtyroindim.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jinqigfzy.top/gttibqgqsp.html

[B05] 遍历数组 / 列表
来源：http://hz.ybcxt.top/gtoyktdsyw.html

Py:   for item in arr: print(item)
来源：http://hz.aibaodan.cn/gtokigdkbr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.shangyingyoupin.top/gtgivohcrh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.c1oappe.top/gtcgdkkiik.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.quarkkingdee.top/gtlmdyoydc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.cqqwz.cn/gtxfaoytrx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ehwqpu.com/gtyyqujxsk.html

Ruby: arr.each { |item| puts item }
来源：http://hz.tian-w.cn/gtnofaxmrh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.havefunace.top/gtmzbzxdlv.html

[B06] 遍历字典 / 对象
来源：http://hz.hfpthk.cn/gtvzvavarg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.svipenyu.cn/gtjwxhdyhy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jianghu66.top/gttbqadhjo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cashguo.top/gtoyutfhoz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinqigufen.top/gtouflzrkc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.jinghuilouyu.cn/gtozocnorj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hnqzz.top/gtazbjlyni.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jinyuanbaomall.cn/gtziokcocx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.gzhubu.top/gtplclktnj.html

[B07] while 循环
来源：http://hz.xingfuxueyuan.xyz/gtnjkbkuqq.html

Py:   while i < 10: i += 1
来源：http://hz.hongshengwenyu.top/gtuciozagf.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.kuanghao11.cn/gtwglzboxm.html

JS:   while (i < 10) { i++; }
来源：http://hz.ybcxt.top/gtzjqjtrko.html

TS:   while (i < 10) { i++; }
来源：http://hz.smart0.xyz/gtjhsuvkxp.html

Java: while (i < 10) { i++; }
来源：http://hz.sysykeji.top/gtlridsyzc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yuxming.cn/gtrhagdgea.html

Ruby: while i < 10; i += 1; end
来源：http://hz.daria6918.cn/gtjszhawcn.html

C#:   while (i < 10) { i++; }
来源：http://hz.nanxinkj.top/gtxlpjoyno.html

[B08] do-while（至少执行一次）
来源：http://hz.yanxiufei.cn/gtoxwqqqkr.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.nanxuanxn.top/gtdfkyotsa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.shzxlz.cn/gtozetrdem.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zycfv.cn/gtspjrucyw.html

TS:   do { i++; } while (i < 10);
来源：http://hz.haohaochexian.top/gtxaezuizh.html

Java: do { i++; } while (i < 10);
来源：http://hz.zdqjudy.top/gtmdxbqxye.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yj202588.top/gtpsaikcro.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jinqigufen.top/gtvtcpfqoe.html

C#:   do { i++; } while (i < 10);
来源：http://hz.ydjk.org.cn/gtakbgyaif.html

[B09] break 与 continue
来源：http://hz.jqgfzy.top/gthwhbrilh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.andypj.xyz/gtrvscdkpm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.sufxvd.cn/gtlwqwgzyk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cdnleiting.top/gtfwdtnapn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.vqdsnc.cn/gtjehckdpd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sxryk.cn/gtfhvniscd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.aibaodan.cn/gtxsajbfiy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhixingplan.top/gtojtczafc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ppjwa.cn/gtgyehjcgm.html

[B10] 遍历同时拿索引
来源：http://hz.jiagoushi.top/gtzypuwbkd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.pengpengdd.cyou/gtxnaapxwj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.316326.xyz/gtohuxfeye.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yangfankeji.com/gtjtqujzlg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.haohaochexian.top/gtwdpdgvwh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cheryme.top/gtmeboehwt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.ydjk.org.cn/gtexibproh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xuetiantiany.cn/gtrbjsumtz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.wangshuangyany.cn/gtzusaflgy.html

[B11] 生成数字序列 / 区间
来源：http://hz.dashuyun.cn/gtiasmwyzl.html

Py:   list(range(0, 10, 2))
来源：http://hz.gaohongyu789.top/gtujlzjaai.html

PHP:  range(0, 10, 2);
来源：http://hz.andypj.xyz/gtocxxtsci.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ybcxt.top/gtyesellzw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhiwuduotai.top/gtdxfipcuc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.mhx1999.top/gtkawvkwyz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.quarkkingdee.top/gtfivbhnre.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sweek.top/gtcatwdoai.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yonumen.top/gtqswpjrwg.html

[B12] 跳出多层循环
来源：http://hz.cashguo.top/gtofdzbrpo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shzxlz.cn/gtavxvcslc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.wangshuangyany.cn/gtjimngltm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ehwqpu.com/gtacuipnmc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gotoacloud.top/gtrsrhnjyk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuanzx.com/gtklovxuwf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.meibo888.top/gtskncowfg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zycfv.cn/gttjpvudpm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhijiandao.cn/gtejwoufxg.html

[B13] 判断是否为数字
来源：http://hz.zycfv.cn/gtgbwihhhu.html

Py:   isinstance(x, (int, float))
来源：http://hz.jyoumei.cn/gtimcyzole.html

PHP:  is_numeric($x)
来源：http://hz.sxryk.cn/gtowkmvozv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xingfuxueyuan.xyz/gtfeemoxrt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xylfe.cn/gtpawxwifn.html

Java: x instanceof Number
来源：http://hz.jqgfzy.top/gtzbdjzjqp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ivvv.top/gtrdmlxtuc.html

Ruby: x.is_a?(Numeric)
来源：http://hz.chenlongwang.top/gtpmsazwdk.html

C#:   x is int or double or decimal
来源：http://hz.52xcode.cn/gtubwwanfl.html

[B14] 判断值是否在集合内
来源：http://hz.jyoumei.cn/gthklytogl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zycfv.cn/gtxbplpspx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ywan-chungtsiang.top/gtanlrchhq.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.9152youxi.cn/gtwjgandwr.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xuanzx.com/gtgajpiiwv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cashguo.top/gtclbngxrd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.nwbrower.top/gtxiadapqt.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.feifeiyinyue.top/gtvaxprqtv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zycfv.cn/gtawpkndfy.html

[B15] 布尔运算与取反
来源：http://hz.cdnleiting.top/gtjrocajkp.html

Py:   a and b or not c
来源：http://hz.jlsjyb.cn/gtegnzpedx.html

PHP:  $a && $b || !$c
来源：http://hz.hongshengwenyu.top/gtjhxrsonu.html

JS:   a && b || !c
来源：http://hz.daxiang520.top/gtipczsmdd.html

TS:   a && b || !c
来源：http://hz.pycfn.com/gtlihitzui.html

Java: a && b || !c
来源：http://hz.hammf.cn/gtmmgaxcxk.html

Go:   a && b || !c
来源：http://hz.xylfe.cn/gtuiwctokv.html

Ruby: a && b || !c
来源：http://hz.ybcxt.top/gtivjscuov.html

C#:   a && b || !c
来源：http://hz.tian-w.cn/gtopabaqje.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhongyouzk.top/gtoynigxam.html

Py:   if not data: return
来源：http://hz.hysaishi.cn/gtkgsnjyri.html

PHP:  if (!$data) { return; }
来源：http://hz.mhx1999.top/gtootnsbio.html

JS:   if (!data) return;
来源：http://hz.nanxinkj.top/gtsisnpfth.html

TS:   if (!data) return;
来源：http://hz.0kj1m.cn/gtmzeqotkg.html

Java: if (data == null) return;
来源：http://hz.xylfe.cn/gtoxzorfwp.html

Go:   if data == nil { return }
来源：http://hz.shanyushiyangtech.top/gtvgnngflq.html

Ruby: return if data.nil?
来源：http://hz.dianchejie.cn/gtqnilmewl.html

C#:   if (data == null) return;
来源：http://hz.yuxming.cn/gtbijffvyo.html

================================================================================
来源：http://hz.fengsongda.top/gtfdgbrpzf.html

C. 函数与作用域
来源：http://hz.havefunace.top/gtldynmfzj.html

================================================================================
来源：http://hz.havefunace.top/gtskraybmh.html

[C01] 定义函数
来源：http://hz.yuanzhike.top/gtxxiaelms.html

Py:   def add(a, b): return a + b
来源：http://hz.jianghu66.top/gtomgzqbtx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtnuosjmmr.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xuanzx.com/gtnmkvrdmw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtyxfxpixl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinqigfzy.top/gtymdnumxi.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xylfe.cn/gtiosoevky.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jinyuanbaomall.cn/gtdwknyjdi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jqgufenzy.top/gtweqtimcr.html

[C02] 默认参数
来源：http://hz.hnqzz.top/gtmnnbxjrn.html

Py:   def greet(name="World"): return name
来源：http://hz.hongshengwenyu.top/gtdmbyiexn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zycfv.cn/gtvrqstfna.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.wangshuangyany.cn/gtcpayluih.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cashguo.top/gtmzcovips.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yuxming.cn/gtqcqbkaui.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.wangshuangyany.cn/gtfbdbprtb.html

Ruby: def greet(name = "World") = name
来源：http://hz.yanxiufei.cn/gthluoqrum.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jqgfzy.top/gtntrkylee.html

[C03] 可变参数
来源：http://hz.zhoulong.xyz/gtkagmqyvh.html

Py:   def total(*args): return sum(args)
来源：http://hz.shangyingyoupin.top/gtugwbehye.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.kuanghao11.cn/gtukrfdwwe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xingfuxueyuan.xyz/gtsavhzzaf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nanxuanxn.top/gtmffvmmsl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xuanzx.com/gtjzyeniyg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yj202588.top/gtzcygetna.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ydjk.org.cn/gtyounyupw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xylfe.cn/gtdwiriybc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yanxiufei.cn/gtzdustrzm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.daria6918.cn/gtxgpjzgst.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gzhubu.top/gtcydjkfmd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.chenzaomai.com/gtzhuaoklu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.dianchejie.cn/gtknkknnwj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yj20258.top/gtjkldwcnb.html

Go:   // 无：用配置结构体参数
来源：http://hz.ybcxt.top/gtyjlhtyxf.html

Ruby: f(a: 1, b: 2)
来源：http://hz.nanxinkj.top/gtsstzzsgd.html

C#:   f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtgkfqqdpi.html

[C05] 返回多个值
来源：http://hz.fengsongda.top/gtfedgmazb.html

Py:   return a, b
来源：http://hz.cdnleiting.top/gtxarqyuqj.html

PHP:  return [$a, $b];
来源：http://hz.jyoumei.cn/gteapiimwd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yj202588.top/gttwezbsdn.html

TS:   return { a, b };
来源：http://hz.nanxuanxn.top/gtrfabcbua.html


<!-- 参考信息 -->