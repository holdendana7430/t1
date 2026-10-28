代发 wailian999

Java: new ArrayList<>(list);
来源：http://hz.zdqjudy.top/gthydeupyw.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xylfe.cn/gtlkjvsdzn.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hammf.cn/gtbdkrpvpa.html

C#:   new List<int>(list);
来源：http://hz.yvedp.cn/gtvgfjvfep.html

[D23] reduce 累积计算
来源：http://hz.ppjwa.cn/gtwiywdkmv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.guannengcc.top/gtqqemrfkj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhengqikj.top/gtepbkhkdl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xziqi.cn/gtqpvbhwkg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258.top/gtbumvxpqy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cheryme.top/gtxpspqguy.html

Go:   // 手写循环
来源：http://hz.hongshengwenyu.top/gtprgqgesf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yvedp.cn/gtkzhcwpkf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gogol.net.cn/gtfdsjlapo.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhongyouzk.top/gtkovvxcli.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jianghu66.top/gtiiorgkoe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jqgfzy.top/gthmllmqfj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.redwolf501.top/gtjkqmeecw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.redwolf501.top/gtcfurumtx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.havefunace.top/gtjqcffkls.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.havefunace.top/gtdwovnduh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.svipenyu.cn/gtvibercuf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zdqjudy.top/gtdbnxlous.html

[D25] Set 集合去重与交并差
来源：http://hz.sweek.top/gtamndtfkl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gaohongyu789.top/gtrsbvmlde.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.iojbl.cn/gtnufsanwg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ivvv.top/gtdphwhegg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cqqwz.cn/gtjcgatirn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hfpthk.cn/gtthmxzmip.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yvedp.cn/gtvxaecgog.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gogol.net.cn/gtpqmcnmjb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.redwolf501.top/gtozoktwgq.html

[D26] 数组转字符串
来源：http://hz.fengsongda.top/gtjgdzmdwn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cdnleiting.top/gtxbrbttzy.html

PHP:  implode(", ", $arr);
来源：http://hz.jinghuilouyu.cn/gtxjgladbc.html

JS:   arr.join(", ")
来源：http://hz.jinyuanbaomall.cn/gtkwwgygrr.html

TS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtxarjdfah.html

Java: String.join(", ", list)
来源：http://hz.gogol.net.cn/gtzzrkbxhl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hysaishi.cn/gtmecqveuy.html

Ruby: arr.join(", ")
来源：http://hz.fengsongda.top/gtlppngatc.html

C#:   string.Join(", ", list)
来源：http://hz.dianchejie.cn/gtwjmjzdxe.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtgubsxrkx.html

E. 字符串处理
来源：http://hz.zhixingplan.top/gtyklouvpz.html

================================================================================
来源：http://hz.gotoacloud.top/gtyfedvkfr.html

[E01] 拼接字符串
来源：http://hz.zhengqikj.top/gtasqgsmbd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yanxiufei.cn/gtnpztgsjo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.snrcjt.cn/gtabjzbhen.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guannengcc.top/gtmsdvrfyy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuxming.cn/gthvzkfxus.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhijiandao.cn/gtmgtcxpcf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.c1oappe.top/gtwjszypcz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sweek.top/gtovneaxaf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtsdsjvxxr.html

[E02] 重复字符串
来源：http://hz.cucudq.cn/gtyaoludni.html

Py:   "ab" * 3
来源：http://hz.hysaishi.cn/gtzsytqafq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ydzc1.top/gtzivwatfi.html

JS:   "ab".repeat(3)
来源：http://hz.smart0.xyz/gtgrcelwsl.html

TS:   "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtvrduqxas.html

Java: "ab".repeat(3)
来源：http://hz.316326.xyz/gtrhzxnmgv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zdqjudy.top/gtpsasmohj.html

Ruby: "ab" * 3
来源：http://hz.hywenlv.cn/gtxxocmdvb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.guannengcc.top/gtvkkzzxkj.html

