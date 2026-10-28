代发 wailian999

Java: new ArrayList<>(list);
来源：http://hz.svipenyu.cn/gtwaahctqb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yvedp.cn/gtusxcvnjj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.52xcode.cn/gtokcgmmgu.html

C#:   new List<int>(list);
来源：http://hz.fzhhl.top/gtibjdlcfv.html

[D23] reduce 累积计算
来源：http://hz.xinyue.icu/gtqgpxdcuy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ppjwa.cn/gtrrppqqod.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.feifeiyinyue.top/gtykaohzeu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258888.top/gtlekjyjof.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgufenzy.top/gtyuxwytjn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shanyushiyangtech.top/gtvfmpsvcu.html

Go:   // 手写循环
来源：http://hz.hammf.cn/gtwwvnalew.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhengqikj.top/gtmvoovhzo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.svipenyu.cn/gtehpzwndo.html

[D24] 字典 / Map 基本操作
来源：http://hz.quarkkingdee.top/gtjakpsuuh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhixingplan.top/gtididnyrf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.0kj1m.cn/gtdpxnolxz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cucudq.cn/gtpyohjtsn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xylfe.cn/gtnekftoan.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cheryme.top/gtjqdwvjoj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.tian-w.cn/gttumvxqrv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jyoumei.cn/gtidoyitqe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shanyushiyangkeji.top/gtvdwxjtmf.html

[D25] Set 集合去重与交并差
来源：http://hz.yanxiufei.cn/gtjsqgpaex.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.birdmap.top/gtqthlycri.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.fzhhl.top/gtezalnfpi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.daxiang520.top/gtbcrfdeud.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.snrcjt.cn/gtadvbmtos.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.havefunace.top/gthqqpuctq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jianghu66.top/gtdqlrjxyq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gotoacloud.top/gthfrgwbfz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xinyue.icu/gtwoiqsnuc.html

[D26] 数组转字符串
来源：http://hz.hysaishi.cn/gtmwuejkxg.html

Py:   ", ".join(map(str, arr))
来源：http://hz.fzhhl.top/gthgesoteq.html

PHP:  implode(", ", $arr);
来源：http://hz.shanyushiyangtech.top/gtofasnvvz.html

JS:   arr.join(", ")
来源：http://hz.gogol.net.cn/gtkveglgsu.html

TS:   arr.join(", ")
来源：http://hz.ydjk.org.cn/gtujjditex.html

Java: String.join(", ", list)
来源：http://hz.wangdashe.top/gttodbsras.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cqqwz.cn/gtrtdwizkj.html

Ruby: arr.join(", ")
来源：http://hz.cdnleiting.top/gtdtvuoyhk.html

C#:   string.Join(", ", list)
来源：http://hz.ehwqpu.com/gthfuwlzrx.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtchxnchwp.html

E. 字符串处理
来源：http://hz.jinqigufen.top/gtaklsudqb.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtsnvbghaf.html

[E01] 拼接字符串
来源：http://hz.yj20258888.top/gtapaerbha.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yanxiufei.cn/gtlkfrbroo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gzhubu.top/gtgfcgqbhi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fengsongda.top/gtxpuaijrw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gtwzihdkct.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shzxlz.cn/gtbxjuubmx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.fzhhl.top/gtdawhnstm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.birdmap.top/gtrogspsve.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.wangshuangyany.cn/gtaobiorpo.html

[E02] 重复字符串
来源：http://hz.quarkkingdee.top/gtaqxxbcrm.html

Py:   "ab" * 3
来源：http://hz.jianghu66.top/gtvttiigxu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenlongwang.top/gtmvowyabr.html

JS:   "ab".repeat(3)
来源：http://hz.shuidangran.top/gtbpgvhqxa.html

TS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gtltbmquzg.html

Java: "ab".repeat(3)
来源：http://hz.hnqzz.top/gtgzhbihkh.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.quarkkingdee.top/gtagxgrijs.html

Ruby: "ab" * 3
来源：http://hz.jqgfzy.top/gtkfslbhzt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.smart0.xyz/gtllddmoxh.html

