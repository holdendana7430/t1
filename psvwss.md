代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://hz.nanxuanxn.top/gtjtfmxrhy.html

TS:   const value = data ?? "默认值";
来源：http://hz.xinyue.icu/gtvpjoqamh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.hongshengwenyu.top/gtwqpdzcob.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.nwbrower.top/gtvcjgpdji.html

Ruby: value = data || "默认值"
来源：http://hz.zhoulong.xyz/gtudypfeut.html

C#:   var value = data ?? "默认值";
来源：http://hz.ppjwa.cn/gtzeerqezg.html

[A16] 真假值判断规则
来源：http://hz.9152youxi.cn/gttsgxxtne.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.yj202588.top/gtbuyyuauh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.gotoacloud.top/gtjcikjado.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.ehwqpu.com/gtgllvaipg.html

TS:   if (!x) {}
来源：http://hz.jqgufenzy.top/gtjetsophp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.guannengcc.top/gtctceifuz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.vqdsnc.cn/gtchfhdhbw.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.guannengcc.top/gtmqyjnpua.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.hnxiangtu.top/gtpqppvatk.html

[A17] 位运算
来源：http://hz.aizwys.cn/gtzueukjns.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hfpthk.cn/gtldtjikuh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yueranfly.top/gtcnkmuykc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shzxlz.cn/gtxbiwjvua.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.vqdsnc.cn/gtiqbbuhad.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hongshengwenyu.top/gthswhuxad.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.pengpengdd.cyou/gtiaxlcihy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.meibo888.top/gtheibkboe.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.redwolf501.top/gtppszhgjm.html

[A18] 字符与 ASCII 码互转
来源：http://hz.fengsongda.top/gtztdktast.html

Py:   ord("A"); chr(65)
来源：http://hz.chenlongwang.top/gtukbmafhs.html

PHP:  ord("A"); chr(65)
来源：http://hz.xuetiantiany.cn/gtleoijcus.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.chenjidiqi.icu/gtvuyaphmd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jiagoushi.top/gtnefklvbg.html

Java: (int) 'A'; (char) 65
来源：http://hz.zhiwuduotai.top/gtqumczfqx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.guannengcc.top/gtkakwzhfn.html

Ruby: "A".ord; 65.chr
来源：http://hz.hnqzz.top/gtbhgssqyi.html

C#:   (int)'A'; (char)65
来源：http://hz.jqgufenzy.top/gtiokspkeu.html

[A19] 交换两个变量
来源：http://hz.hysaishi.cn/gtuizpuuok.html

Py:   a, b = b, a
来源：http://hz.daxiang520.top/gtfayichnm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.yj20258888.top/gtuwfbvxcw.html

JS:   [a, b] = [b, a];
来源：http://hz.cucudq.cn/gtgqgyanud.html

TS:   [a, b] = [b, a];
来源：http://hz.jinyuanbaomall.cn/gtnmjyaivq.html

Java: int t = a; a = b; b = t;
来源：http://hz.daxiang520.top/gtyeqthupl.html

Go:   a, b = b, a
来源：http://hz.xziqi.cn/gthxwljbzq.html

Ruby: a, b = b, a
来源：http://hz.jianghu66.top/gtnknbjdsh.html

C#:   (a, b) = (b, a);
来源：http://hz.wangshuangyany.cn/gtgntwbaot.html

[A20] 读取标准输入
来源：http://hz.xziqi.cn/gthfshhvpz.html

Py:   name = input("请输入：")
来源：http://hz.birdmap.top/gtglqfzlcx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.gaohongyu789.top/gtgqbctiwo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.316326.xyz/gtdycitpif.html

TS:   // Node.js：readline 模块
来源：http://hz.nwbrower.top/gthqxnkhqs.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.pycfn.com/gtaxmjvfay.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.nanxuanxn.top/gtvamyfbtm.html

Ruby: gets.chomp
来源：http://hz.yongpay.top/gtfmlvakhm.html

C#:   Console.ReadLine();
来源：http://hz.zhaomingkeji.xyz/gtrogfmvdy.html

[A21] 保留指定小数位输出
来源：http://hz.hongshengwenyu.top/gtjdwdotbh.html

