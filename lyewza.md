代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://hz.zhongyouzk.top/gthuchfvuj.html

Ruby: arr.include?(x)
来源：http://hz.ivvv.top/gtfcchmalk.html

C#:   list.Contains(x)
来源：http://hz.nanxuanxn.top/gtctrzhckm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yvedp.cn/gtlnclmufw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jyoumei.cn/gtjxrwuwab.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jqgfzy.top/gtbziknplt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.aibaodan.cn/gttxisjnfo.html

TS:   [...arr];
来源：http://hz.chenjidiqi.icu/gtontdjwrc.html

Java: new ArrayList<>(list);
来源：http://hz.hammf.cn/gtuqymbirm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.daxiang520.top/gtmvnamsfv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.dashuyun.cn/gtsjrlcfon.html

C#:   new List<int>(list);
来源：http://hz.gotoacloud.top/gtvbnrhitj.html

[D23] reduce 累积计算
来源：http://hz.yangfankeji.com/gtdpkmzdlr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.chenzaomai.com/gtfrhiatxf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yuxming.cn/gtbyvpxfoa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jlsjyb.cn/gtyytaqkin.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ywan-chungtsiang.top/gtordyueyx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jianghu66.top/gtkhoyjojs.html

Go:   // 手写循环
来源：http://hz.bjfxy.top/gtgsdghfuq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jyoumei.cn/gtkofdshcg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xylfe.cn/gtbqidetvn.html

[D24] 字典 / Map 基本操作
来源：http://hz.52xcode.cn/gtlgluofbe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.meibo888.top/gtaxahqtnm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nwbrower.top/gtpypwlymv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ywan-chungtsiang.top/gtjzlqhmab.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.iojbl.cn/gtlghawpnu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cqqwz.cn/gtvzoawwvw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gaohongyu789.top/gtyvgbspmt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sweek.top/gtyzlvgcno.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhijiandao.cn/gtosxjaknp.html

[D25] Set 集合去重与交并差
来源：http://hz.sysykeji.top/gtppljhmeb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shanyushiyangkeji.top/gtlfihdkfp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zdqjudy.top/gtntextnfc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hnxiangtu.top/gtkyaofgeg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.havefunace.top/gtynfbscrq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yongpay.top/gtaaajudwf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.dianchejie.cn/gtnjvvevgl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinqigufen.top/gtxfaymxmr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gaohongyu789.top/gtfekbrfcw.html

[D26] 数组转字符串
来源：http://hz.hfpthk.cn/gtshupxkep.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ydzc1.top/gtkmdwxkjk.html

PHP:  implode(", ", $arr);
来源：http://hz.jyoumei.cn/gtjlltkdqr.html

JS:   arr.join(", ")
来源：http://hz.guannengcc.top/gtgyxbnacc.html

TS:   arr.join(", ")
来源：http://hz.fengsongda.top/gtpeilwjzp.html

Java: String.join(", ", list)
来源：http://hz.pengpengdd.cyou/gtnmraurrz.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hnqzz.top/gtnloxoiqr.html

Ruby: arr.join(", ")
来源：http://hz.hfpthk.cn/gtgngpmxwz.html

C#:   string.Join(", ", list)
来源：http://hz.sysykeji.top/gthrsxgkre.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtzvdfoskb.html

E. 字符串处理
来源：http://hz.bjfxy.top/gtqhyztwgk.html

================================================================================
来源：http://hz.gotoacloud.top/gtdzissazr.html

[E01] 拼接字符串
来源：http://hz.xziqi.cn/gtibdorpgc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hywenlv.cn/gtmjmnttrm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xylfe.cn/gtsqgcddgf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.andypj.xyz/gthwazdcdb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gttgwacqrv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shanyushiyangtech.top/gtwwthfxqh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.tanke756.top/gtrpfagjjp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj202588.top/gtduihpwwy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtnxxpiygh.html

[E02] 重复字符串
来源：http://hz.hammf.cn/gtplipqobw.html

