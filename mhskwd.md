代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhongyouzk.top/gtftqscbvv.html

Ruby: rescue ArgumentError => e
来源：http://hz.cucudq.cn/gtfgqorohi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.iojbl.cn/gtmvpetdyd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.316326.xyz/gtagwbfnxm.html

Py:   value = d.get("k") or default
来源：http://hz.zhijiandao.cn/gtjsuutdiz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jiagoushi.top/gtxzrkirzj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jianghu66.top/gtoxmpecdb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtjdqvtdyd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.aibaodan.cn/gtkhjvlxnw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.guannengcc.top/gtsdlqcxfs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zdqjudy.top/gtpkizvjdf.html

C#:   obj?.A?.B ?? default
来源：http://hz.tian-w.cn/gtaybbmxhy.html

[H07] 断言
来源：http://hz.daxiang520.top/gtftzezoca.html

Py:   assert x > 0, "必须为正"
来源：http://hz.havefunace.top/gtdcfollau.html

PHP:  assert($x > 0);
来源：http://hz.zdqjudy.top/gtcroqdclk.html

JS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gtfvwoiihv.html

TS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtmpjjneoj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.kuanghao11.cn/gtnjzqtnxa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hnxiangtu.top/gtidyaqluq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ehwqpu.com/gtzgczhpsy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenzaomai.com/gtbhmiqbit.html

[H08] 获取错误信息与堆栈
来源：http://hz.yangfankeji.com/gtaidbtagy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gogol.net.cn/gtkvhbwqxb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cashguo.top/gthyatffxy.html

JS:   e.message;  e.stack
来源：http://hz.yanxiufei.cn/gthcrchnlt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.316326.xyz/gtmbxgfoug.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.vqdsnc.cn/gtrwkdjqof.html

Go:   err.Error()
来源：http://hz.zhijiandao.cn/gtlpmskkcd.html

Ruby: e.message;  e.backtrace
来源：http://hz.shanyushiyangkeji.top/gtkyjypmsj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxinkj.top/gtbdpzyvmd.html

[H09] 带错误码的异常
来源：http://hz.hfpthk.cn/gtbczmwing.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xinyue.icu/gtzvppqtrb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yvedp.cn/gtlllcmjcy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cheryme.top/gtktuukylx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhaomingkeji.xyz/gtbfgpfksa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nanxinkj.top/gtdcupjagi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.pycfn.com/gtfrcdyfjs.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.pycfn.com/gtxweqbjxu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zycfv.cn/gtclsygtcc.html

[H10] 资源自动释放
来源：http://hz.xingfuxueyuan.xyz/gtlizgulna.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tanke756.top/gtxapwgjyo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gotoacloud.top/gtvfzoprlo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtkovqqduo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gtktkkqxct.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xziqi.cn/gtpndkqroj.html

Go:   defer f.Close()
来源：http://hz.aizwys.cn/gtagmwmxra.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sxryk.cn/gtkpwomxak.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dianchejie.cn/gtikzvqwoh.html

================================================================================
来源：http://hz.vqdsnc.cn/gtriedicuo.html

I. 正则表达式
来源：http://hz.jinyuanbaomall.cn/gtjokidmsi.html

================================================================================
来源：http://hz.jqgfzy.top/gtgbnqhjoj.html

[I01] 判断是否匹配
来源：http://hz.nanxinkj.top/gtzwdlnwja.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtnlbgdyvs.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shanyushiyangkeji.top/gtgncmlezm.html

JS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gtbauphdab.html

TS:   /\d+/.test(s)
来源：http://hz.jinyuanbaomall.cn/gtfdvupksr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aibaodan.cn/gtqtxtnuxo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinqigfzy.top/gthowzludu.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxuanxn.top/gtwcasdsad.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.havefunace.top/gtnygtxfsj.html

[I02] 提取所有匹配
来源：http://hz.xziqi.cn/gtxojapoqm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.fengsongda.top/gtduuaquhw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shangyingyoupin.top/gtnudeehln.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhengqikj.top/gtvyqrjyof.html

TS:   s.match(/\d+/g)
来源：http://hz.ydzc1.top/gtdbpmwblv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ivvv.top/gtxfmivjqw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jqgufenzy.top/gtoqszbfyf.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinqigufen.top/gtydjdyybv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daria6918.cn/gtpcweqfow.html