Py:   f"{3.14159:.2f}"
来源：http://hz.zhixingplan.top/gtjcpyrvgr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.vqdsnc.cn/gtwmljkrbq.html

JS:   (3.14159).toFixed(2)
来源：http://hz.andypj.xyz/gtchmblmla.html

TS:   (3.14159).toFixed(2)
来源：http://hz.ehwqpu.com/gtccrtjukr.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.dianchejie.cn/gtnokyzcvj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.jianghu66.top/gtwcjbzgxj.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.zdqjudy.top/gtcndynmpt.html

C#:   3.14159.ToString("F2")
来源：http://hz.dianchejie.cn/gtfjklhutq.html

[A22] 获取字符串长度
来源：http://hz.jinqigufen.top/gtyjwworpp.html

Py:   len(s)
来源：http://hz.dashuyun.cn/gtusqykwis.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.havefunace.top/gtclxhadxx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.pycfn.com/gtgvyxlnxr.html

TS:   s.length
来源：http://hz.yangfankeji.com/gtpydadwms.html

Java: s.length()
来源：http://hz.yvedp.cn/gtudjtfcoc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.yj20258888.top/gtdthpphfo.html

Ruby: s.length
来源：http://hz.guowangkeji.top/gtwilvprpf.html

C#:   s.Length
来源：http://hz.cqqwz.cn/gtogpvsscb.html

[A23] 大小写转换
来源：http://hz.ywan-chungtsiang.top/gtlqbvisox.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.iojbl.cn/gtahzgzmnf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.ydzc1.top/gtshosumxt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hfpthk.cn/gtdvilnsib.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yuanzhike.top/gtggctwvip.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.dashuyun.cn/gtokxvkygl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.sysykeji.top/gtpodpqdep.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zhijiandao.cn/gthbtyunfi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.gogol.net.cn/gtecibyafl.html

[A24] 去除首尾空白
来源：http://hz.shzxlz.cn/gtcpcrjnra.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.vqdsnc.cn/gtjvpucjkg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.daxiang520.top/gtkpepnzzi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.tanke756.top/gtcdegovjl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.cucudq.cn/gtkhecwgsw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.yj20258888.top/gtayjvobsg.html

Go:   strings.TrimSpace(s)
来源：http://hz.tianlin.xyz/gthgkfhawu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.hammf.cn/gtodqsvcdq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.nanxinkj.top/gtcnngetjt.html

[A25] 字符串比较
来源：http://hz.xziqi.cn/gtwwiseoro.html

Py:   s1 == s2; s1 != s2
来源：http://hz.cheryme.top/gtqmhbkhrk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.wangshuangyany.cn/gtngdpbxtw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yj20258.top/gtmeiaihhu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.birdmap.top/gtlfqneeie.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.jqgufenzy.top/gtaxmbybil.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yj202588.top/gtnedcnsiy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.jiagoushi.top/gtenclwppf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.wangdashe.top/gtttpdnbpc.html

[A26] 类型转换总览
来源：http://hz.zdqjudy.top/gtbyugvicq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.havefunace.top/gtfwsoxuoy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.gaohongyu789.top/gtscmkixtm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.vqdsnc.cn/gtnapzelvv.html

TS:   Number() String() Boolean() x as number
来源：http://hz.ehwqpu.com/gtxfroavud.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.svipenyu.cn/gthhtjdjnf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.wangdashe.top/gtzuwtuxom.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.xylfe.cn/gtezyoxlju.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.wangshuangyany.cn/gtcocrqmhe.html

================================================================================
来源：http://hz.birdmap.top/gtotpfwcby.html

B. 流程控制
来源：http://hz.jinqigfzy.top/gtcptgbnth.html

================================================================================
来源：http://hz.snrcjt.cn/gtqtfpathr.html

[B01] 条件判断 if / else
来源：http://hz.xinyue.icu/gtnthoyuqx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.sufxvd.cn/gtxhxfefos.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jiagoushi.top/gtsjalmlmn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.cashguo.top/gtnigbwspz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258.top/gtpcvvodrn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.shanyushiyangtech.top/gtpqbgvzqb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.xylfe.cn/gtafgfjvxn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yanxiufei.cn/gtbuovivwp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hnqzz.top/gtelkojuyx.html