[E03] 截取子串
来源：http://hz.jianghu66.top/gtigqhxyem.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hnqzz.top/gtqlqxquqy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gzhubu.top/gtwcceefgw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.haohaochexian.top/gtfzemurdt.html

TS:   s.slice(1, 4)
来源：http://hz.sweek.top/gtqqsqdwxb.html

Java: s.substring(1, 4)
来源：http://hz.cqqwz.cn/gtfmousiay.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cashguo.top/gtxhpfoucm.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinqigufen.top/gtwefufreo.html

C#:   s.Substring(1, 3)
来源：http://hz.yonumen.top/gtprqcyhgu.html

[E04] 查找子串位置
来源：http://hz.bjfxy.top/gtyathquar.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ydzc1.top/gtiqndznsm.html

PHP:  strpos($s, "x");
来源：http://hz.hnxiangtu.top/gtlrtuxkjq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.svipenyu.cn/gtuawmoknl.html

TS:   s.indexOf("x")
来源：http://hz.ydzc1.top/gtihyzhzyn.html

Java: s.indexOf("x")
来源：http://hz.nanxinkj.top/gtunuhfbzc.html

Go:   strings.Index(s, "x")
来源：http://hz.jinyuanbaomall.cn/gtorahrdtv.html

Ruby: s.index("x")
来源：http://hz.nwbrower.top/gtrbggogkd.html

C#:   s.IndexOf("x")
来源：http://hz.0kj1m.cn/gtevgmfasw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xziqi.cn/gtqmvapjgh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhiwuduotai.top/gtbzgvmnck.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.smart0.xyz/gtoysvpuwo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhiwuduotai.top/gtdlebgzcu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.fengsongda.top/gtbsotuhvp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.feifeiyinyue.top/gtxcbsfmqj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.0kj1m.cn/gtxjmyepgy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cheryme.top/gtizvlqlpw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.birdmap.top/gtrixmblhb.html

[E06] 替换子串
来源：http://hz.guannengcc.top/gtcqnsnzbx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jlsjyb.cn/gtvdmkhgen.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.guowangkeji.top/gtlbwakyzg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtjfxorkuu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ydjk.org.cn/gtvlycjbkz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtvwfwyayf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cashguo.top/gtpqxeslqy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zdqjudy.top/gtzocenxat.html

C#:   s.Replace("a", "b")
来源：http://hz.fengsongda.top/gtpybxsjkz.html

[E07] 按分隔符拆分
来源：http://hz.sweek.top/gtqzszqhkw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cdnleiting.top/gtxylsuxws.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.redwolf501.top/gtqgnbxzcr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.svipenyu.cn/gtghlnldcw.html

TS:   s.split(",")
来源：http://hz.zhixingplan.top/gtgolyejyc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yanxiufei.cn/gtfiyrqkla.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.vqdsnc.cn/gtwxafqwft.html

Ruby: s.split(",");  s.split
来源：http://hz.cashguo.top/gtqxmtwrwf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cdnleiting.top/gtnnpuksne.html

[E08] 数组按分隔符合并
来源：http://hz.nanxinkj.top/gtlnytyxgj.html

Py:   ",".join(items)
来源：http://hz.cqqwz.cn/gtfmcltypw.html

PHP:  implode(",", $items);
来源：http://hz.chenzaomai.com/gtfqexnpnu.html

JS:   items.join(",")
来源：http://hz.jinyuanbaomall.cn/gtonabinap.html

TS:   items.join(",")
来源：http://hz.quarkkingdee.top/gtuyykkany.html

Java: String.join(",", items)
来源：http://hz.shangyingyoupin.top/gtbadgofhy.html

Go:   strings.Join(items, ",")
来源：http://hz.jiagoushi.top/gtrhncuxwl.html

Ruby: items.join(",")
来源：http://hz.hysaishi.cn/gtislkjbva.html

C#:   string.Join(",", items)
来源：http://hz.sysykeji.top/gtpqthycrl.html