[I03] 提取捕获分组
来源：http://hz.cdnleiting.top/gtivvobnok.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xylfe.cn/gtxqzodquk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.meibo888.top/gtbqkfpxoa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hywenlv.cn/gtqvpmdpki.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.guannengcc.top/gtygcirnti.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinqigufen.top/gtayvebnab.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhaomingkeji.xyz/gtmuwihfxk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj20258.top/gtikmlnbxl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daria6918.cn/gtfmgiktkp.html

[I04] 正则替换
来源：http://hz.fzhhl.top/gtkqjwzcvu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hammf.cn/gtplcikjip.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinyuanbaomall.cn/gtxtteeblk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shangyingyoupin.top/gtopprykno.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.pycfn.com/gtxlhazspl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sufxvd.cn/gtpzcdkhnq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hysaishi.cn/gtgaczggjp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.wangdashe.top/gtgngnecex.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.chenzaomai.com/gthofpfpiy.html

[I05] 按正则拆分
来源：http://hz.jqgfzy.top/gtdkowmlsv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.9152youxi.cn/gtfijfyonm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhixingplan.top/gtclphtcyu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtfhusayzx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtkbetwmov.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hammf.cn/gtaawfktaw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.feifeiyinyue.top/gtvoudtnnz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtsntmgdln.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xinyue.icu/gtnemtjfem.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258888.top/gtvtullnwl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yvedp.cn/gtorsvklul.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yongpay.top/gttqgcmdrn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xziqi.cn/gthiwjmygf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtjsvbhwzw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhixingplan.top/gtpqcmlvzz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jiagoushi.top/gtchldspgp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.fengsongda.top/gtazthaabu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ydzc1.top/gtcliutivy.html

[I07] 忽略大小写与多行模式
来源：http://hz.xylfe.cn/gtgjruljkf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.pycfn.com/gtrtoaepqi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.wangshuangyany.cn/gtingyyyrz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.mhx1999.top/gtcyilpzsv.html

TS:   /error/gim
来源：http://hz.cashguo.top/gtmvcqllfl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ppjwa.cn/gtwzqsmtpf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinqigfzy.top/gtroftfsye.html

Ruby: s.scan(/error/i)
来源：http://hz.hammf.cn/gtcfhefoft.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yonumen.top/gtwusqllxs.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.0kj1m.cn/gtygjjfdrk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ppjwa.cn/gtgkaspddt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pengpengdd.cyou/gtlgwetnkc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daxiang520.top/gtimhegppd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hammf.cn/gterankpdk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.guowangkeji.top/gtubcduiwt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sxryk.cn/gtiiocitej.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cqqwz.cn/gtifpbblnd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenjidiqi.icu/gtmkcoyrgw.html

================================================================================
来源：http://hz.cucudq.cn/gtlgnjqxfz.html

J. 日期与时间
来源：http://hz.aizwys.cn/gtcjwyboht.html

================================================================================
来源：http://hz.xylfe.cn/gtpmlcrrqt.html

[J01] 获取当前时间
来源：http://hz.havefunace.top/gtymqhmuwb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shangyingyoupin.top/gtivdeksid.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenzaomai.com/gtlhyfcogo.html

JS:   new Date();  Date.now()
来源：http://hz.yj20258888.top/gtmsvivwuz.html

TS:   new Date();  Date.now()
来源：http://hz.sufxvd.cn/gtqkdsnopl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sufxvd.cn/gtqpmyxxnq.html

Go:   time.Now()
来源：http://hz.316326.xyz/gtwvcvjawo.html

Ruby: Time.now
来源：http://hz.guannengcc.top/gtqdgpggmp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.birdmap.top/gtjfmfzsxt.html

[J02] 格式化输出
来源：http://hz.iojbl.cn/gtrqpxpabh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtgfdsasmm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.0kj1m.cn/gtqcstbfyo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nwbrower.top/gtzbsnhgnl.html

TS:   d.toISOString()
来源：http://hz.316326.xyz/gtknzcagnh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xuanzx.com/gtvxtnbnan.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yuanzhike.top/gtccqogfqw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtoevxwwou.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jiagoushi.top/gtmolgatsp.html

[J03] 字符串解析为日期
来源：http://hz.gzhubu.top/gtgztozsyc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.daxiang520.top/gtdlelchkc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangkeji.top/gtfatfdeje.html