[E03] 截取子串
来源：http://hz.hnqzz.top/gtwjvoazli.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zycfv.cn/gtpqjinapn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yuxming.cn/gteqnzgpbx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jlsjyb.cn/gtowtcficc.html

TS:   s.slice(1, 4)
来源：http://hz.jlsjyb.cn/gtmncyakmc.html

Java: s.substring(1, 4)
来源：http://hz.chenjidiqi.icu/gtsrbcisaj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ehwqpu.com/gttffsfmkg.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yj202588.top/gtsdwwttnq.html

C#:   s.Substring(1, 3)
来源：http://hz.jianghu66.top/gtvsvhmifu.html

[E04] 查找子串位置
来源：http://hz.ydzc1.top/gtersrlvnx.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yueranfly.top/gtyxgijxjg.html

PHP:  strpos($s, "x");
来源：http://hz.tian-w.cn/gtvbrwldjt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gotoacloud.top/gtspqsogwj.html

TS:   s.indexOf("x")
来源：http://hz.hysaishi.cn/gtxclmhrlm.html

Java: s.indexOf("x")
来源：http://hz.nanxinkj.top/gtcesmqyog.html

Go:   strings.Index(s, "x")
来源：http://hz.aibaodan.cn/gtkkhdtsqr.html

Ruby: s.index("x")
来源：http://hz.quarkkingdee.top/gtmjljakii.html

C#:   s.IndexOf("x")
来源：http://hz.zhiwuduotai.top/gtaftchrmw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yvedp.cn/gtjokoxqri.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.tian-w.cn/gtdtdxgimr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sweek.top/gthjnwoogm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangkeji.top/gthhkxbqqx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhengqikj.top/gtcaktwdky.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hfpthk.cn/gteyrtixle.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cdnleiting.top/gtnykngzlg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cheryme.top/gtmytzqcdy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.redwolf501.top/gtglaycian.html

[E06] 替换子串
来源：http://hz.jinqigufen.top/gtsnvaecrr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jlsjyb.cn/gtrxootqcq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.svipenyu.cn/gtmrklrbml.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtrnkwvcxx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.fzhhl.top/gtmkhkfudy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtsrbqbaty.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jianghu66.top/gtydhmmxhc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xziqi.cn/gtfwsrezbr.html

C#:   s.Replace("a", "b")
来源：http://hz.jyoumei.cn/gtickhbxmq.html

[E07] 按分隔符拆分
来源：http://hz.tian-w.cn/gtdlmvodhz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yuanzhike.top/gtlkiqcsad.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.bjfxy.top/gtdmhuxslt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jinyuanbaomall.cn/gtfoibssiw.html

TS:   s.split(",")
来源：http://hz.tianlin.xyz/gtzpferkep.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jqgfzy.top/gtzqhaczmo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.aibaodan.cn/gtaamkstwz.html

Ruby: s.split(",");  s.split
来源：http://hz.jinghuilouyu.cn/gtpsnstheb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhongyouzk.top/gtkuvkkmrv.html

[E08] 数组按分隔符合并
来源：http://hz.pycfn.com/gthywifwkt.html

Py:   ",".join(items)
来源：http://hz.cdnleiting.top/gtsyrhidcq.html

PHP:  implode(",", $items);
来源：http://hz.hywenlv.cn/gtlfaoyzoj.html

JS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gtqwaxmaol.html

TS:   items.join(",")
来源：http://hz.meibo888.top/gtfjcafssc.html

Java: String.join(",", items)
来源：http://hz.ywan-chungtsiang.top/gtmlnwwukl.html

Go:   strings.Join(items, ",")
来源：http://hz.zhiwuduotai.top/gtvmicvkqs.html

Ruby: items.join(",")
来源：http://hz.chenzaomai.com/gthyvzwnem.html

C#:   string.Join(",", items)
来源：http://hz.zhongyouzk.top/gtgsemmunl.html

