代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://hz.gotoacloud.top/gtvvoxehct.html

JS:   arr.includes(x)
来源：http://hz.shanyushiyangkeji.top/gtbchdvmib.html

TS:   arr.includes(x)
来源：http://hz.fengsongda.top/gtqgiwkmiu.html

Java: list.contains(x)
来源：http://hz.zhijiandao.cn/gtbgykoucl.html

Go:   slices.Contains(arr, x)
来源：http://hz.ivvv.top/gtvyiujbur.html

Ruby: arr.include?(x)
来源：http://hz.aibaodan.cn/gtowhlaktv.html

C#:   list.Contains(x)
来源：http://hz.0kj1m.cn/gtdzdryldz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yangfankeji.com/gttrpajswr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhoulong.xyz/gthsdsjblw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yj202588.top/gtmgsgmzpe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.mhx1999.top/gtvpfddpun.html

TS:   [...arr];
来源：http://hz.hnxiangtu.top/gtjbaksevy.html

Java: new ArrayList<>(list);
来源：http://hz.redwolf501.top/gthnqjcbor.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.havefunace.top/gtvgcfpcmx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinghuilouyu.cn/gtxkijtffn.html

C#:   new List<int>(list);
来源：http://hz.shanyushiyangkeji.top/gtedrducul.html

[D23] reduce 累积计算
来源：http://hz.aibaodan.cn/gtytkmvyut.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.wangdashe.top/gtaesgpwbg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.dashuyun.cn/gtxobxpcgz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gtfunfcwct.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jlsjyb.cn/gtakehisuh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hysaishi.cn/gtvaoqghlf.html

Go:   // 手写循环
来源：http://hz.cucudq.cn/gtujecjpoy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.fzhhl.top/gtigmohlll.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gzhubu.top/gtanwclmkw.html

[D24] 字典 / Map 基本操作
来源：http://hz.yangfankeji.com/gtjhieflhp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.iojbl.cn/gtfegjcjnu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gzhubu.top/gtzbppgpgn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xinyue.icu/gtgqoacirl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.pengpengdd.cyou/gtvlptamsk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jlsjyb.cn/gtxairwtmh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.chenlongwang.top/gtwxogzzug.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.smart0.xyz/gthanavkkh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.svipenyu.cn/gtxbefiiip.html

[D25] Set 集合去重与交并差
来源：http://hz.gotoacloud.top/gtgkufayzn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.bjfxy.top/gtptqeiqiu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jqgufenzy.top/gtzrbdvomd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.andypj.xyz/gtgjtsnogx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yanxiufei.cn/gtuvdnpawa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhengqikj.top/gtammpdnwl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinqigufen.top/gtgqaicmru.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ppjwa.cn/gtumlopolv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.nanxuanxn.top/gtxkkhgavb.html

[D26] 数组转字符串
来源：http://hz.guannengcc.top/gtquwryocu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.wangdashe.top/gtmvswxuja.html

PHP:  implode(", ", $arr);
来源：http://hz.yongpay.top/gtqletmstu.html

JS:   arr.join(", ")
来源：http://hz.yonumen.top/gtductkprv.html

TS:   arr.join(", ")
来源：http://hz.jqgfzy.top/gtpzrlpana.html

Java: String.join(", ", list)
来源：http://hz.zdqjudy.top/gtcddkfyhq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhiwuduotai.top/gtsgtoizpw.html

Ruby: arr.join(", ")
来源：http://hz.yueranfly.top/gtmipnwlyq.html

C#:   string.Join(", ", list)
来源：http://hz.gotoacloud.top/gtkgoyclfc.html

================================================================================
来源：http://hz.jyoumei.cn/gtftqsvipv.html

E. 字符串处理
来源：http://hz.shanyushiyangtech.top/gtnwxhyhga.html

================================================================================
来源：http://hz.cheryme.top/gtmkahogjh.html

