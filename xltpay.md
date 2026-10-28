代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://hz.nanxuanxn.top/gtkslrznli.html

Ruby: arr.include?(x)
来源：http://hz.hfpthk.cn/gtamskbmue.html

C#:   list.Contains(x)
来源：http://hz.zycfv.cn/gtsoxnfpmw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yvedp.cn/gtjxxiwsks.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jlsjyb.cn/gtptzgucjp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daria6918.cn/gtdaiilfhq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.svipenyu.cn/gtlamtigtr.html

TS:   [...arr];
来源：http://hz.yvedp.cn/gtiqyawwqf.html

Java: new ArrayList<>(list);
来源：http://hz.sufxvd.cn/gteoxzdftg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ywan-chungtsiang.top/gtvfxfucjf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinyuanbaomall.cn/gtctbmcyze.html

C#:   new List<int>(list);
来源：http://hz.nanxuanxn.top/gtnqwnrqrp.html

[D23] reduce 累积计算
来源：http://hz.cdnleiting.top/gtakxvywtx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cqqwz.cn/gtpbdzcaon.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.52xcode.cn/gtfysmqcdt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxinkj.top/gtrsdbxwxm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gtkqcueivt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj20258888.top/gtxalvhida.html

Go:   // 手写循环
来源：http://hz.yj202588.top/gtwwtubuud.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.aibaodan.cn/gturfutvvi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.fzhhl.top/gtcdvxvmyt.html

[D24] 字典 / Map 基本操作
来源：http://hz.wangshuangyany.cn/gtpbduudzh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.vqdsnc.cn/gtjghvlcgn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.wangdashe.top/gtarvsvdho.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sufxvd.cn/gtkfmbaiuf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jlsjyb.cn/gtuxsnvrzc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhongyouzk.top/gtambzfjfe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhengqikj.top/gtoxxefzfi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhijiandao.cn/gtwaagtmyp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jlsjyb.cn/gtgbzokqff.html

[D25] Set 集合去重与交并差
来源：http://hz.ivvv.top/gtcpsermmp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.andypj.xyz/gtadbklate.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.dianchejie.cn/gtrlunvqdl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yanxiufei.cn/gtawsuzawj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.316326.xyz/gtbpsyoban.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.fzhhl.top/gtgnusjeka.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.chenjidiqi.icu/gtmyyjbaop.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxinkj.top/gthnaestfs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yuanzhike.top/gtgtwkogko.html

[D26] 数组转字符串
来源：http://hz.yonumen.top/gtvavrdlsq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.quarkkingdee.top/gtfgyaileu.html

PHP:  implode(", ", $arr);
来源：http://hz.aizwys.cn/gtugobruvo.html

JS:   arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtuzfngnth.html

TS:   arr.join(", ")
来源：http://hz.hongshengwenyu.top/gtgecssaxm.html

Java: String.join(", ", list)
来源：http://hz.zycfv.cn/gtvnrkkkre.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hysaishi.cn/gtxxkbhzce.html

Ruby: arr.join(", ")
来源：http://hz.jinqigfzy.top/gtghcktzbu.html

C#:   string.Join(", ", list)
来源：http://hz.guowangkeji.top/gtdtqlccmc.html

================================================================================
来源：http://hz.hammf.cn/gtqziwhybd.html

E. 字符串处理
来源：http://hz.shanyushiyangkeji.top/gtekqbtsso.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtksjfmuzy.html

[E01] 拼接字符串
来源：http://hz.zycfv.cn/gtiogjtfqv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yonumen.top/gtmvcgrzde.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hnqzz.top/gttbieosfr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.meibo888.top/gtemuoqjli.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuetiantiany.cn/gtbxezdcwh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.wangshuangyany.cn/gtjkpyixvc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cucudq.cn/gtabphemea.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.pengpengdd.cyou/gtizjqttqz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhongyouzk.top/gtidliltgj.html

[E02] 重复字符串
来源：http://hz.yongpay.top/gtjmduxska.html