JS:   new Date("2024-01-02")
来源：http://hz.shzxlz.cn/gtnhrsvoyn.html

TS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gtumdlnzcu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guowangkeji.top/gtdymnnrnc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jiagoushi.top/gtvuaijxbz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jqgufenzy.top/gtoxzgyidp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jlsjyb.cn/gtzwtnuzld.html

[J04] 时间戳与日期互转
来源：http://hz.jiagoushi.top/gtgzkqlxoq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yangfankeji.com/gtqfmkfcod.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.pycfn.com/gtyamvnvqh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hywenlv.cn/gtjcicqezc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yj20258888.top/gtvuvibfjc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ivvv.top/gtcxmsjhsj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.wangshuangyany.cn/gthapowbut.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhiwuduotai.top/gtoarykpso.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cashguo.top/gtamekxpks.html

[J05] 时间加减（加 7 天）
来源：http://hz.xziqi.cn/gtmwrsngxg.html

Py:   now + timedelta(days=7)
来源：http://hz.ivvv.top/gtnfpqhufz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.kuanghao11.cn/gtvtfyojyh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shangyingyoupin.top/gtyvypahnp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydzc1.top/gtbaajervc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aizwys.cn/gtzqcrbbdn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj20258888.top/gttrszvdrr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zycfv.cn/gtvpdtdbpn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinyuanbaomall.cn/gtmighnysf.html

[J06] 计算两时间之差
来源：http://hz.vqdsnc.cn/gtbfojlfgb.html

Py:   (end - start).total_seconds()
来源：http://hz.gzhubu.top/gtmjudvntq.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenlongwang.top/gtousmzhzo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shuidangran.top/gtydakgsdq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigufen.top/gticcznpmf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenjidiqi.icu/gtcaqimsbi.html

Go:   end.Sub(start).Hours()
来源：http://hz.guowangkeji.top/gtitzohdsl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aibaodan.cn/gtdpgqmfex.html

C#:   (end - start).TotalSeconds
来源：http://hz.andypj.xyz/gtgmabxpos.html

[J07] 比较两个日期
来源：http://hz.gotoacloud.top/gtmbbjnfpx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtarqavdij.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shangyingyoupin.top/gtpusktrxt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yangfankeji.com/gtcassuoro.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gtyicmxusb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenlongwang.top/gtbqzqxglc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhengqikj.top/gtlsujbzwq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtoxzbnbqt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtiizatpnb.html

[J08] 提取年月日与星期
来源：http://hz.daxiang520.top/gtshlasjab.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhaomingkeji.xyz/gtbpsfigao.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gogol.net.cn/gtzrxfebzg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.pengpengdd.cyou/gtbvyobmwu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ppjwa.cn/gtwvsmosot.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhongyouzk.top/gtzetabcrg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sufxvd.cn/gtfuxhehpp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sxryk.cn/gtbmkczbub.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jqgufenzy.top/gtnrwitspd.html

[J09] 时区处理
来源：http://hz.iojbl.cn/gtnydncqur.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinqigfzy.top/gtvwacfyfs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenjidiqi.icu/gtgqrfowkg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gtquwnbhso.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtuwthrmgr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenjidiqi.icu/gtruznyspq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhixingplan.top/gtjrfnlbfz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fzhhl.top/gtixsjrtta.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.kuanghao11.cn/gtkafdazii.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhixingplan.top/gtmamiwqeb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sysykeji.top/gttdejklgp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tian-w.cn/gtbyslggzv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zycfv.cn/gtembqdmcn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinqigufen.top/gtrllecfag.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cashguo.top/gtqxufcoeh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gotoacloud.top/gtrvrfaumd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yvedp.cn/gtipaqumpv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.c1oappe.top/gtiejaqryg.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtebimgxfk.html

K. JSON 与序列化
来源：http://hz.gogol.net.cn/gtgojmdnfq.html

================================================================================
来源：http://hz.sysykeji.top/gtfelqyyrf.html

[K01] 对象转 JSON 字符串
来源：http://hz.zycfv.cn/gtomluzetf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtjfnsndzl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gtlrurtloj.html

JS:   JSON.stringify(obj)
来源：http://hz.mhx1999.top/gtelkxfcfs.html

TS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gteuznrstk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.andypj.xyz/gtrxkxxadj.html