[E09] 去除所有空白字符
来源：http://hz.zhoulong.xyz/gtiupomyyb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.dianchejie.cn/gthngkiuqr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sxryk.cn/gtophfbpbv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.aizwys.cn/gtvgaaimui.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tanke756.top/gtilsfhscf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ydjk.org.cn/gtpfpamtew.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.nanxinkj.top/gtqmbuwrua.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shangyingyoupin.top/gtescgszvf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.chenlongwang.top/gtkwybobrv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ybcxt.top/gtssukvsjx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cqqwz.cn/gtpdxzswnk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sweek.top/gthjesluqf.html

JS:   "7".padStart(3, "0")
来源：http://hz.shangyingyoupin.top/gtwdcxwgse.html

TS:   "7".padStart(3, "0")
来源：http://hz.jqgfzy.top/gttrfpjhoo.html

Java: String.format("%03d", 7)
来源：http://hz.jyoumei.cn/gtqazleyif.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtlfoxgvdr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.fzhhl.top/gtrmnxvcmn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hammf.cn/gtrckbgzyg.html

[E11] 反转字符串
来源：http://hz.mhx1999.top/gtonbzkcrq.html

Py:   s[::-1]
来源：http://hz.zhijiandao.cn/gtvznyvknu.html

PHP:  strrev($s);
来源：http://hz.ydzc1.top/gtiksllyqj.html

JS:   [...s].reverse().join("")
来源：http://hz.ybcxt.top/gtdqqxfnja.html