Py:   "ab" * 3
来源：http://hz.gaohongyu789.top/gtwrcybuxu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.shanyushiyangtech.top/gtprddavxw.html

JS:   "ab".repeat(3)
来源：http://hz.ydjk.org.cn/gtoqyyjbwn.html

TS:   "ab".repeat(3)
来源：http://hz.tian-w.cn/gtaqnhxeyb.html

Java: "ab".repeat(3)
来源：http://hz.cashguo.top/gtymiswcbw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.guannengcc.top/gtplzoqepc.html

Ruby: "ab" * 3
来源：http://hz.hammf.cn/gtjkhnshqp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dashuyun.cn/gtpaxivmox.html

[E03] 截取子串
来源：http://hz.zycfv.cn/gtgtofwcta.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ybcxt.top/gtpwbjnbjb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hnxiangtu.top/gtnazkwrcj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258.top/gtywgkbgmr.html

TS:   s.slice(1, 4)
来源：http://hz.shzxlz.cn/gtainqqyrt.html

Java: s.substring(1, 4)
来源：http://hz.tian-w.cn/gtyjjaczmq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zycfv.cn/gtlktttgpa.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yangfankeji.com/gtjnxgklya.html

C#:   s.Substring(1, 3)
来源：http://hz.hfpthk.cn/gtnzuwmkbg.html

[E04] 查找子串位置
来源：http://hz.yvedp.cn/gtxcpnndqm.html

Py:   s.find("x");  s.index("x")
来源：http://hz.redwolf501.top/gtobfamrdh.html

PHP:  strpos($s, "x");
来源：http://hz.cdnleiting.top/gtqtvnrnxp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.snrcjt.cn/gtepvrbrzw.html

TS:   s.indexOf("x")
来源：http://hz.tanke756.top/gtmjckgvlx.html

Java: s.indexOf("x")
来源：http://hz.shzxlz.cn/gttnuowvuu.html

Go:   strings.Index(s, "x")
来源：http://hz.hongshengwenyu.top/gtrgjslhlo.html

Ruby: s.index("x")
来源：http://hz.0kj1m.cn/gtijpyyzup.html

C#:   s.IndexOf("x")
来源：http://hz.nanxinkj.top/gtqqbfxpun.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yuxming.cn/gtwzsujvxg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hnqzz.top/gtdofgthzu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhiwuduotai.top/gtrfmxkdgv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinghuilouyu.cn/gtrdiyrkwk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shzxlz.cn/gtvwwceocj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pycfn.com/gthhrukldo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yangfankeji.com/gtafsvzizk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.c1oappe.top/gtaouogskx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.daria6918.cn/gtrpltgyiv.html

[E06] 替换子串
来源：http://hz.haohaochexian.top/gtudmhuekh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.wangshuangyany.cn/gtkzdbvgqw.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.andypj.xyz/gtbynnwlzn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ydzc1.top/gtammnksjh.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gthmfmdezj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgfzy.top/gtinqsqwzv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.birdmap.top/gthsfdruvi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.nanxinkj.top/gthtmldgzz.html

C#:   s.Replace("a", "b")
来源：http://hz.zycfv.cn/gtslaiblvn.html

[E07] 按分隔符拆分
来源：http://hz.zhiwuduotai.top/gtwidqlzgq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jqgfzy.top/gtxkvfaorp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.meibo888.top/gtpjwbkgdt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yongpay.top/gtvlyxwpzw.html

TS:   s.split(",")
来源：http://hz.52xcode.cn/gtizgftpqe.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cheryme.top/gttjpgkiva.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.pycfn.com/gtsdpugevv.html

Ruby: s.split(",");  s.split
来源：http://hz.zhixingplan.top/gtuifdecny.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hywenlv.cn/gthkmmdhgs.html

[E08] 数组按分隔符合并
来源：http://hz.cheryme.top/gtmnlnifht.html

Py:   ",".join(items)
来源：http://hz.cheryme.top/gtrlckqrtl.html