Go:   json.Marshal(obj)
来源：http://hz.52xcode.cn/gtrmefmwxt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj20258.top/gthpxdptvm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigufen.top/gtebyvqbjx.html

[K02] JSON 字符串转对象
来源：http://hz.ppjwa.cn/gtztwkoamn.html

Py:   json.loads(s)
来源：http://hz.redwolf501.top/gtvfkyegdd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xuanzx.com/gtbxvtkujl.html

JS:   JSON.parse(s)
来源：http://hz.sysykeji.top/gtuztkujtf.html

TS:   JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtnvsahkur.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yueranfly.top/gtqfwvlwpl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xuanzx.com/gtmobaxstc.html

Ruby: JSON.parse(s)
来源：http://hz.andypj.xyz/gtyiplnrcw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jiagoushi.top/gtkmhbbkmv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.daria6918.cn/gthjuonbcs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenjidiqi.icu/gtsxklusyf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zycfv.cn/gtfezxezla.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gtlchkdeij.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ybcxt.top/gtxjcymrss.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hammf.cn/gtzqlogkdq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jiagoushi.top/gtqcaiqsim.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jqgfzy.top/gtsintxvsm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gotoacloud.top/gtphsoyjmy.html

[K04] 读取 JSON 文件
来源：http://hz.ydzc1.top/gtruwbwawj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuanzhike.top/gtqgupdskd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gotoacloud.top/gtygatqekw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.svipenyu.cn/gtgyfjgzkx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dashuyun.cn/gtjgpmmijg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.guannengcc.top/gtqncsasif.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.c1oappe.top/gtuxsqxbze.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hnqzz.top/gtkmqoqkbk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangdashe.top/gtdexrhmzx.html

[K05] 深拷贝对象
来源：http://hz.quarkkingdee.top/gtvqbpcibg.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenzaomai.com/gtgjcctvpd.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hysaishi.cn/gtnuioeblw.html

JS:   structuredClone(obj)
来源：http://hz.cucudq.cn/gthbvnqdbl.html

TS:   structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtbtipmpfl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tianlin.xyz/gtricaoyra.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xylfe.cn/gtmbstutpu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fengsongda.top/gtqgdcvzey.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hywenlv.cn/gtnghgjgvx.html

[K06] 解析 URL 查询串
来源：http://hz.daxiang520.top/gteexdnxkh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.meibo888.top/gtfeldnumc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zdqjudy.top/gtqdgvbtwo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hfpthk.cn/gtlaphvrvi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtvaoiitnl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ywan-chungtsiang.top/gtqbmnbsno.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.mhx1999.top/gtxeropwcy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tian-w.cn/gtgiqfsuvn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cucudq.cn/gtimfviujm.html

[K07] 进制转换
来源：http://hz.jyoumei.cn/gtrmzsykhl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhoulong.xyz/gthojraakm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj202588.top/gtlyfdfaja.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xuanzx.com/gttdavxakn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtczcwjggo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yj202588.top/gtubmsbjbd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sysykeji.top/gtihynjkid.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sxryk.cn/gteqfyrrxn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jqgufenzy.top/gtylocgllm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hongshengwenyu.top/gtkfvhfzdi.html

Py:   pickle.dumps(obj)
来源：http://hz.aibaodan.cn/gtklxxwsqx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jyoumei.cn/gtvxdbktbk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangtech.top/gtnrzjdrbb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtwzyjlpxl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.havefunace.top/gtygsmwhev.html

Go:   encoding/gob
来源：http://hz.hnqzz.top/gtltdxtegq.html

Ruby: Marshal.dump(obj)
来源：http://hz.0kj1m.cn/gthllufrkn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hywenlv.cn/gtiiqrsspx.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtifmoixlh.html

L. 网络请求
来源：http://hz.c1oappe.top/gtnjbuzays.html

================================================================================
来源：http://hz.cashguo.top/gtbqyekrfm.html

[L01] 发送 GET 请求
来源：http://hz.shangyingyoupin.top/gtdtxrcehm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.guannengcc.top/gtsvyzmvai.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258.top/gtszpnaesm.html

JS:   await fetch(url)
来源：http://hz.redwolf501.top/gtouvtnojb.html

TS:   await fetch(url)
来源：http://hz.yj202588.top/gtpqlglnnc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jlsjyb.cn/gtllljxaxh.html


<!-- 参考信息 -->