[E01] 拼接字符串
来源：http://hz.kuanghao11.cn/gtwvlrwkfl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hnqzz.top/gtzwduwwao.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sxryk.cn/gtaysvncyy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sweek.top/gtuffotehi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guowangkeji.top/gtobvkjsph.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sufxvd.cn/gtkoviazzw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.haohaochexian.top/gtpfsgfxnd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cucudq.cn/gtlnqzymut.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.316326.xyz/gtagyqqxzb.html

[E02] 重复字符串
来源：http://hz.jinqigufen.top/gtjgcrreis.html

Py:   "ab" * 3
来源：http://hz.mhx1999.top/gtnlsavdrt.html

PHP:  str_repeat("ab", 3);
来源：http://hz.birdmap.top/gtswzvemdm.html

JS:   "ab".repeat(3)
来源：http://hz.ywan-chungtsiang.top/gtzzentcfq.html

TS:   "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtucvostev.html

Java: "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtabptdssa.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tianlin.xyz/gtfguvtpar.html

Ruby: "ab" * 3
来源：http://hz.sxryk.cn/gtxzcybkqr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.aibaodan.cn/gtdfairecf.html

[E03] 截取子串
来源：http://hz.yj202588.top/gtnakplhas.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.mhx1999.top/gtiatfbssf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinqigufen.top/gtdwfosksg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258.top/gtijrbdgju.html

TS:   s.slice(1, 4)
来源：http://hz.kuanghao11.cn/gtzkizekag.html

Java: s.substring(1, 4)
来源：http://hz.ivvv.top/gtkwdtkwyj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinyuanbaomall.cn/gttwlpixig.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.smart0.xyz/gtovaipons.html

C#:   s.Substring(1, 3)
来源：http://hz.xingfuxueyuan.xyz/gtzddteiab.html

[E04] 查找子串位置
来源：http://hz.yanxiufei.cn/gtwywixfpe.html

Py:   s.find("x");  s.index("x")
来源：http://hz.mhx1999.top/gtypcsflkl.html

PHP:  strpos($s, "x");
来源：http://hz.yuxming.cn/gtlfkeiutw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hysaishi.cn/gtdrekhomo.html

TS:   s.indexOf("x")
来源：http://hz.yonumen.top/gtyfmxnoee.html

Java: s.indexOf("x")
来源：http://hz.zhengqikj.top/gthzrhyovu.html

Go:   strings.Index(s, "x")
来源：http://hz.zhongyouzk.top/gtusyxstok.html

Ruby: s.index("x")
来源：http://hz.xingfuxueyuan.xyz/gtdoxolfjr.html

C#:   s.IndexOf("x")
来源：http://hz.cheryme.top/gtlqctlwhl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinqigfzy.top/gtrmdroadz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.c1oappe.top/gtztgzbeco.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shanyushiyangtech.top/gtkdchbkuo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zdqjudy.top/gtplzjzjxv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxinkj.top/gtqcmpuzqb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gthyfsglrt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.guowangkeji.top/gtrjzgqxnr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.fzhhl.top/gtjlsjbqur.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ehwqpu.com/gtidntsezs.html

[E06] 替换子串
来源：http://hz.fzhhl.top/gtzxpwyllf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.shanyushiyangtech.top/gtgoocefwk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cdnleiting.top/gtpvyvpqxv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtcegwvmek.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gtgawyuxlu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangshuangyany.cn/gtzyajwxif.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hfpthk.cn/gtscspqbtt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cheryme.top/gtgipquwpy.html

C#:   s.Replace("a", "b")
来源：http://hz.jianghu66.top/gttbphepdx.html

[E07] 按分隔符拆分
来源：http://hz.cheryme.top/gtlxdewlrp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.smart0.xyz/gtioldaoje.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xuanzx.com/gtoogfigqh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hnqzz.top/gtylelyyyt.html

TS:   s.split(",")
来源：http://hz.cucudq.cn/gtqtoahocg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hfpthk.cn/gtxslrbelq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenzaomai.com/gthqgpbaky.html

Ruby: s.split(",");  s.split
来源：http://hz.zycfv.cn/gtzfwcwtpk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yvedp.cn/gtmiiciwvh.html