Py:   "ab" * 3
来源：http://hz.zhiwuduotai.top/gtlgknlnix.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jiagoushi.top/gtnmnyltvm.html

JS:   "ab".repeat(3)
来源：http://hz.yuxming.cn/gtvffikwfx.html

TS:   "ab".repeat(3)
来源：http://hz.cdnleiting.top/gtjsfjifak.html

Java: "ab".repeat(3)
来源：http://hz.jiagoushi.top/gtffchgpzm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sufxvd.cn/gtavtrisjy.html

Ruby: "ab" * 3
来源：http://hz.yuxming.cn/gtjwghkeuj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.iojbl.cn/gtkfrkxial.html

[E03] 截取子串
来源：http://hz.chenjidiqi.icu/gtfvqqzhfg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ivvv.top/gtuqxvehoo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.0kj1m.cn/gtzwlzpuuf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shuidangran.top/gtllijvxao.html

TS:   s.slice(1, 4)
来源：http://hz.tianlin.xyz/gtcbhtyacv.html

Java: s.substring(1, 4)
来源：http://hz.yonumen.top/gtzncswzmi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hongshengwenyu.top/gtrkpxxoax.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.svipenyu.cn/gtlpollhoo.html

C#:   s.Substring(1, 3)
来源：http://hz.yj202588.top/gttfqdjksg.html

[E04] 查找子串位置
来源：http://hz.zhixingplan.top/gtdypokydo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.vqdsnc.cn/gtapddutvn.html

PHP:  strpos($s, "x");
来源：http://hz.hongshengwenyu.top/gtivowcbmh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shuidangran.top/gtbkwlgnoy.html

TS:   s.indexOf("x")
来源：http://hz.c1oappe.top/gtipytjnxq.html

Java: s.indexOf("x")
来源：http://hz.wangdashe.top/gtgzyvhukp.html

Go:   strings.Index(s, "x")
来源：http://hz.hongshengwenyu.top/gtjejbmwnw.html

Ruby: s.index("x")
来源：http://hz.guowangkeji.top/gtzeywvxty.html

C#:   s.IndexOf("x")
来源：http://hz.zdqjudy.top/gtayswwcmd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ydjk.org.cn/gtepaazlgt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.cdnleiting.top/gtaqndbjwi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.bjfxy.top/gtwzhthmxm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cucudq.cn/gtxfkomzyk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yanxiufei.cn/gtdsdxohqj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhijiandao.cn/gtvtgrnkuz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yueranfly.top/gtpogowtxx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xinyue.icu/gtpkgdcxyl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cashguo.top/gtrokirjaq.html

[E06] 替换子串
来源：http://hz.daria6918.cn/gtnzwporps.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.haohaochexian.top/gtyurimlfz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jyoumei.cn/gtezjholxi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yonumen.top/gtontfhlnk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtdhhpqwdt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtzesazmzf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.feifeiyinyue.top/gtuldtsdcn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.guannengcc.top/gtzlzopzdv.html

C#:   s.Replace("a", "b")
来源：http://hz.yueranfly.top/gtxktrmgkk.html

[E07] 按分隔符拆分
来源：http://hz.yuanzhike.top/gteinybjin.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yueranfly.top/gtmzsrxswo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.52xcode.cn/gtsbascpwb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sufxvd.cn/gtyrmgwqyj.html

TS:   s.split(",")
来源：http://hz.cashguo.top/gtgogjpbwd.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.sysykeji.top/gtpbbxqsaj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cqqwz.cn/gtueqhzmqn.html

Ruby: s.split(",");  s.split
来源：http://hz.cheryme.top/gtgmpxwfqn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jqgfzy.top/gtahemyhbr.html

[E08] 数组按分隔符合并
来源：http://hz.tianlin.xyz/gtiehbglqp.html

Py:   ",".join(items)
来源：http://hz.hammf.cn/gtogeqquvr.html

PHP:  implode(",", $items);
来源：http://hz.jyoumei.cn/gtkuacjezn.html

JS:   items.join(",")
来源：http://hz.yuanzhike.top/gthxliupox.html