PHP:  implode(",", $items);
来源：http://hz.hongshengwenyu.top/gtfkwgjbaw.html

JS:   items.join(",")
来源：http://hz.meibo888.top/gtazvwwutr.html

TS:   items.join(",")
来源：http://hz.sxryk.cn/gtxfizssvd.html

Java: String.join(",", items)
来源：http://hz.andypj.xyz/gtbwvjztms.html

Go:   strings.Join(items, ",")
来源：http://hz.zhengqikj.top/gtbesqaawr.html

Ruby: items.join(",")
来源：http://hz.zhongyouzk.top/gtdunvooss.html

C#:   string.Join(",", items)
来源：http://hz.snrcjt.cn/gtdtwfitik.html

[E09] 去除所有空白字符
来源：http://hz.sweek.top/gtdxdeifyd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.9152youxi.cn/gtwgfpasck.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.tanke756.top/gtywysrqpl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.aizwys.cn/gtpnujzbmh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.aibaodan.cn/gtycrdhvbd.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tanke756.top/gtkvutxngx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hnqzz.top/gtzzcydsxu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yj202588.top/gtqsuepoxn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shzxlz.cn/gtkidrievx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sweek.top/gtqrufklpe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.feifeiyinyue.top/gtfellnkyu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daxiang520.top/gtzpbyfksb.html

JS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtuqjexezc.html

TS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtsbaejitf.html