[E08] 数组按分隔符合并
来源：http://hz.mhx1999.top/gtrocggaul.html

Py:   ",".join(items)
来源：http://hz.shuidangran.top/gtbfvideoj.html

PHP:  implode(",", $items);
来源：http://hz.yanxiufei.cn/gtmuymcyxo.html

JS:   items.join(",")
来源：http://hz.jiagoushi.top/gtluivkpqg.html

TS:   items.join(",")
来源：http://hz.jiagoushi.top/gtrjofjrtc.html

Java: String.join(",", items)
来源：http://hz.pengpengdd.cyou/gtsknddcyn.html

Go:   strings.Join(items, ",")
来源：http://hz.ydzc1.top/gtvxdvlnjc.html

Ruby: items.join(",")
来源：http://hz.hysaishi.cn/gtddvmziwi.html

C#:   string.Join(",", items)
来源：http://hz.aibaodan.cn/gtfetmltly.html

[E09] 去除所有空白字符
来源：http://hz.ehwqpu.com/gtipvozlmu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.guannengcc.top/gtjaphnivm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shangyingyoupin.top/gtpkdcaqtj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.fengsongda.top/gtzeoxvnhf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ybcxt.top/gthkjxajdp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.vqdsnc.cn/gtfvmywgmm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.redwolf501.top/gtdkmfghbj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ydjk.org.cn/gtfgozjgyo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yongpay.top/gtyyrfiuqx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cashguo.top/gtxbfsdnbt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinqigufen.top/gtkopgbend.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sysykeji.top/gttauaqrqj.html

JS:   "7".padStart(3, "0")
来源：http://hz.bjfxy.top/gthhhggkvi.html

TS:   "7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gtmuqfgjjj.html

Java: String.format("%03d", 7)
来源：http://hz.nwbrower.top/gtixycbjuq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ehwqpu.com/gtkjtmzxqh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.dashuyun.cn/gtwrqbswdq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xylfe.cn/gtxaiiwtts.html

[E11] 反转字符串
来源：http://hz.shzxlz.cn/gtqghtcnzq.html

Py:   s[::-1]
来源：http://hz.smart0.xyz/gtivvhsmme.html

PHP:  strrev($s);
来源：http://hz.yueranfly.top/gtjqdwjvzn.html

JS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtraujrpsq.html