TS:   items.join(",")
来源：http://hz.yongpay.top/gtitnliewl.html

Java: String.join(",", items)
来源：http://hz.daria6918.cn/gtdmtimmyz.html

Go:   strings.Join(items, ",")
来源：http://hz.gzhubu.top/gtmqbbgqyt.html

Ruby: items.join(",")
来源：http://hz.nwbrower.top/gtnyegncpm.html

C#:   string.Join(",", items)
来源：http://hz.zhiwuduotai.top/gtjtxktjnl.html

[E09] 去除所有空白字符
来源：http://hz.zhaomingkeji.xyz/gtznzcfwxk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.daria6918.cn/gthvpsoljt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.52xcode.cn/gtjpydpkee.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.vqdsnc.cn/gtegcktosx.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.aizwys.cn/gtqhhsavse.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhiwuduotai.top/gtmwzxuqop.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.aizwys.cn/gtszflegod.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shuidangran.top/gtrdkdduvw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ywan-chungtsiang.top/gtbxqxppgi.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xuetiantiany.cn/gtqqlrrlhb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.316326.xyz/gtnwhavpcz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gotoacloud.top/gtkyjkiqgx.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhaomingkeji.xyz/gtwvdwpbhu.html

TS:   "7".padStart(3, "0")
来源：http://hz.hysaishi.cn/gtuxjuqlzp.html

Java: String.format("%03d", 7)
来源：http://hz.316326.xyz/gtabpjhmsb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cheryme.top/gtrcohptoi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.dianchejie.cn/gtsmnlxcez.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yongpay.top/gtlinellor.html

[E11] 反转字符串
来源：http://hz.pengpengdd.cyou/gtnibyyqea.html

Py:   s[::-1]
来源：http://hz.zhengqikj.top/gtnhmqopmi.html

PHP:  strrev($s);
来源：http://hz.hnqzz.top/gtpdqnoeod.html

JS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtrzwkfkak.html