Java: String.format("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtxypdvbrb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gotoacloud.top/gtkfukalia.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zycfv.cn/gtsapnoyvc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gogol.net.cn/gtdwdmiifs.html

[E11] 反转字符串
来源：http://hz.feifeiyinyue.top/gtbyanckmz.html

Py:   s[::-1]
来源：http://hz.wangshuangyany.cn/gtlbrmsqhz.html

PHP:  strrev($s);
来源：http://hz.yvedp.cn/gtxemtyxfi.html

JS:   [...s].reverse().join("")
来源：http://hz.316326.xyz/gtjdippblk.html

TS:   [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtzuzoczbc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dashuyun.cn/gtdotiehwz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ehwqpu.com/gthgcuevhf.html

Ruby: s.reverse
来源：http://hz.shangyingyoupin.top/gtljlhyjde.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.daria6918.cn/gtwgyytple.html

[E12] 统计某字符出现次数
来源：http://hz.zhengqikj.top/gtykzgytqc.html

Py:   s.count("a")
来源：http://hz.haohaochexian.top/gtwfmmyajz.html

PHP:  substr_count($s, "a");
来源：http://hz.hnxiangtu.top/gtiphpsrmj.html

JS:   s.split("a").length - 1
来源：http://hz.daxiang520.top/gtecyttgpl.html

TS:   s.split("a").length - 1
来源：http://hz.smart0.xyz/gtduymeack.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhixingplan.top/gtebjozaps.html

Go:   strings.Count(s, "a")
来源：http://hz.jqgufenzy.top/gtppltocxy.html

Ruby: s.count("a")
来源：http://hz.zhengqikj.top/gtxbquxgbg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.svipenyu.cn/gtcpxwudjl.html

[E13] 逐字符遍历
来源：http://hz.ydzc1.top/gtvmmlyrjf.html

Py:   for ch in s: print(ch)
来源：http://hz.jinghuilouyu.cn/gtxsisgtss.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gaohongyu789.top/gthxuqunwx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shangyingyoupin.top/gtdfaubzua.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gtqefrwpwe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.c1oappe.top/gtghigqypk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cashguo.top/gtkyiqxtnk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jyoumei.cn/gtdezyirbe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jianghu66.top/gtmqhnejcf.html

[E14] URL 编码与 Base64
来源：http://hz.mhx1999.top/gtaeqgifvy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ydzc1.top/gtdkwdnelh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.daxiang520.top/gtwowyzavk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jqgfzy.top/gtgzsvlair.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hnqzz.top/gtvttaqlyy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigfzy.top/gtdqcbyqtt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinqigfzy.top/gtkrplqbyk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shzxlz.cn/gtqjxcvvkh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cheryme.top/gtwftezrnk.html

[E15] HTML 转义 / 反转义
来源：http://hz.9152youxi.cn/gtfyskvhfe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.snrcjt.cn/gtqkmqhjvw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yanxiufei.cn/gtclgswabt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.dashuyun.cn/gtrehobjsd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xuanzx.com/gtyuwuoxbf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.daria6918.cn/gtkreayxmg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cheryme.top/gtqungaxiv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhiwuduotai.top/gtvmaydbue.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.meibo888.top/gtimakydwz.html

[E16] 数字千分位
来源：http://hz.chenjidiqi.icu/gtikrpxgfr.html

Py:   f"{1234567:,}"
来源：http://hz.nanxinkj.top/gtfxrjgovt.html

PHP:  number_format(1234567);
来源：http://hz.yj20258888.top/gtxenpcajw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtumiqcupb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydzc1.top/gtfaxzalsa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tian-w.cn/gttdpitpmy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xingfuxueyuan.xyz/gtqvhqbngq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.pengpengdd.cyou/gtsdrhnfsc.html

C#:   1234567.ToString("N0")
来源：http://hz.jianghu66.top/gtxkgedmvd.html

[E17] 首字母大写
来源：http://hz.c1oappe.top/gtlvriaweg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cashguo.top/gthsszfqac.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cucudq.cn/gtflftfkes.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shangyingyoupin.top/gttabklskq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnxiangtu.top/gtncujynso.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hongshengwenyu.top/gtoygmytpw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj202588.top/gtrcyhxjzr.html

Ruby: s.capitalize
来源：http://hz.jianghu66.top/gtqitipbhp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cashguo.top/gtfbfzatbi.html

[E18] 模板占位符替换
来源：http://hz.wangdashe.top/gtbumekwpu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jianghu66.top/gtlstcfhhq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tanke756.top/gtzpfovbnm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nwbrower.top/gtkkaovunc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhijiandao.cn/gtggelnvgt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xziqi.cn/gtztzrwpwh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yonumen.top/gttcttisnf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhoulong.xyz/gtatyybasu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jiagoushi.top/gtfsonigrp.html

[E19] 多行文本按行拆分
来源：http://hz.havefunace.top/gtyagsgfdd.html

Py:   s.splitlines()
来源：http://hz.chenzaomai.com/gtrqskswoa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhixingplan.top/gtkemzpkat.html

JS:   s.split(/\r?\n/)
来源：http://hz.pengpengdd.cyou/gtnindyoyx.html

TS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtnusivdum.html

Java: s.lines().toList()
来源：http://hz.cashguo.top/gtabzvcyol.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinyuanbaomall.cn/gtvoxttmck.html

Ruby: s.lines
来源：http://hz.xingfuxueyuan.xyz/gtyvuwodpc.html

C#:   s.Split('\n')
来源：http://hz.cdnleiting.top/gtzgmyvxpq.html

[E20] 判断字符串是否为空
来源：http://hz.chenzaomai.com/gtavwbjczp.html

Py:   if not s:
来源：http://hz.yangfankeji.com/gtuwmdduis.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.mhx1999.top/gtahjawfjy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ybcxt.top/gtyqrsaoyh.html

TS:   if (s === "") {}
来源：http://hz.yonumen.top/gtcpzkwrww.html

Java: if (s.isEmpty()) {}
来源：http://hz.meibo888.top/gtrlvcyabw.html

Go:   if s == "" {}
来源：http://hz.jyoumei.cn/gtfazownsy.html

Ruby: if s.empty?
来源：http://hz.dianchejie.cn/gtgbpigogj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daxiang520.top/gtbjavgvzc.html

[E21] 超长截断加省略号
来源：http://hz.ydjk.org.cn/gtxitqqazn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenjidiqi.icu/gtsqawztet.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.chenzaomai.com/gtuzexydzw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.meibo888.top/gtemzdseoc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtvrnyiqpn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtrhxdavko.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hongshengwenyu.top/gtfmgngcgz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.iojbl.cn/gtwdarwsow.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xinyue.icu/gtulootycz.html

[E22] 字节长度与字符长度
来源：http://hz.hysaishi.cn/gthqnkdbez.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xuetiantiany.cn/gtjqyplwmu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenjidiqi.icu/gttschxwuc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cheryme.top/gtkzjthsbg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pycfn.com/gtnirxgbpo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jyoumei.cn/gtzkuisiyl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xylfe.cn/gtlcjhfith.html

Ruby: s.bytesize;  s.length
来源：http://hz.gogol.net.cn/gtbongkqwa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.havefunace.top/gtslcqqvlh.html

================================================================================
来源：http://hz.c1oappe.top/gtjpbkihdy.html

F. 文件与目录
来源：http://hz.shuidangran.top/gtbobepqoe.html

================================================================================
来源：http://hz.zycfv.cn/gtbypdivel.html

[F01] 读取整个文件
来源：http://hz.daxiang520.top/gtskekykhe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hysaishi.cn/gtylwizibw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yanxiufei.cn/gtoizmumqi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangdashe.top/gtgzmzsxgn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinyuanbaomall.cn/gtmupsxyrw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtnqqndzrl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yj202588.top/gtntzbwtwe.html

Ruby: File.read("a.txt")
来源：http://hz.guowangkeji.top/gtyubjmvel.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinqigufen.top/gtsqjwuueg.html

[F02] 逐行读取文件
来源：http://hz.hongshengwenyu.top/gtdqztffal.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yonumen.top/gtbhgjdjjk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shzxlz.cn/gtmgyyekfi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sufxvd.cn/gtjrundsws.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hammf.cn/gtxjixlsnv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ehwqpu.com/gtfcnrvtih.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ywan-chungtsiang.top/gtbdzuwggv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.c1oappe.top/gtwybygjxt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yonumen.top/gtbhdzflih.html

[F03] 写入文件（覆盖）
来源：http://hz.yuxming.cn/gtlnsjzcjs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hnqzz.top/gtrnsmpljy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.haohaochexian.top/gthiflurth.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.vqdsnc.cn/gtiwlylmjk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuanzhike.top/gtjblhrpee.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tian-w.cn/gtxoxpexxo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cqqwz.cn/gtpootukni.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinqigfzy.top/gtfbnkdzpa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.chenlongwang.top/gtgrkzszwf.html

[F04] 追加写入文件
来源：http://hz.quarkkingdee.top/gtznjblbtw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhiwuduotai.top/gtbtefkadu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.fzhhl.top/gtyozitmhj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cashguo.top/gtvmgulake.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.dashuyun.cn/gtmdjydlvg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ydjk.org.cn/gtnrpitueb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tianlin.xyz/gtpbwihbdl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ivvv.top/gtevussebq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.aizwys.cn/gtgefmkumd.html

[F05] 判断文件或目录是否存在
来源：http://hz.cashguo.top/gtassuuncd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ybcxt.top/gtyshgktct.html

PHP:  file_exists("a.txt");
来源：http://hz.tian-w.cn/gtirxhapou.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yanxiufei.cn/gtffdyfnez.html

TS:   fs.existsSync("a.txt")
来源：http://hz.dianchejie.cn/gtgtmebxlv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtricnmalr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jqgufenzy.top/gttqvnzmlt.html

Ruby: File.exist?("a.txt")
来源：http://hz.jyoumei.cn/gtinubdkhz.html

C#:   File.Exists("a.txt")
来源：http://hz.smart0.xyz/gtxhziftfs.html

[F06] 删除文件
来源：http://hz.0kj1m.cn/gtcbnuhwcl.html

Py:   os.remove("a.txt")
来源：http://hz.jyoumei.cn/gtmnzcdftb.html

PHP:  unlink("a.txt");
来源：http://hz.xuanzx.com/gtswhyfswv.html


<!-- 参考信息 -->