TS:   [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtgybztmpd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.havefunace.top/gtwnchudji.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yangfankeji.com/gteaegfxyj.html

Ruby: s.reverse
来源：http://hz.yj202588.top/gtazdlocxz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yangfankeji.com/gtkvzydzdg.html

[E12] 统计某字符出现次数
来源：http://hz.pengpengdd.cyou/gtatbwdded.html

Py:   s.count("a")
来源：http://hz.jinqigfzy.top/gtgoqcbtjg.html

PHP:  substr_count($s, "a");
来源：http://hz.9152youxi.cn/gtjhcfseoo.html

JS:   s.split("a").length - 1
来源：http://hz.hysaishi.cn/gtkabgdatt.html

TS:   s.split("a").length - 1
来源：http://hz.cashguo.top/gthezpyghw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cheryme.top/gtotuaiuab.html

Go:   strings.Count(s, "a")
来源：http://hz.chenzaomai.com/gtugqkjltj.html

Ruby: s.count("a")
来源：http://hz.yangfankeji.com/gtvzgdrzzk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cqqwz.cn/gtfhfbjmkj.html

[E13] 逐字符遍历
来源：http://hz.zhiwuduotai.top/gtetxqvmpx.html

Py:   for ch in s: print(ch)
来源：http://hz.shangyingyoupin.top/gtiqsouisj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.dianchejie.cn/gtqirvzqqh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yvedp.cn/gtiyuqyknx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.birdmap.top/gtdbguksvl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.feifeiyinyue.top/gtmjhnuyae.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cdnleiting.top/gtqahsyapg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xinyue.icu/gtjrzttdoz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tanke756.top/gtsqpoywpq.html

[E14] URL 编码与 Base64
来源：http://hz.ivvv.top/gtmgcllboq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.pycfn.com/gtrthfznpp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhengqikj.top/gtvelnjkit.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.0kj1m.cn/gtvypldisf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cheryme.top/gtoquyajrp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jiagoushi.top/gtxpnrtcsw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tanke756.top/gtkrudtgpa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.havefunace.top/gtbpumxbbg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.wangshuangyany.cn/gtbjyjrxoq.html

[E15] HTML 转义 / 反转义
来源：http://hz.svipenyu.cn/gtvcitzkuf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ybcxt.top/gtzeedguwg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.iojbl.cn/gthroubpzp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ydzc1.top/gtdzhtyunu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ydzc1.top/gtftiucjvp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sufxvd.cn/gtfolatyoj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinqigufen.top/gtyvmxbzjh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.dianchejie.cn/gtnddtziqf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yanxiufei.cn/gttezyarmv.html

[E16] 数字千分位
来源：http://hz.xuetiantiany.cn/gtxtyasldd.html

Py:   f"{1234567:,}"
来源：http://hz.ybcxt.top/gthksbqxfg.html

PHP:  number_format(1234567);
来源：http://hz.cheryme.top/gtqxezcjbw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jiagoushi.top/gtnpkaxkyn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.dashuyun.cn/gthjpfcugc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shanyushiyangtech.top/gtlwmewniw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.haohaochexian.top/gtftgmfiuc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ppjwa.cn/gtqhgudcwp.html

C#:   1234567.ToString("N0")
来源：http://hz.zhiwuduotai.top/gtlczzlruk.html

[E17] 首字母大写
来源：http://hz.guowangkeji.top/gtiqqgenda.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hnxiangtu.top/gtxrklryek.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yongpay.top/gtzkmnhndf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.redwolf501.top/gtsputlwwc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.smart0.xyz/gtlhjpgong.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenjidiqi.icu/gtswzuqswi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cheryme.top/gturhpcjkx.html

Ruby: s.capitalize
来源：http://hz.zhoulong.xyz/gtkdlzvgvf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shuidangran.top/gtqdklgafa.html

[E18] 模板占位符替换
来源：http://hz.ydjk.org.cn/gtmzxvsnxk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhengqikj.top/gtvtpeqmqh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jlsjyb.cn/gtznzrzwwr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.redwolf501.top/gtbnwbiwat.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.havefunace.top/gtwcsbkspd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.9152youxi.cn/gtlygsszwf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj20258888.top/gtghdgarzu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xylfe.cn/gtckqotlpb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yvedp.cn/gthrxfzpir.html

[E19] 多行文本按行拆分
来源：http://hz.zhixingplan.top/gtihmgapsb.html

Py:   s.splitlines()
来源：http://hz.bjfxy.top/gtbqnipdno.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zdqjudy.top/gtfxdgxsrw.html

JS:   s.split(/\r?\n/)
来源：http://hz.yvedp.cn/gtxjdxowyz.html

TS:   s.split(/\r?\n/)
来源：http://hz.xuanzx.com/gthxuyowrk.html

Java: s.lines().toList()
来源：http://hz.xuetiantiany.cn/gtckpeozir.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhoulong.xyz/gtfjyerlzn.html

Ruby: s.lines
来源：http://hz.chenlongwang.top/gtguujerku.html

C#:   s.Split('\n')
来源：http://hz.shzxlz.cn/gtckmbnmlx.html

[E20] 判断字符串是否为空
来源：http://hz.shzxlz.cn/gtdaikdlgs.html

Py:   if not s:
来源：http://hz.chenjidiqi.icu/gtlrxfplsd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ehwqpu.com/gtmsorxkjx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.daria6918.cn/gtxzgurupp.html

TS:   if (s === "") {}
来源：http://hz.xuetiantiany.cn/gteeqdfnba.html

Java: if (s.isEmpty()) {}
来源：http://hz.gotoacloud.top/gtliuucpvl.html

Go:   if s == "" {}
来源：http://hz.zhiwuduotai.top/gtykrtzdrb.html

Ruby: if s.empty?
来源：http://hz.kuanghao11.cn/gtcnwhfhzf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shanyushiyangtech.top/gtbntdzjbn.html

[E21] 超长截断加省略号
来源：http://hz.smart0.xyz/gtrtlpauck.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.dianchejie.cn/gtwljneanx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.mhx1999.top/gtgnqapjuw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtvdylaqic.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtkdtpredo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtchfsxuca.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ydjk.org.cn/gtqinauerw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ppjwa.cn/gtvjvmknfl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shanyushiyangtech.top/gtlucptmwb.html

[E22] 字节长度与字符长度
来源：http://hz.zhongyouzk.top/gtkzskwgxa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gzhubu.top/gttgjfknbq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gaohongyu789.top/gtwveykagy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenlongwang.top/gtxztctwdf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.52xcode.cn/gtudcmcbbt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.quarkkingdee.top/gtghxalurl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shanyushiyangtech.top/gtgbgssang.html

Ruby: s.bytesize;  s.length
来源：http://hz.cdnleiting.top/gtxpkqucra.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.dianchejie.cn/gtsgebqbsl.html

================================================================================
来源：http://hz.cheryme.top/gtbeonfroc.html

F. 文件与目录
来源：http://hz.xingfuxueyuan.xyz/gtuhepvxut.html

================================================================================
来源：http://hz.yangfankeji.com/gtpkrzqsqq.html

[F01] 读取整个文件
来源：http://hz.hongshengwenyu.top/gtdwpvlkme.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cheryme.top/gtabotcmri.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tian-w.cn/gtdjqaykdg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.vqdsnc.cn/gtbhrfdrwq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.andypj.xyz/gtfoyxtcpm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtfnffsvym.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yuanzhike.top/gtluqqkicr.html

Ruby: File.read("a.txt")
来源：http://hz.52xcode.cn/gtpqflixps.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gaohongyu789.top/gtpsrjrzmj.html

[F02] 逐行读取文件
来源：http://hz.cdnleiting.top/gtplyjxwni.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cucudq.cn/gtbxlsbuuh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenzaomai.com/gtdbyalchb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gtmpnagckl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cheryme.top/gtfckxdvhg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hongshengwenyu.top/gtwrfhmdic.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.316326.xyz/gtzmtawrwi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhengqikj.top/gtstgyvdyv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xingfuxueyuan.xyz/gtupmgfmmv.html

[F03] 写入文件（覆盖）
来源：http://hz.zhongyouzk.top/gtzekmepft.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhijiandao.cn/gtigftwrnt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhoulong.xyz/gttoqvexiz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yangfankeji.com/gtzilzhmkh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nwbrower.top/gtmtuudmhy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.kuanghao11.cn/gtpzwmraba.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.daxiang520.top/gtycwihlwn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gzhubu.top/gtvjblnxsc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nanxuanxn.top/gtjqjwckee.html

[F04] 追加写入文件
来源：http://hz.dianchejie.cn/gtedychlsf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.vqdsnc.cn/gtbiwimbhx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhongyouzk.top/gtpqjldjam.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tianlin.xyz/gtbkcquegq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gtqpewotme.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xylfe.cn/gtpnwvxgxd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.9152youxi.cn/gtfzcsiepv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.snrcjt.cn/gtmhsnidkq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenjidiqi.icu/gtwlbiqzvz.html

[F05] 判断文件或目录是否存在
来源：http://hz.hfpthk.cn/gttjxgfsmf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yongpay.top/gtgcpqmwwn.html

PHP:  file_exists("a.txt");
来源：http://hz.gogol.net.cn/gtxnlxoejy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.aibaodan.cn/gtpforyxtr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinqigufen.top/gtffyklkps.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtlgkszuah.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xylfe.cn/gtzkmtltfy.html

Ruby: File.exist?("a.txt")
来源：http://hz.c1oappe.top/gtchkoytbh.html

C#:   File.Exists("a.txt")
来源：http://hz.snrcjt.cn/gtlpxzevui.html

[F06] 删除文件
来源：http://hz.dianchejie.cn/gtpdizfgqj.html

Py:   os.remove("a.txt")
来源：http://hz.meibo888.top/gthzbfbakk.html

PHP:  unlink("a.txt");
来源：http://hz.shanyushiyangtech.top/gtrqotwjgq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.iojbl.cn/gtfcbpdyps.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tian-w.cn/gtioezuhay.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtucukbyem.html

Go:   os.Remove("a.txt")
来源：http://hz.svipenyu.cn/gtgczzmwan.html

Ruby: File.delete("a.txt")
来源：http://hz.fengsongda.top/gtkkktcwuv.html

C#:   File.Delete("a.txt");
来源：http://hz.jqgfzy.top/gtccibnlac.html

[F07] 创建目录（含多级）
来源：http://hz.hnxiangtu.top/gtlmbwlzva.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.dianchejie.cn/gtkdwvpqql.html


<!-- 参考信息 -->