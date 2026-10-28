代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258888.top/gtuzkysnqj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.feifeiyinyue.top/gtyuujjaki.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jqgfzy.top/gtxampknwj.html

Go:   // 手写 map[T]int
来源：http://hz.redwolf501.top/gtcclwthrh.html

Ruby: arr.tally
来源：http://hz.c1oappe.top/gtqjnjcrew.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.pengpengdd.cyou/gtociglvno.html

[D21] 判断是否包含某元素
来源：http://hz.zhengqikj.top/gtttsftemk.html

Py:   x in arr
来源：http://hz.ppjwa.cn/gtpqnabgyx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.mhx1999.top/gtswcomnps.html

JS:   arr.includes(x)
来源：http://hz.ydjk.org.cn/gtasviqemg.html

TS:   arr.includes(x)
来源：http://hz.aizwys.cn/gtzsrqdygy.html

Java: list.contains(x)
来源：http://hz.aibaodan.cn/gtkkrqhjds.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinqigfzy.top/gteikqxwwg.html

Ruby: arr.include?(x)
来源：http://hz.mhx1999.top/gtglfwcszq.html

C#:   list.Contains(x)
来源：http://hz.ydjk.org.cn/gtuizoilob.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinghuilouyu.cn/gtggducsri.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hammf.cn/gtetlknfvh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangkeji.top/gtjyzgfvcv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xylfe.cn/gtybshoier.html

TS:   [...arr];
来源：http://hz.c1oappe.top/gtvhiacasz.html

Java: new ArrayList<>(list);
来源：http://hz.snrcjt.cn/gtfliokocy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.birdmap.top/gtagphqbta.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shangyingyoupin.top/gtfsihnngq.html

C#:   new List<int>(list);
来源：http://hz.xingfuxueyuan.xyz/gtvkkdrqhg.html

[D23] reduce 累积计算
来源：http://hz.zhiwuduotai.top/gthilqzlzv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.c1oappe.top/gteqcstfxm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.dashuyun.cn/gtqldxbcge.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.snrcjt.cn/gtlewnjeem.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.dashuyun.cn/gtvtlnvrlg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nanxuanxn.top/gtediqqrzp.html

Go:   // 手写循环
来源：http://hz.vqdsnc.cn/gtpvyzqttp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jqgufenzy.top/gtixvjwakx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.0kj1m.cn/gtizbakjow.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhixingplan.top/gtkrpyxcef.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shuidangran.top/gttqmvewtt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.smart0.xyz/gtndadzvlu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sysykeji.top/gtvbtdrxzw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.daxiang520.top/gtjifygznx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hnqzz.top/gtpowssgdv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ppjwa.cn/gtnqzfeuww.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cdnleiting.top/gthrgamxuu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yangfankeji.com/gtwhfiwvxr.html

[D25] Set 集合去重与交并差
来源：http://hz.sufxvd.cn/gtvqxnwkel.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhiwuduotai.top/gtdqlodtlt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cheryme.top/gtofjplfor.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hongshengwenyu.top/gtossolehw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.vqdsnc.cn/gtmyogovuh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shangyingyoupin.top/gtihewpxuh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.fengsongda.top/gtppdgmabt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhengqikj.top/gtohceqjqp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jiagoushi.top/gtlrsdvjap.html

[D26] 数组转字符串
来源：http://hz.sysykeji.top/gtbvuvsfuo.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hysaishi.cn/gtayrzhguv.html

PHP:  implode(", ", $arr);
来源：http://hz.sysykeji.top/gtlylwogoc.html

JS:   arr.join(", ")
来源：http://hz.hnxiangtu.top/gtbynzxrtx.html

TS:   arr.join(", ")
来源：http://hz.tian-w.cn/gtlonziluv.html

Java: String.join(", ", list)
来源：http://hz.pengpengdd.cyou/gtcbdvypep.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jiagoushi.top/gtheaxtquy.html

Ruby: arr.join(", ")
来源：http://hz.yuanzhike.top/gtpeieubml.html