[E09] 去除所有空白字符
来源：http://hz.daxiang520.top/gtcpzkabxf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.52xcode.cn/gtaujqmill.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yj20258888.top/gttfigtoqg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yj202588.top/gtoscaxzmk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.wangshuangyany.cn/gtpkocyczt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.fengsongda.top/gtcnwazxih.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj202588.top/gtefwnykwd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.9152youxi.cn/gtfcgslqxr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.9152youxi.cn/gtfragdlcm.html

[E10] 左侧补零 / 定长填充
来源：http://hz.aizwys.cn/gtrunoicxq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.0kj1m.cn/gtlzuokczq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.mhx1999.top/gtwmsddscl.html

JS:   "7".padStart(3, "0")
来源：http://hz.ehwqpu.com/gtanneiuwf.html

TS:   "7".padStart(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtotgererd.html

Java: String.format("%03d", 7)
来源：http://hz.xuanzx.com/gtfjbsjien.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hnxiangtu.top/gtyfnmafbv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.quarkkingdee.top/gtdpnivkcc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhijiandao.cn/gtpuzbcngs.html

[E11] 反转字符串
来源：http://hz.hysaishi.cn/gtoydirjru.html

Py:   s[::-1]
来源：http://hz.aibaodan.cn/gtctgwxeit.html

PHP:  strrev($s);
来源：http://hz.jqgfzy.top/gtmwqhedvu.html

JS:   [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtbwwarylh.html

TS:   [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gtdqupyiyh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.wangshuangyany.cn/gthhweniaf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ybcxt.top/gtwxyjuywm.html

Ruby: s.reverse
来源：http://hz.tian-w.cn/gtfzplrbkh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gtmhcljrym.html

[E12] 统计某字符出现次数
来源：http://hz.nanxuanxn.top/gtnxzbxgxh.html

Py:   s.count("a")
来源：http://hz.cashguo.top/gtbnfkcpax.html

PHP:  substr_count($s, "a");
来源：http://hz.cucudq.cn/gtiwhzfsvo.html

JS:   s.split("a").length - 1
来源：http://hz.yuanzhike.top/gtoforgkap.html

TS:   s.split("a").length - 1
来源：http://hz.guowangkeji.top/gtbpmijguj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yanxiufei.cn/gtrwdwjate.html

Go:   strings.Count(s, "a")
来源：http://hz.cucudq.cn/gtdbqzogyc.html

Ruby: s.count("a")
来源：http://hz.0kj1m.cn/gttgewuxkh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xylfe.cn/gtrvpufekq.html

[E13] 逐字符遍历
来源：http://hz.aibaodan.cn/gtkmevkjqm.html

Py:   for ch in s: print(ch)
来源：http://hz.tian-w.cn/gtwufilaun.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xylfe.cn/gtxobrwtcb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinghuilouyu.cn/gtoujgcghd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.svipenyu.cn/gtsulucnju.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.tanke756.top/gtudktoqrg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.birdmap.top/gtpocnumlb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.haohaochexian.top/gtnnhvywgp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhengqikj.top/gtwdakkynm.html

[E14] URL 编码与 Base64
来源：http://hz.xinyue.icu/gtnycvxlvd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinyuanbaomall.cn/gtohbryeji.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhaomingkeji.xyz/gtgtyljdex.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.pengpengdd.cyou/gtqqcrasbl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenzaomai.com/gttjqeyfml.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangdashe.top/gtxtssdpna.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinqigfzy.top/gttoonabhv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hammf.cn/gtbyawvywl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.meibo888.top/gtcowvzord.html

[E15] HTML 转义 / 反转义
来源：http://hz.shuidangran.top/gthocmibtw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhixingplan.top/gtxdmcgcgx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hnqzz.top/gtdjuzrvfk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.dashuyun.cn/gtvdbbhiyr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.daxiang520.top/gthpmqxqdw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nwbrower.top/gtixifkrbi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yanxiufei.cn/gtrgcicasp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhengqikj.top/gtyivrbsfm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.316326.xyz/gttddohriq.html

[E16] 数字千分位
来源：http://hz.9152youxi.cn/gtyxtgsvez.html

Py:   f"{1234567:,}"
来源：http://hz.redwolf501.top/gtjwpbuyei.html

PHP:  number_format(1234567);
来源：http://hz.aibaodan.cn/gtflgjhlps.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hysaishi.cn/gtmieahcyw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhaomingkeji.xyz/gtfkyspbwa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.cucudq.cn/gthspbikvk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenzaomai.com/gtbhidmncs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hongshengwenyu.top/gtnzfjnvow.html

C#:   1234567.ToString("N0")
来源：http://hz.ehwqpu.com/gtfpyxzbay.html

[E17] 首字母大写
来源：http://hz.zdqjudy.top/gtjwjivlho.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cdnleiting.top/gtkieziuaq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jlsjyb.cn/gttacaqsue.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtbqbmmwdy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.aibaodan.cn/gtiznngwac.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.dianchejie.cn/gtedbfcyjy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.quarkkingdee.top/gtbziabnxb.html

Ruby: s.capitalize
来源：http://hz.fzhhl.top/gtuemtcxxp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.daxiang520.top/gtnjanzdrq.html

[E18] 模板占位符替换
来源：http://hz.yueranfly.top/gtuxjczmpy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.feifeiyinyue.top/gtuyuavicg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yj20258.top/gtxqhxpipz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fengsongda.top/gtavbjfzch.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.9152youxi.cn/gtkhugpmrn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.vqdsnc.cn/gthdnaatrg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hongshengwenyu.top/gthhmyuguu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zycfv.cn/gtfrvuqnzc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.316326.xyz/gtafxrbjbn.html

[E19] 多行文本按行拆分
来源：http://hz.ehwqpu.com/gtspknsjbc.html

Py:   s.splitlines()
来源：http://hz.xuanzx.com/gtlohhsnxr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.fengsongda.top/gthoocpcbh.html

JS:   s.split(/\r?\n/)
来源：http://hz.sysykeji.top/gtcgwhvfkv.html

TS:   s.split(/\r?\n/)
来源：http://hz.hammf.cn/gtzmzdcafi.html

Java: s.lines().toList()
来源：http://hz.ivvv.top/gtykubptqu.html

Go:   strings.Split(s, "\n")
来源：http://hz.ehwqpu.com/gtxbzrfiup.html

Ruby: s.lines
来源：http://hz.cashguo.top/gtkmpllsup.html

C#:   s.Split('\n')
来源：http://hz.wangdashe.top/gturhxtils.html

[E20] 判断字符串是否为空
来源：http://hz.xylfe.cn/gtidonwqns.html

Py:   if not s:
来源：http://hz.tianlin.xyz/gteoidozit.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hnxiangtu.top/gtrgjnrtkz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinqigufen.top/gtzcznqrcs.html

TS:   if (s === "") {}
来源：http://hz.zhiwuduotai.top/gteklotorl.html

Java: if (s.isEmpty()) {}
来源：http://hz.52xcode.cn/gtdgxtvqjl.html

Go:   if s == "" {}
来源：http://hz.yonumen.top/gtacszxnwp.html

Ruby: if s.empty?
来源：http://hz.sysykeji.top/gtzgqlhmve.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cqqwz.cn/gtxgfawmsd.html

[E21] 超长截断加省略号
来源：http://hz.wangshuangyany.cn/gtpmsloqci.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sysykeji.top/gtativnbex.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fengsongda.top/gtnttpnhbd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhiwuduotai.top/gtevmridjh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gtulcvxpyo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtdtdibsgg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nanxuanxn.top/gtyalcdtjh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.fengsongda.top/gtfrsbukvw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ybcxt.top/gtvglouier.html

[E22] 字节长度与字符长度
来源：http://hz.jinqigfzy.top/gtzhpyrnui.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yanxiufei.cn/gtjqquyagp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtxvgtotwp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ppjwa.cn/gtdtetomjs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hfpthk.cn/gtdkdndybq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ivvv.top/gtfsigdqug.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnxiangtu.top/gtdemphsvt.html

Ruby: s.bytesize;  s.length
来源：http://hz.quarkkingdee.top/gtamqemrpn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xuetiantiany.cn/gtybpdvnxh.html

================================================================================
来源：http://hz.ivvv.top/gtoocakrhw.html

F. 文件与目录
来源：http://hz.zhixingplan.top/gtjsfkuvcj.html

================================================================================
来源：http://hz.dashuyun.cn/gtoldgbguo.html

[F01] 读取整个文件
来源：http://hz.jlsjyb.cn/gtlwngdphk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.snrcjt.cn/gtfwanjhhn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gzhubu.top/gtulmedlwn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinghuilouyu.cn/gtbacipkub.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj202588.top/gtygewmwho.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtwfrlfcvc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.mhx1999.top/gtrheiaoaj.html

Ruby: File.read("a.txt")
来源：http://hz.zhongyouzk.top/gtrtgafrri.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj202588.top/gttnmrtube.html

[F02] 逐行读取文件
来源：http://hz.c1oappe.top/gtvytgxdjm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.haohaochexian.top/gtmdpclgte.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.birdmap.top/gtymmrzotl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shangyingyoupin.top/gtsjbjqyma.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tian-w.cn/gtbmjkmrpx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.redwolf501.top/gtvporxhlp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.kuanghao11.cn/gtllgggnre.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.kuanghao11.cn/gtbvfvhyvu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.aizwys.cn/gtjeesdsof.html

[F03] 写入文件（覆盖）
来源：http://hz.xziqi.cn/gtzfknunbp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hammf.cn/gtsgxawvsm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cqqwz.cn/gtzguqcehd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.aibaodan.cn/gtxbdtjobs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jiagoushi.top/gtkvkhxxlw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aizwys.cn/gtkuklrhhg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ybcxt.top/gtprdekxko.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yangfankeji.com/gtjqbqznti.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.quarkkingdee.top/gtsggmxybw.html

[F04] 追加写入文件
来源：http://hz.jinqigfzy.top/gtkroxplrc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhengqikj.top/gtoidlznno.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.aibaodan.cn/gtaigpxjzq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigufen.top/gtzweuumaj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuetiantiany.cn/gtvsnegkpw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ydzc1.top/gttfhxmpnq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yongpay.top/gtdtezldmg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jqgufenzy.top/gtuawjvabb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.aibaodan.cn/gtwfkjzluk.html

[F05] 判断文件或目录是否存在
来源：http://hz.yongpay.top/gtjkpgvjuz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jiagoushi.top/gtcjdjsgsh.html

PHP:  file_exists("a.txt");
来源：http://hz.smart0.xyz/gtxyhzahrv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.dashuyun.cn/gtdnhxykct.html

TS:   fs.existsSync("a.txt")
来源：http://hz.smart0.xyz/gtbspomjcn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtfnldzbgl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nwbrower.top/gtnusdbcrm.html

Ruby: File.exist?("a.txt")
来源：http://hz.shanyushiyangtech.top/gtsehtmabx.html

C#:   File.Exists("a.txt")
来源：http://hz.ivvv.top/gtdrjhfpgl.html

[F06] 删除文件
来源：http://hz.jiagoushi.top/gtfhqfgzrc.html

Py:   os.remove("a.txt")
来源：http://hz.wangdashe.top/gtaadusxci.html

PHP:  unlink("a.txt");
来源：http://hz.xinyue.icu/gtvvwsqzsd.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtnwbcrgxj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gteqmqchgw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtrrowkpiw.html

Go:   os.Remove("a.txt")
来源：http://hz.jqgfzy.top/gthihjfdkw.html

Ruby: File.delete("a.txt")
来源：http://hz.zhiwuduotai.top/gtzzlwelxj.html

C#:   File.Delete("a.txt");
来源：http://hz.xinyue.icu/gtesuzrlwt.html

[F07] 创建目录（含多级）
来源：http://hz.52xcode.cn/gtnlppqatl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhixingplan.top/gtzptkqzif.html


<!-- 参考信息 -->