TS:   [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtsdbchuiz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinghuilouyu.cn/gtmrqvsgiu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yuanzhike.top/gtugysmcuu.html

Ruby: s.reverse
来源：http://hz.jlsjyb.cn/gtthivmajy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinyuanbaomall.cn/gtbibmqhuc.html

[E12] 统计某字符出现次数
来源：http://hz.tian-w.cn/gtacfserjc.html

Py:   s.count("a")
来源：http://hz.guowangkeji.top/gtdhthukll.html

PHP:  substr_count($s, "a");
来源：http://hz.kuanghao11.cn/gtivvvnwld.html

JS:   s.split("a").length - 1
来源：http://hz.chenzaomai.com/gtsksuhyws.html

TS:   s.split("a").length - 1
来源：http://hz.jyoumei.cn/gtkoydxkbt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nanxinkj.top/gtcxzyvvmr.html

Go:   strings.Count(s, "a")
来源：http://hz.chenlongwang.top/gthrkmtyok.html

Ruby: s.count("a")
来源：http://hz.kuanghao11.cn/gtfqadrmpt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hnqzz.top/gtmfiblfcp.html

[E13] 逐字符遍历
来源：http://hz.gaohongyu789.top/gttuyffzns.html

Py:   for ch in s: print(ch)
来源：http://hz.zycfv.cn/gtxhldyjfv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gaohongyu789.top/gteunyzcnl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenzaomai.com/gtlucuporm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydzc1.top/gtxsvemjom.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtdufnfpkh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hammf.cn/gtwoluajbd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cashguo.top/gtmjordtep.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yanxiufei.cn/gteomzdafk.html

[E14] URL 编码与 Base64
来源：http://hz.jqgufenzy.top/gtcdywccow.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gaohongyu789.top/gtxeuhjmon.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ywan-chungtsiang.top/gtcgbfkhif.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinqigfzy.top/gtfdkgpjfw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jiagoushi.top/gtkznlpgyr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jianghu66.top/gthozxvvww.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.mhx1999.top/gtssvrvbvc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yongpay.top/gtgyuronwi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ivvv.top/gtiuuivyho.html

[E15] HTML 转义 / 反转义
来源：http://hz.meibo888.top/gtimcpjgen.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yueranfly.top/gtiireapeh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.daxiang520.top/gtdergozgx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yuanzhike.top/gtjfzpbajg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhongyouzk.top/gtskbhrkht.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhijiandao.cn/gtmkxgkmgn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xziqi.cn/gtoikescqb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.haohaochexian.top/gtiihijyhz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhoulong.xyz/gtndwtdtbq.html

[E16] 数字千分位
来源：http://hz.cucudq.cn/gtbofofydf.html

Py:   f"{1234567:,}"
来源：http://hz.jinqigfzy.top/gtpvhtlxpc.html

PHP:  number_format(1234567);
来源：http://hz.havefunace.top/gtovwpnjjc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gthzbjaptt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgfzy.top/gtuyftcmdq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ppjwa.cn/gtbokmqjtw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.feifeiyinyue.top/gtfxnuzhkj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ywan-chungtsiang.top/gtyrpqdwyd.html

C#:   1234567.ToString("N0")
来源：http://hz.redwolf501.top/gtjplszypr.html

[E17] 首字母大写
来源：http://hz.xuanzx.com/gtziskzgod.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj20258888.top/gtylnrucxf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jqgfzy.top/gtnulamhnk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ehwqpu.com/gtgsdfzhwb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guannengcc.top/gtxgggnkww.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tianlin.xyz/gtnjghzyyr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yvedp.cn/gtebugiefw.html

Ruby: s.capitalize
来源：http://hz.cqqwz.cn/gtkenmyruc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinghuilouyu.cn/gtzmumhhwy.html

[E18] 模板占位符替换
来源：http://hz.chenjidiqi.icu/gtjlezysdt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.nanxuanxn.top/gtfzwhdwui.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.redwolf501.top/gtyugmxjzp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.sxryk.cn/gtaqbptyxh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxinkj.top/gtuhqhhube.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gogol.net.cn/gtztmpuedi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinqigufen.top/gthtnlifxm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinghuilouyu.cn/gtgazsslid.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenzaomai.com/gtraxbjwes.html

[E19] 多行文本按行拆分
来源：http://hz.smart0.xyz/gtsyndqebp.html

Py:   s.splitlines()
来源：http://hz.quarkkingdee.top/gtkypuyaqe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.0kj1m.cn/gtsozypjls.html

JS:   s.split(/\r?\n/)
来源：http://hz.9152youxi.cn/gtgghwovph.html

TS:   s.split(/\r?\n/)
来源：http://hz.yj20258888.top/gtmaczihkp.html

Java: s.lines().toList()
来源：http://hz.ydzc1.top/gtjttgvvvb.html

Go:   strings.Split(s, "\n")
来源：http://hz.nanxinkj.top/gtkswtowik.html

Ruby: s.lines
来源：http://hz.sufxvd.cn/gtcuoxukrb.html

C#:   s.Split('\n')
来源：http://hz.cashguo.top/gtwanrihan.html

[E20] 判断字符串是否为空
来源：http://hz.yangfankeji.com/gtdbwcdshl.html

Py:   if not s:
来源：http://hz.quarkkingdee.top/gtmarxmqex.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pengpengdd.cyou/gtmbomadeg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenjidiqi.icu/gtzqpsezbx.html

TS:   if (s === "") {}
来源：http://hz.jqgufenzy.top/gtsyoiykbz.html

Java: if (s.isEmpty()) {}
来源：http://hz.gotoacloud.top/gtokfidkxg.html

Go:   if s == "" {}
来源：http://hz.jinqigfzy.top/gtpigehqhb.html

Ruby: if s.empty?
来源：http://hz.chenzaomai.com/gtghahhajq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shuidangran.top/gtnzskpvov.html

[E21] 超长截断加省略号
来源：http://hz.fzhhl.top/gtwrdbnemf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gzhubu.top/gtffpqncrp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xuanzx.com/gtwzlhqdcz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.0kj1m.cn/gtjiyckkic.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hfpthk.cn/gtrkouvxzr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtgncvgggr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhongyouzk.top/gtugfaugnk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.haohaochexian.top/gtepreutoa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shuidangran.top/gtmasgkiex.html

[E22] 字节长度与字符长度
来源：http://hz.jianghu66.top/gtzegpjeit.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sysykeji.top/gtmtdvmhqo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.52xcode.cn/gtnsluasdd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xingfuxueyuan.xyz/gtxnzrbpnm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ywan-chungtsiang.top/gtsnohfzaz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xuanzx.com/gtuvtogovl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.pycfn.com/gtgsppcxhj.html

Ruby: s.bytesize;  s.length
来源：http://hz.daria6918.cn/gtftxqhkse.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhaomingkeji.xyz/gtgvulylcj.html

================================================================================
来源：http://hz.zhengqikj.top/gtrrkqaxun.html

F. 文件与目录
来源：http://hz.havefunace.top/gtgkbrpdoo.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdgjhawev.html

[F01] 读取整个文件
来源：http://hz.jyoumei.cn/gtxtddlino.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jianghu66.top/gtfsgdrckv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hnqzz.top/gtcjsmmejb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zdqjudy.top/gtjnhuponw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuetiantiany.cn/gtwrhhljvz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gtrnksuejk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hammf.cn/gtlgpiembs.html

Ruby: File.read("a.txt")
来源：http://hz.hfpthk.cn/gtacjdmqpj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.feifeiyinyue.top/gtfhahkrnl.html

[F02] 逐行读取文件
来源：http://hz.gogol.net.cn/gtmdzrzkxk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.kuanghao11.cn/gtnegtfkjw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jianghu66.top/gtgpxcrymx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xylfe.cn/gtcumrdhmr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigufen.top/gtpsvtxxfr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shzxlz.cn/gttirlkfkz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.redwolf501.top/gtigzpqjwr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.bjfxy.top/gtfaxtcjst.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hywenlv.cn/gttvuzlqpe.html

[F03] 写入文件（覆盖）
来源：http://hz.yvedp.cn/gttcsxmvbe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pycfn.com/gtjouwprtw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.fengsongda.top/gtnmborbfi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhoulong.xyz/gtbnnpttje.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jianghu66.top/gtvmwzbicl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sufxvd.cn/gtwhzmdhyx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.c1oappe.top/gtiqxlovjw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ybcxt.top/gtvlplepvq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ydzc1.top/gtpwnkuzek.html

[F04] 追加写入文件
来源：http://hz.nanxuanxn.top/gtqhgviefz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj202588.top/gtismolblq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gzhubu.top/gtzlciubnt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgfzy.top/gthckrvika.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuetiantiany.cn/gtfmlaresq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yvedp.cn/gtywsgvxjd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yongpay.top/gtfatistuq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.fengsongda.top/gtlqnckzuz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.nwbrower.top/gtqbwdyxup.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhaomingkeji.xyz/gtyitpcwgl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nanxinkj.top/gtfmsmrhyw.html

PHP:  file_exists("a.txt");
来源：http://hz.jiagoushi.top/gtszbdzuee.html

JS:   fs.existsSync("a.txt")
来源：http://hz.birdmap.top/gtlxmmrwnf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gteblncimg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtvgsejbju.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.kuanghao11.cn/gtvjaxyxfo.html

Ruby: File.exist?("a.txt")
来源：http://hz.wangshuangyany.cn/gtphqixmeg.html

C#:   File.Exists("a.txt")
来源：http://hz.ppjwa.cn/gtgjfbxxnp.html

[F06] 删除文件
来源：http://hz.yangfankeji.com/gtvdcxadpk.html

Py:   os.remove("a.txt")
来源：http://hz.9152youxi.cn/gtwewcgvkl.html

PHP:  unlink("a.txt");
来源：http://hz.ybcxt.top/gtxbsznwcf.html


<!-- 参考信息 -->