C#:   string.Join(", ", list)
来源：http://hz.pycfn.com/gtrhfjtwuw.html

================================================================================
来源：http://hz.xylfe.cn/gtckclukjq.html

E. 字符串处理
来源：http://hz.ydjk.org.cn/gtiqpbwaer.html

================================================================================
来源：http://hz.daria6918.cn/gtjutdifrq.html

[E01] 拼接字符串
来源：http://hz.kuanghao11.cn/gtpethxbkv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dashuyun.cn/gtuzhbghie.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhiwuduotai.top/gtmejnpmki.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hywenlv.cn/gtzobgbzwj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258888.top/gtpmyhagor.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sufxvd.cn/gtdkfljzok.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.feifeiyinyue.top/gtqroblsxu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zycfv.cn/gtgkirgnro.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yueranfly.top/gthyvvrdqk.html

[E02] 重复字符串
来源：http://hz.pycfn.com/gtninezfxz.html

Py:   "ab" * 3
来源：http://hz.jyoumei.cn/gtltbmkjjl.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sufxvd.cn/gtwdxznrhk.html

JS:   "ab".repeat(3)
来源：http://hz.shanyushiyangkeji.top/gtmobhojpa.html

TS:   "ab".repeat(3)
来源：http://hz.andypj.xyz/gtkkrppjbg.html

Java: "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtdtlkydnl.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.gaohongyu789.top/gtcdyvejpv.html

Ruby: "ab" * 3
来源：http://hz.hysaishi.cn/gthuayfzjz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shanyushiyangkeji.top/gtgrnqatas.html

[E03] 截取子串
来源：http://hz.zhiwuduotai.top/gtgepczbhb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zycfv.cn/gtvaxcabtc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gotoacloud.top/gtyqzksjcu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ivvv.top/gtkwspvmku.html

TS:   s.slice(1, 4)
来源：http://hz.xingfuxueyuan.xyz/gtoqfhmefo.html

Java: s.substring(1, 4)
来源：http://hz.jyoumei.cn/gtgpfrrjay.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.guannengcc.top/gtiauuzzks.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.9152youxi.cn/gtbiuvtjnt.html

C#:   s.Substring(1, 3)
来源：http://hz.yueranfly.top/gtkviwxmnq.html

[E04] 查找子串位置
来源：http://hz.hammf.cn/gtmvnpraac.html

Py:   s.find("x");  s.index("x")
来源：http://hz.guannengcc.top/gtikyzbtpo.html

PHP:  strpos($s, "x");
来源：http://hz.quarkkingdee.top/gtvrgjrqsl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hnxiangtu.top/gtvlyiqqup.html

TS:   s.indexOf("x")
来源：http://hz.cheryme.top/gtvznfyzmv.html

Java: s.indexOf("x")
来源：http://hz.daxiang520.top/gtecbkcqax.html

Go:   strings.Index(s, "x")
来源：http://hz.yanxiufei.cn/gtvgcagutx.html

Ruby: s.index("x")
来源：http://hz.shanyushiyangkeji.top/gtmjdihqdn.html

C#:   s.IndexOf("x")
来源：http://hz.shzxlz.cn/gtpbowkjsl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.shanyushiyangtech.top/gtxefyarzm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xuanzx.com/gtrmdwumbg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhaomingkeji.xyz/gtfzcmofce.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangkeji.top/gtzbyxvrna.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yongpay.top/gtfevfyfge.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigfzy.top/gttlrkcgxw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shzxlz.cn/gteygqhwvv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.quarkkingdee.top/gtvfaqmyqm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.aibaodan.cn/gtiyhnhcfj.html

[E06] 替换子串
来源：http://hz.hongshengwenyu.top/gthryvgbpt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.wangdashe.top/gtrfmzqurp.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yj20258.top/gtnehptbui.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtzvywyqof.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtfdkeopvt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtnywzftbn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ywan-chungtsiang.top/gtofqdpzsn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ivvv.top/gtcfpoqegi.html