[B02] 多分支 else if / elif
来源：http://hz.yvedp.cn/gthmafjuhs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.kuanghao11.cn/gtgwgkhvaj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yj20258.top/gtmzoytjqf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhengqikj.top/gtineumunb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hfpthk.cn/gthuppuvzh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinqigufen.top/gtymxihstm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.quarkkingdee.top/gtgjywsiji.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.dianchejie.cn/gtzjkxmxkx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shanyushiyangtech.top/gtylzfgyhc.html

[B03] switch / match / case
来源：http://hz.tanke756.top/gttmzfcptj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.hongshengwenyu.top/gtdtadkwwz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.cdnleiting.top/gtmanvqbrq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.guannengcc.top/gtpwvlqbsb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ywan-chungtsiang.top/gtywtanitv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yj20258888.top/gthopabdsp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.tian-w.cn/gtlkkcpltc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jiagoushi.top/gtrxacdrbu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.dianchejie.cn/gttkiwqlcz.html

[B04] for 计数循环
来源：http://hz.jyoumei.cn/gtdoeuqqkm.html

Py:   for i in range(10): print(i)
来源：http://hz.shanyushiyangkeji.top/gtdphknpnn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yangfankeji.com/gttnpxglsf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yanxiufei.cn/gtupqfhtqm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.smart0.xyz/gtlupeomet.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhijiandao.cn/gtqtyujdon.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.shuidangran.top/gtczxrpwqd.html

Ruby: 10.times { |i| puts i }
来源：http://hz.yuanzhike.top/gtslhctmbn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yuxming.cn/gtafaejfwu.html

[B05] 遍历数组 / 列表
来源：http://hz.jqgufenzy.top/gtmspeqhec.html

Py:   for item in arr: print(item)
来源：http://hz.ivvv.top/gtncyuvole.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hnxiangtu.top/gtfpswmvtx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yj202588.top/gteguugczb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.smart0.xyz/gtvyarajrn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.wangshuangyany.cn/gtxmvtuvwg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jqgufenzy.top/gtbppbtuxd.html

Ruby: arr.each { |item| puts item }
来源：http://hz.pycfn.com/gtitdjyjkp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yj202588.top/gtnrybmyvb.html

[B06] 遍历字典 / 对象
来源：http://hz.tianlin.xyz/gtwpmjufml.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.shanyushiyangkeji.top/gtiqohjwvy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.dashuyun.cn/gtcffkervk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yongpay.top/gtrspsuvya.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.haohaochexian.top/gtgzzvofdd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.bjfxy.top/gtxbhwsjku.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jinghuilouyu.cn/gtiqpdbkfs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.ivvv.top/gtpzbounwt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jyoumei.cn/gtsdfwtlbx.html

[B07] while 循环
来源：http://hz.jinyuanbaomall.cn/gtztrvfipg.html

Py:   while i < 10: i += 1
来源：http://hz.sufxvd.cn/gtocguyair.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.cdnleiting.top/gthoxsjatb.html

JS:   while (i < 10) { i++; }
来源：http://hz.ybcxt.top/gtrhnciadf.html

TS:   while (i < 10) { i++; }
来源：http://hz.wangshuangyany.cn/gtfaxjlcex.html

Java: while (i < 10) { i++; }
来源：http://hz.xziqi.cn/gtavtcpdlw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yj20258.top/gtaxmnaqzy.html

Ruby: while i < 10; i += 1; end
来源：http://hz.fzhhl.top/gtmdkgfekx.html

C#:   while (i < 10) { i++; }
来源：http://hz.hnqzz.top/gtgtodprvt.html

[B08] do-while（至少执行一次）
来源：http://hz.yueranfly.top/gtdpafzhqa.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ivvv.top/gtlhaksnsv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.shanyushiyangtech.top/gtiuqequzv.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jqgufenzy.top/gttektcsds.html

TS:   do { i++; } while (i < 10);
来源：http://hz.redwolf501.top/gtneciranb.html