TS:   [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtqhfrbwxa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yvedp.cn/gtmnzuglov.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yueranfly.top/gturxqkjis.html

Ruby: s.reverse
来源：http://hz.hnqzz.top/gtvqschjfg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.tianlin.xyz/gtlwkjfjrb.html

[E12] 统计某字符出现次数
来源：http://hz.shuidangran.top/gtggrfxwqa.html

Py:   s.count("a")
来源：http://hz.ydzc1.top/gtiaxbtfgq.html

PHP:  substr_count($s, "a");
来源：http://hz.xylfe.cn/gtdmyqesbr.html

JS:   s.split("a").length - 1
来源：http://hz.xinyue.icu/gtyxvgtdaj.html

TS:   s.split("a").length - 1
来源：http://hz.yj20258888.top/gtobtwjdua.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yj202588.top/gtujlqfzfz.html

Go:   strings.Count(s, "a")
来源：http://hz.guowangkeji.top/gtyqnauklo.html

Ruby: s.count("a")
来源：http://hz.xylfe.cn/gtqrnamnch.html

C#:   s.Count(c => c == 'a')
来源：http://hz.wangdashe.top/gtawlwqilx.html

[E13] 逐字符遍历
来源：http://hz.daria6918.cn/gtzyhiydzm.html

Py:   for ch in s: print(ch)
来源：http://hz.nwbrower.top/gtgquabbwx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xingfuxueyuan.xyz/gtoipeohun.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangshuangyany.cn/gtbumjwmww.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gotoacloud.top/gtzyicxryd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.52xcode.cn/gtjttkuckp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guannengcc.top/gtpyavzjcy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuxming.cn/gtlfpjrjvy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhixingplan.top/gtotadkfiu.html

[E14] URL 编码与 Base64
来源：http://hz.jinghuilouyu.cn/gtgowuthal.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hfpthk.cn/gtncytcemg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sxryk.cn/gtxxqoctax.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.redwolf501.top/gtwwicoujh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jqgufenzy.top/gtafzzaawf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.daxiang520.top/gtnxgbfqtb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xuetiantiany.cn/gtqedwfnem.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zycfv.cn/gtevfnqlam.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.dashuyun.cn/gtoljjwizq.html

[E15] HTML 转义 / 反转义
来源：http://hz.xuetiantiany.cn/gthvwkapnl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.guannengcc.top/gtmmjgznot.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.meibo888.top/gtliorqegw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hfpthk.cn/gtjnljiphi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shuidangran.top/gtxyotvfvf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.316326.xyz/gthhpskhgy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sweek.top/gtnpkdarzv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.haohaochexian.top/gtxfpmhypt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ehwqpu.com/gtodqdfcgu.html

[E16] 数字千分位
来源：http://hz.yj202588.top/gtvdnojcgr.html

Py:   f"{1234567:,}"
来源：http://hz.snrcjt.cn/gtpntkbykk.html

PHP:  number_format(1234567);
来源：http://hz.ehwqpu.com/gtxrmeoduc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.tanke756.top/gtbsopyyrx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydzc1.top/gtbfeucdgb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ivvv.top/gtgxdxmcae.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nanxuanxn.top/gtiwdzmuya.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.iojbl.cn/gtqugehbhy.html

C#:   1234567.ToString("N0")
来源：http://hz.pycfn.com/gtoeibnafc.html

[E17] 首字母大写
来源：http://hz.ydzc1.top/gtbsfiwoyg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ppjwa.cn/gtnkfysbms.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sufxvd.cn/gtkljdwjzu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cqqwz.cn/gtrsegmcfp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nwbrower.top/gttcxrhrho.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yj202588.top/gtvcwmnvzc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ydjk.org.cn/gtylimtfxv.html

Ruby: s.capitalize
来源：http://hz.smart0.xyz/gtmggbxigm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinqigfzy.top/gtwuahyupy.html

[E18] 模板占位符替换
来源：http://hz.cheryme.top/gthkztcrou.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.quarkkingdee.top/gtqqkrknxj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tian-w.cn/gtrrbpzkii.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.sysykeji.top/gtonjxnlir.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gtwdquiizr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yvedp.cn/gtihqrkldk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinqigufen.top/gtzwmbyxzs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jqgufenzy.top/gtvsxqymap.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.aizwys.cn/gtedupwrtc.html

[E19] 多行文本按行拆分
来源：http://hz.tian-w.cn/gttoiqpfxi.html

Py:   s.splitlines()
来源：http://hz.ydjk.org.cn/gtjhmyexgs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jqgufenzy.top/gtogaewuyz.html

JS:   s.split(/\r?\n/)
来源：http://hz.jqgfzy.top/gtnvtezzkr.html

TS:   s.split(/\r?\n/)
来源：http://hz.jqgufenzy.top/gtwwhwlgiw.html

Java: s.lines().toList()
来源：http://hz.hfpthk.cn/gtzvroobdn.html

Go:   strings.Split(s, "\n")
来源：http://hz.ehwqpu.com/gtcekgdobq.html

Ruby: s.lines
来源：http://hz.pycfn.com/gtndrihcdm.html

C#:   s.Split('\n')
来源：http://hz.wangshuangyany.cn/gtrgklbtdd.html

[E20] 判断字符串是否为空
来源：http://hz.yvedp.cn/gtebjoaeqb.html

Py:   if not s:
来源：http://hz.gotoacloud.top/gtnfdjbmoc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ivvv.top/gtdexkmkem.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.nanxinkj.top/gtlntyqkdp.html

TS:   if (s === "") {}
来源：http://hz.zhengqikj.top/gtldenriux.html

Java: if (s.isEmpty()) {}
来源：http://hz.aizwys.cn/gtgleemcep.html

Go:   if s == "" {}
来源：http://hz.pengpengdd.cyou/gtxsfjxaej.html

Ruby: if s.empty?
来源：http://hz.yonumen.top/gtmdlqwypk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yuxming.cn/gthvuccjoj.html

[E21] 超长截断加省略号
来源：http://hz.shuidangran.top/gtizlitakv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ydjk.org.cn/gtvytxttwd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj20258.top/gtaxhzbogu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtpkaiytta.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gtzcqicfgt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtnihcgsjp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.guannengcc.top/gtoxwkwihq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.fengsongda.top/gtnfbeaift.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yuxming.cn/gtxfweefcj.html

[E22] 字节长度与字符长度
来源：http://hz.ybcxt.top/gtvcxtaxgw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xylfe.cn/gtivtawytu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtzokgdqnw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenlongwang.top/gtkocbatck.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cucudq.cn/gtvdmfnflc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ivvv.top/gtufqwwssn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sufxvd.cn/gtzmecbcuo.html

Ruby: s.bytesize;  s.length
来源：http://hz.pycfn.com/gtlwqhanow.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hfpthk.cn/gtjjewsaag.html

================================================================================
来源：http://hz.yonumen.top/gtzzsepyaq.html

F. 文件与目录
来源：http://hz.shanyushiyangkeji.top/gtmgikhuds.html

================================================================================
来源：http://hz.cashguo.top/gtuzwaycpf.html

[F01] 读取整个文件
来源：http://hz.xziqi.cn/gtznpakhhe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenzaomai.com/gtodxcthjp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhongyouzk.top/gtojpnavqc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.birdmap.top/gtmqidibrx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.dashuyun.cn/gtnsgrvfvp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtjlxxkudx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinqigufen.top/gtifmfzgbl.html

Ruby: File.read("a.txt")
来源：http://hz.shzxlz.cn/gtsbkhqghe.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hammf.cn/gthpmdgtag.html

[F02] 逐行读取文件
来源：http://hz.yj20258888.top/gtuslsojpc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.mhx1999.top/gtkxjrflyx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xuanzx.com/gtkprajijb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.andypj.xyz/gtrznzdtli.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gtpotbomei.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cucudq.cn/gtlupptqph.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xuetiantiany.cn/gtryzzffgf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhijiandao.cn/gtlxwphxcl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ybcxt.top/gtnpampmac.html

[F03] 写入文件（覆盖）
来源：http://hz.jianghu66.top/gtddisqsos.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gzhubu.top/gtseijbgtv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhoulong.xyz/gtrhojdnes.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zdqjudy.top/gtxfgfqdil.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gtszbcihor.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hfpthk.cn/gtekxxsteq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhiwuduotai.top/gtrcdpghhf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhixingplan.top/gtbashddfy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.aizwys.cn/gtzyubywbb.html

[F04] 追加写入文件
来源：http://hz.haohaochexian.top/gtbzwsltas.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuxming.cn/gtuutokvre.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shuidangran.top/gtpldmdezr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ivvv.top/gtsajpzvxq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxuanxn.top/gtepjyglst.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gotoacloud.top/gtuyurnwrh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinyuanbaomall.cn/gtplpcwftw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daria6918.cn/gtpnthirvg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gogol.net.cn/gtjtubmwim.html

[F05] 判断文件或目录是否存在
来源：http://hz.tianlin.xyz/gtomkheene.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ydjk.org.cn/gtxssclvyt.html

PHP:  file_exists("a.txt");
来源：http://hz.yj20258.top/gtsahfeycb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.52xcode.cn/gtsuouvwdl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gtfmjldmxq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtudwwyqwn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.meibo888.top/gtglpvtlsy.html

Ruby: File.exist?("a.txt")
来源：http://hz.quarkkingdee.top/gtrevwrswa.html


<!-- 参考信息 -->