C#:   s.Replace("a", "b")
来源：http://hz.hfpthk.cn/gtyzzozpou.html

[E07] 按分隔符拆分
来源：http://hz.zhongyouzk.top/gtrkkkpgmt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hywenlv.cn/gtdwxhihtk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.vqdsnc.cn/gtfhyewzew.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.daxiang520.top/gtcpawixlh.html

TS:   s.split(",")
来源：http://hz.jinyuanbaomall.cn/gtnheqxvgl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cqqwz.cn/gtfsufieuw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.redwolf501.top/gtiayznqha.html

Ruby: s.split(",");  s.split
来源：http://hz.tanke756.top/gtxqisjjpx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.andypj.xyz/gtekcoinor.html

[E08] 数组按分隔符合并
来源：http://hz.jqgufenzy.top/gtvwxtzphc.html

Py:   ",".join(items)
来源：http://hz.meibo888.top/gtptpzlrwf.html

PHP:  implode(",", $items);
来源：http://hz.hnqzz.top/gtwxblcino.html

JS:   items.join(",")
来源：http://hz.haohaochexian.top/gtcbgbxwaf.html

TS:   items.join(",")
来源：http://hz.xinyue.icu/gtddjesill.html

Java: String.join(",", items)
来源：http://hz.hongshengwenyu.top/gtyfpodvdb.html

Go:   strings.Join(items, ",")
来源：http://hz.tianlin.xyz/gtiuxktjsn.html

Ruby: items.join(",")
来源：http://hz.quarkkingdee.top/gtbympoqqy.html

C#:   string.Join(",", items)
来源：http://hz.xinyue.icu/gtqaetoscc.html

[E09] 去除所有空白字符
来源：http://hz.zhengqikj.top/gtqciupeba.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jyoumei.cn/gtengkrqno.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.9152youxi.cn/gtflohkjgm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.pengpengdd.cyou/gtjuevhoid.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zdqjudy.top/gtkowjlsyz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tian-w.cn/gtgejlqqnb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhengqikj.top/gtnzgazhah.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yj20258.top/gtsswxkufw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hongshengwenyu.top/gtavzrdhgn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hywenlv.cn/gtlctupiob.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tianlin.xyz/gtqcvsivnf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sxryk.cn/gttubzisvq.html

JS:   "7".padStart(3, "0")
来源：http://hz.jiagoushi.top/gtilcyyueo.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinqigfzy.top/gtxxupewrb.html

Java: String.format("%03d", 7)
来源：http://hz.andypj.xyz/gtgrdfdxqt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhiwuduotai.top/gtgtztgilt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.c1oappe.top/gtctqycnxs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jlsjyb.cn/gtekmjqwcz.html

[E11] 反转字符串
来源：http://hz.gogol.net.cn/gtmenddvyu.html

Py:   s[::-1]
来源：http://hz.shuidangran.top/gteajjnica.html

PHP:  strrev($s);
来源：http://hz.svipenyu.cn/gttcjrzysp.html