Java: do { i++; } while (i < 10);
来源：http://hz.kuanghao11.cn/gtixrltbxg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yj20258888.top/gtxswtifhv.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hysaishi.cn/gtmipxxddz.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hfpthk.cn/gtpbjxhqho.html

[B09] break 与 continue
来源：http://hz.guowangkeji.top/gtzpjhixnx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.tanke756.top/gtjqsockxw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.fengsongda.top/gtrvxjvrbz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sweek.top/gtfkmgvdbi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuxming.cn/gtdklbzrje.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yvedp.cn/gtujjlmmsl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.cashguo.top/gtjmkwgxwc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xziqi.cn/gtdzzugvpd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxinkj.top/gtxfgoghdu.html

[B10] 遍历同时拿索引
来源：http://hz.yangfankeji.com/gtsskzxjpc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jyoumei.cn/gtxljgykhm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gogol.net.cn/gtybvvzxsg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.chenzaomai.com/gturjclutb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jianghu66.top/gtdqoowjqi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shanyushiyangtech.top/gtlpgdwgqt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.wangshuangyany.cn/gteqsgjdqc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xuetiantiany.cn/gtefcrbxub.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.xuanzx.com/gtmknkjizq.html

[B11] 生成数字序列 / 区间
来源：http://hz.sufxvd.cn/gtuumfyxii.html

Py:   list(range(0, 10, 2))
来源：http://hz.aibaodan.cn/gtedrywkju.html

PHP:  range(0, 10, 2);
来源：http://hz.yj202588.top/gtmksjiplj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gaohongyu789.top/gtveacvbny.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xylfe.cn/gtfdcmxtdi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hnxiangtu.top/gtygzondvt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.kuanghao11.cn/gtooxwotjm.html

Ruby: (0...10).step(2).to_a
来源：http://hz.kuanghao11.cn/gtwasjutlq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.kuanghao11.cn/gtfhlohxpb.html

[B12] 跳出多层循环
来源：http://hz.yongpay.top/gtrepczepp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yonumen.top/gtjgxeefnq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yuxming.cn/gtmpkrslho.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuxming.cn/gtpzhwisei.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jiagoushi.top/gtjbvciopo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.quarkkingdee.top/gtobcakggg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guowangkeji.top/gtkrpuiutd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hfpthk.cn/gtvyhsegpc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yuxming.cn/gtpdnrquow.html

[B13] 判断是否为数字
来源：http://hz.ivvv.top/gtyjeriygi.html

Py:   isinstance(x, (int, float))
来源：http://hz.tianlin.xyz/gtbqtlaewr.html

PHP:  is_numeric($x)
来源：http://hz.yj20258888.top/gttrnnoytv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dianchejie.cn/gtwwhjcqqt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtxqabxhdu.html

Java: x instanceof Number
来源：http://hz.hfpthk.cn/gtjntyfxmm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ybcxt.top/gtvxqdmkus.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yangfankeji.com/gtstxjpkxi.html

C#:   x is int or double or decimal
来源：http://hz.cheryme.top/gtfnysneay.html

[B14] 判断值是否在集合内
来源：http://hz.quarkkingdee.top/gtwvwdtybz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shzxlz.cn/gtibdkzcvk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.meibo888.top/gtzocdlasc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hfpthk.cn/gtakkrqmwg.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.andypj.xyz/gtyhrvpikl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jlsjyb.cn/gtcxanskle.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhijiandao.cn/gtxugeggkt.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yangfankeji.com/gtpcvccnen.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cucudq.cn/gtvgagygrv.html

[B15] 布尔运算与取反
来源：http://hz.yj20258.top/gtvjwesxlv.html

Py:   a and b or not c
来源：http://hz.sysykeji.top/gtkrutfnhd.html

PHP:  $a && $b || !$c
来源：http://hz.gogol.net.cn/gtnuzghbxa.html

JS:   a && b || !c
来源：http://hz.gotoacloud.top/gtlwgfjdrc.html

TS:   a && b || !c
来源：http://hz.zdqjudy.top/gthlbbilmh.html

Java: a && b || !c
来源：http://hz.jiagoushi.top/gtthqxkuez.html

Go:   a && b || !c
来源：http://hz.pengpengdd.cyou/gtqkifyfch.html