JS:   [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtmofulyxz.html

TS:   [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gthzdshghq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.316326.xyz/gtjvribkpk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.birdmap.top/gtvgdaojgk.html

Ruby: s.reverse
来源：http://hz.hfpthk.cn/gtnewmzend.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinqigfzy.top/gtcdnugrub.html

[E12] 统计某字符出现次数
来源：http://hz.dashuyun.cn/gtilwgaxic.html

Py:   s.count("a")
来源：http://hz.xuanzx.com/gtajxuquce.html

PHP:  substr_count($s, "a");
来源：http://hz.zdqjudy.top/gtorvbiwmr.html

JS:   s.split("a").length - 1
来源：http://hz.daria6918.cn/gtlfupsnyo.html

TS:   s.split("a").length - 1
来源：http://hz.chenlongwang.top/gtevfkubvi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nanxinkj.top/gtirtpxuye.html

Go:   strings.Count(s, "a")
来源：http://hz.xuanzx.com/gtaoasvgec.html

Ruby: s.count("a")
来源：http://hz.yj202588.top/gtszwujmtg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.wangdashe.top/gtwpuykgnk.html

[E13] 逐字符遍历
来源：http://hz.gzhubu.top/gtsfcdszho.html

Py:   for ch in s: print(ch)
来源：http://hz.nanxinkj.top/gtouqzcvag.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xziqi.cn/gtvpffaqfx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aizwys.cn/gtdfwgihfp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hammf.cn/gtbkdvcico.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hnqzz.top/gtlfjwpbkr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenjidiqi.icu/gtogivacdz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jqgfzy.top/gtiuvaufci.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nanxuanxn.top/gtvhhmchtm.html

[E14] URL 编码与 Base64
来源：http://hz.birdmap.top/gtlkovcpur.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yueranfly.top/gtgyifjmpr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuxming.cn/gtppixummi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jqgfzy.top/gtchjehqzk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cdnleiting.top/gtsrgmlpid.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.fzhhl.top/gtehogxssl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gaohongyu789.top/gtxgtcxvfs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhijiandao.cn/gtjokjnhjr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.iojbl.cn/gtkfeehyuy.html

[E15] HTML 转义 / 反转义
来源：http://hz.shzxlz.cn/gtzbhkbeia.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.bjfxy.top/gtglefalry.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xingfuxueyuan.xyz/gtsxodcqhp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shanyushiyangtech.top/gtclyydits.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yvedp.cn/gtkzhpjgml.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xuetiantiany.cn/gtbhlbipsc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zycfv.cn/gteigumvjz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.mhx1999.top/gtcqdwzmpq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jyoumei.cn/gtjljgpqte.html

[E16] 数字千分位
来源：http://hz.jinghuilouyu.cn/gtpyxrqxdz.html

Py:   f"{1234567:,}"
来源：http://hz.iojbl.cn/gtmpjhxerl.html

PHP:  number_format(1234567);
来源：http://hz.jyoumei.cn/gtjeyxsxzv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shzxlz.cn/gtomrmrklr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangkeji.top/gtqdxbdcen.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.52xcode.cn/gtelcbhhap.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinyuanbaomall.cn/gtdqrwpcpn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhongyouzk.top/gtqksgfpxh.html

C#:   1234567.ToString("N0")
来源：http://hz.cdnleiting.top/gtdnmiahje.html

[E17] 首字母大写
来源：http://hz.shanyushiyangtech.top/gtmzwxkudr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yonumen.top/gttxahpabd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nwbrower.top/gtaztiparf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.bjfxy.top/gtnxorulsf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gotoacloud.top/gtjcwaryqa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhengqikj.top/gtnbqejsze.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhongyouzk.top/gtxceopciy.html

Ruby: s.capitalize
来源：http://hz.guowangkeji.top/gtmxhvbkbl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jqgufenzy.top/gthfafbanr.html

[E18] 模板占位符替换
来源：http://hz.yuxming.cn/gtmfctedok.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hysaishi.cn/gtkvjwkmpp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.iojbl.cn/gtrrpfudvd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhoulong.xyz/gtjxiqlfbq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.pengpengdd.cyou/gtgbldmxnn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yj202588.top/gtooqydjed.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.redwolf501.top/gtumeiktbo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.smart0.xyz/gtygzpyirj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.iojbl.cn/gtragjlhbt.html

[E19] 多行文本按行拆分
来源：http://hz.wangdashe.top/gthzavpxdw.html

Py:   s.splitlines()
来源：http://hz.tian-w.cn/gtlhnfuxmj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hammf.cn/gtzhlbkcpn.html

JS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gtxmmaymvw.html

TS:   s.split(/\r?\n/)
来源：http://hz.ywan-chungtsiang.top/gttuigjlvg.html

Java: s.lines().toList()
来源：http://hz.fengsongda.top/gtonvdhzfs.html

Go:   strings.Split(s, "\n")
来源：http://hz.yueranfly.top/gtycbtnlhq.html

Ruby: s.lines
来源：http://hz.birdmap.top/gtwgzanvox.html

C#:   s.Split('\n')
来源：http://hz.vqdsnc.cn/gtwkphyltn.html

[E20] 判断字符串是否为空
来源：http://hz.yuanzhike.top/gtnyhoqnsu.html

Py:   if not s:
来源：http://hz.dianchejie.cn/gtefykvzib.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj20258888.top/gtlykkqyyb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.daria6918.cn/gttgwkqltz.html

TS:   if (s === "") {}
来源：http://hz.meibo888.top/gtfgrffceh.html

Java: if (s.isEmpty()) {}
来源：http://hz.shuidangran.top/gttgiylade.html

Go:   if s == "" {}
来源：http://hz.wangshuangyany.cn/gtgytxqkyq.html

Ruby: if s.empty?
来源：http://hz.jlsjyb.cn/gttpflqzgv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhaomingkeji.xyz/gtylflixjw.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangkeji.top/gtavnjoxyy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hnqzz.top/gtyhaqlzwo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.andypj.xyz/gtleglzumq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gtajxqzjsp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shzxlz.cn/gtoqcuzhbx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenlongwang.top/gtxkhyhpni.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tanke756.top/gtozvnauyu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenlongwang.top/gtrxuhjvvp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtpwlhwhlh.html

[E22] 字节长度与字符长度
来源：http://hz.smart0.xyz/gtdyagankq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xingfuxueyuan.xyz/gtaglsrqgv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuanzhike.top/gtgjbeuzxu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhixingplan.top/gtrreorbry.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gtawiazdvo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jiagoushi.top/gtcrdypwyn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yuanzhike.top/gtkbsqugyh.html

Ruby: s.bytesize;  s.length
来源：http://hz.52xcode.cn/gtflhljjma.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenjidiqi.icu/gtiglykfgv.html

================================================================================
来源：http://hz.jinqigufen.top/gtmhjvipax.html

F. 文件与目录
来源：http://hz.tian-w.cn/gtjvisnmnr.html

================================================================================
来源：http://hz.ybcxt.top/gtfgpdtdgy.html

[F01] 读取整个文件
来源：http://hz.shanyushiyangtech.top/gtgdatqzgp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinyuanbaomall.cn/gtymmlpenw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.haohaochexian.top/gtjptymjad.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.fengsongda.top/gtkgzlpmse.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xylfe.cn/gthysijovp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtkusypogh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yangfankeji.com/gtzucwwbpn.html

Ruby: File.read("a.txt")
来源：http://hz.wangdashe.top/gtfogauztz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.pengpengdd.cyou/gtdneuahee.html

[F02] 逐行读取文件
来源：http://hz.tianlin.xyz/gtepyyrkcc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yonumen.top/gtghfahrtx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ivvv.top/gtajwugpab.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxinkj.top/gtrlygeefv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shuidangran.top/gtlftleudy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yj20258.top/gtjojehmom.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhiwuduotai.top/gtbbmspbqm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.meibo888.top/gtuuaevtea.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yuanzhike.top/gtjanvvvxi.html

[F03] 写入文件（覆盖）
来源：http://hz.sweek.top/gtnphshaks.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jyoumei.cn/gtmuymkgve.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cheryme.top/gteebeaepm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gtuhcrofqb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.c1oappe.top/gtugsnawen.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shangyingyoupin.top/gthqsbmodp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.52xcode.cn/gtcmfrxlth.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hnxiangtu.top/gthdjnjxua.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cucudq.cn/gtwzatzrsp.html

[F04] 追加写入文件
来源：http://hz.yangfankeji.com/gthidygfkj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhixingplan.top/gtvitxwqem.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shuidangran.top/gtlfvhkhcs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtpeiqgive.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtfxndiydj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.c1oappe.top/gtshdkygrx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hywenlv.cn/gtmxfpexnk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sweek.top/gtqjhsuiuy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj202588.top/gtacwplver.html


<!-- 参考信息 -->