Ruby: a && b || !c
来源：http://hz.quarkkingdee.top/gtgaklfchc.html

C#:   a && b || !c
来源：http://hz.guannengcc.top/gtplmpwbbe.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.chenlongwang.top/gticatldxy.html

Py:   if not data: return
来源：http://hz.yuxming.cn/gtpecuipou.html

PHP:  if (!$data) { return; }
来源：http://hz.cdnleiting.top/gtfumneisc.html

JS:   if (!data) return;
来源：http://hz.cashguo.top/gtavgqvlaj.html

TS:   if (!data) return;
来源：http://hz.fengsongda.top/gtbunostlt.html

Java: if (data == null) return;
来源：http://hz.gaohongyu789.top/gtgjfntmfl.html

Go:   if data == nil { return }
来源：http://hz.yangfankeji.com/gtkxzjsxwg.html

Ruby: return if data.nil?
来源：http://hz.tanke756.top/gtzscolfqb.html

C#:   if (data == null) return;
来源：http://hz.hysaishi.cn/gtkvpwnayv.html

================================================================================
来源：http://hz.aibaodan.cn/gtysulipxz.html

C. 函数与作用域
来源：http://hz.xuanzx.com/gtaynbmjfl.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtescwqezb.html

[C01] 定义函数
来源：http://hz.haohaochexian.top/gtpzcjndfq.html

Py:   def add(a, b): return a + b
来源：http://hz.andypj.xyz/gtezldqhur.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.9152youxi.cn/gtiywotfog.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtwaesbjfe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.havefunace.top/gtdxjzhlss.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xylfe.cn/gtmhxgojsi.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.wangdashe.top/gtfxmyfsam.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xingfuxueyuan.xyz/gtcmmchplu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinqigufen.top/gtjtstyygb.html

[C02] 默认参数
来源：http://hz.nanxinkj.top/gtyhmbgyhh.html

Py:   def greet(name="World"): return name
来源：http://hz.sufxvd.cn/gtlhblnlhy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hammf.cn/gtyxnrvizd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hfpthk.cn/gtnszhbknd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.daxiang520.top/gtzhlotvzx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.fengsongda.top/gtdfpikyur.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.daria6918.cn/gthsyibjxi.html

Ruby: def greet(name = "World") = name
来源：http://hz.xylfe.cn/gtplrbutzh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.kuanghao11.cn/gthisfgweu.html

[C03] 可变参数
来源：http://hz.xuetiantiany.cn/gtogijhayq.html

Py:   def total(*args): return sum(args)
来源：http://hz.andypj.xyz/gtojohdglk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.52xcode.cn/gtggblvukz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gaohongyu789.top/gtspwkqwyv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinyuanbaomall.cn/gtiqzoutew.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhongyouzk.top/gttsrednuw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.pycfn.com/gtgjyzwqbh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gzhubu.top/gtltomjhfa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.fzhhl.top/gtnoarvspu.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shanyushiyangkeji.top/gttuphjocr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.snrcjt.cn/gtgvbprslf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhongyouzk.top/gtusocgija.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jlsjyb.cn/gtvsycjikr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.daxiang520.top/gtzkszmwvd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yueranfly.top/gtuyzrcwam.html

Go:   // 无：用配置结构体参数
来源：http://hz.jyoumei.cn/gttqzfkopv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gtovapcutk.html

C#:   f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtmmltlssb.html

[C05] 返回多个值
来源：http://hz.yuxming.cn/gtxmoemjxe.html

Py:   return a, b
来源：http://hz.kuanghao11.cn/gtnmknlbjd.html

PHP:  return [$a, $b];
来源：http://hz.chenzaomai.com/gtxxqhofeg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yueranfly.top/gtmblvpmln.html

TS:   return { a, b };
来源：http://hz.andypj.xyz/gtzsyatvoi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.aizwys.cn/gtrlvlqfca.html

Go:   return a, b
来源：http://hz.xylfe.cn/gtadjzzsmx.html

Ruby: return a, b
来源：http://hz.jiagoushi.top/gtvuamiumo.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.pengpengdd.cyou/gtqgwzpivp.html


<!-- 参考信息 -->