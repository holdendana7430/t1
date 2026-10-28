代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gotoacloud.top/gtjsuprnlo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jiagoushi.top/gtctiabhsr.html

Go:   // 手写 map[string][]T
来源：http://hz.hammf.cn/gtnsoobuyh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhoulong.xyz/gtxermecfb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.havefunace.top/gtiwjnwwxp.html

[D20] 统计每个元素出现次数
来源：http://hz.guowangkeji.top/gtxyrofzrf.html

Py:   Counter(arr)
来源：http://hz.jyoumei.cn/gtfpsvjstf.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigfzy.top/gtuftfhcyg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.feifeiyinyue.top/gtmbqmapjv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jyoumei.cn/gtclxiedwk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dashuyun.cn/gtsahbzyak.html

Go:   // 手写 map[T]int
来源：http://hz.nanxuanxn.top/gtclcqxcdf.html

Ruby: arr.tally
来源：http://hz.zycfv.cn/gtwnnkrwwm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cucudq.cn/gtshwirclx.html

[D21] 判断是否包含某元素
来源：http://hz.gogol.net.cn/gtprqthqcf.html

Py:   x in arr
来源：http://hz.c1oappe.top/gtprgdthob.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xuanzx.com/gteleybdsd.html

JS:   arr.includes(x)
来源：http://hz.xziqi.cn/gtnasbfrjz.html

TS:   arr.includes(x)
来源：http://hz.cucudq.cn/gthztgxotu.html

Java: list.contains(x)
来源：http://hz.zdqjudy.top/gtjezazpek.html

Go:   slices.Contains(arr, x)
来源：http://hz.sufxvd.cn/gtxuecoydn.html

Ruby: arr.include?(x)
来源：http://hz.chenzaomai.com/gtfeooebop.html

C#:   list.Contains(x)
来源：http://hz.shanyushiyangkeji.top/gtppmgsmbb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.havefunace.top/gtrvmbeckk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxinkj.top/gtzbbozcpo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ydzc1.top/gtrutzqoln.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jqgufenzy.top/gtzqxfkreo.html

TS:   [...arr];
来源：http://hz.ydjk.org.cn/gtbmytdqlz.html

Java: new ArrayList<>(list);
来源：http://hz.aibaodan.cn/gtvvnvnhrk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nwbrower.top/gtjnzlircx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nanxinkj.top/gtpnluprwl.html

C#:   new List<int>(list);
来源：http://hz.cucudq.cn/gtjcvhouhs.html

[D23] reduce 累积计算
来源：http://hz.svipenyu.cn/gtcxcbxvdp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.52xcode.cn/gtyfovwowf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tianlin.xyz/gtjzxwcbku.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxinkj.top/gtljzzbish.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.wangshuangyany.cn/gttpkgbfpy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hammf.cn/gtatiwwebu.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtttlmwruc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.fzhhl.top/gtmaxrknqj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yuxming.cn/gtlgvhihan.html

[D24] 字典 / Map 基本操作
来源：http://hz.sweek.top/gtitkasifw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.svipenyu.cn/gtslnwwlih.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhijiandao.cn/gtvgobvmyn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ivvv.top/gtsbjbdtbx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hysaishi.cn/gtloxuhvmr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.bjfxy.top/gtnyrpzxxc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cdnleiting.top/gtcsgyowhq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yonumen.top/gtdtgjuyvi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ybcxt.top/gtucaneynq.html

[D25] Set 集合去重与交并差
来源：http://hz.hfpthk.cn/gtmhgsebij.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yuxming.cn/gtzxymdedx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.dashuyun.cn/gtvoaezkao.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hammf.cn/gtihfdljlh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xziqi.cn/gtkepvbtjy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yuanzhike.top/gtcldqvcij.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zdqjudy.top/gttkkdfojx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.tianlin.xyz/gtmqmlkfpw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.fengsongda.top/gtjsdqlcey.html

[D26] 数组转字符串
来源：http://hz.sxryk.cn/gtvnsxrvwx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.wangshuangyany.cn/gtaicfjrkc.html

PHP:  implode(", ", $arr);
来源：http://hz.zhongyouzk.top/gtekzbqvkb.html

JS:   arr.join(", ")
来源：http://hz.nwbrower.top/gtywnujdyz.html

TS:   arr.join(", ")
来源：http://hz.hywenlv.cn/gtmvycggch.html

Java: String.join(", ", list)
来源：http://hz.zhijiandao.cn/gthbgkuldg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.vqdsnc.cn/gtzjakidyz.html

Ruby: arr.join(", ")
来源：http://hz.gzhubu.top/gtywpyrsvr.html

C#:   string.Join(", ", list)
来源：http://hz.wangdashe.top/gtjldubkdf.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtjbfqdefw.html

E. 字符串处理
来源：http://hz.yonumen.top/gtsggqiaqi.html

================================================================================
来源：http://hz.guannengcc.top/gtznivanlq.html

[E01] 拼接字符串
来源：http://hz.zhixingplan.top/gtilbvjewk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ydjk.org.cn/gtatuiolxg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj20258.top/gtzaukfeax.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fengsongda.top/gtrquvbrne.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhengqikj.top/gtqmezhlnw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cashguo.top/gtyojfpqir.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yongpay.top/gtokjqxjra.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cashguo.top/gtnstvsyzt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.aibaodan.cn/gtqttxnxkp.html

[E02] 重复字符串
来源：http://hz.jinqigfzy.top/gtonedyqcu.html

Py:   "ab" * 3
来源：http://hz.hysaishi.cn/gtptmgfvex.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinqigfzy.top/gtqksirejp.html

JS:   "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtbdzzfbtv.html

TS:   "ab".repeat(3)
来源：http://hz.birdmap.top/gtryjnjneo.html

Java: "ab".repeat(3)
来源：http://hz.gotoacloud.top/gtjpwgnlfz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhaomingkeji.xyz/gtuugacibs.html

Ruby: "ab" * 3
来源：http://hz.jinyuanbaomall.cn/gtxtgilzzi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jqgfzy.top/gtdtacdita.html

[E03] 截取子串
来源：http://hz.shuidangran.top/gtddlzjceo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yongpay.top/gtdfwyfgva.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.tian-w.cn/gtjvmtdxph.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shangyingyoupin.top/gtvmjfjobu.html

TS:   s.slice(1, 4)
来源：http://hz.tianlin.xyz/gtxzryaiqr.html

Java: s.substring(1, 4)
来源：http://hz.yj20258.top/gtydoggmfx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.mhx1999.top/gticfquazq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ydjk.org.cn/gtlkbussbo.html

C#:   s.Substring(1, 3)
来源：http://hz.shuidangran.top/gtiffkcpor.html

[E04] 查找子串位置
来源：http://hz.yuanzhike.top/gtsferupso.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sufxvd.cn/gtshjomulv.html

PHP:  strpos($s, "x");
来源：http://hz.jinghuilouyu.cn/gtpirglggs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gotoacloud.top/gttjgbqihe.html

TS:   s.indexOf("x")
来源：http://hz.yanxiufei.cn/gtacqmoyfp.html

Java: s.indexOf("x")
来源：http://hz.jinqigufen.top/gtderosgcu.html

Go:   strings.Index(s, "x")
来源：http://hz.yanxiufei.cn/gtaotchbau.html

Ruby: s.index("x")
来源：http://hz.jianghu66.top/gtfythnswk.html

C#:   s.IndexOf("x")
来源：http://hz.zhoulong.xyz/gtuanekpol.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.mhx1999.top/gtetyozsgq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jinghuilouyu.cn/gtlzmmvrip.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.wangshuangyany.cn/gtevfgngxi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.0kj1m.cn/gtlkpcjvlo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.daria6918.cn/gtfwyicdwj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cucudq.cn/gtdrarfwbp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cdnleiting.top/gtysgwkvdf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yj20258.top/gtfvzabykd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yonumen.top/gtmxbtfcet.html

[E06] 替换子串
来源：http://hz.dianchejie.cn/gtlomokilh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.52xcode.cn/gtxcmlsfrq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.pengpengdd.cyou/gtplyrrfjf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtrqwokhyh.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtfxdajsas.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuetiantiany.cn/gtpgtedxws.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ivvv.top/gtfcszdopa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hysaishi.cn/gtqfkhmzfc.html

C#:   s.Replace("a", "b")
来源：http://hz.0kj1m.cn/gthrmupeua.html

[E07] 按分隔符拆分
来源：http://hz.sxryk.cn/gtelrzoyya.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sufxvd.cn/gtbpzrvnhh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gogol.net.cn/gtawzqpxip.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xziqi.cn/gtatjbihrk.html

TS:   s.split(",")
来源：http://hz.mhx1999.top/gtsbrqtfaa.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ehwqpu.com/gtrmplbhkf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhengqikj.top/gtqlkjggzx.html

Ruby: s.split(",");  s.split
来源：http://hz.ywan-chungtsiang.top/gtfbwgvasr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jianghu66.top/gtudtvxkpc.html

[E08] 数组按分隔符合并
来源：http://hz.yuanzhike.top/gteyteafks.html

Py:   ",".join(items)
来源：http://hz.aibaodan.cn/gtvfviqfbk.html

PHP:  implode(",", $items);
来源：http://hz.yuxming.cn/gteyxdrofo.html

JS:   items.join(",")
来源：http://hz.cqqwz.cn/gtmyxkicru.html

TS:   items.join(",")
来源：http://hz.daria6918.cn/gttxzozobo.html

Java: String.join(",", items)
来源：http://hz.c1oappe.top/gtxzoppbyc.html

Go:   strings.Join(items, ",")
来源：http://hz.xylfe.cn/gtyexbqwuf.html

Ruby: items.join(",")
来源：http://hz.meibo888.top/gtmehiwyml.html

C#:   string.Join(",", items)
来源：http://hz.daria6918.cn/gtvkaikvdk.html

[E09] 去除所有空白字符
来源：http://hz.sysykeji.top/gtxuadqiyn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aizwys.cn/gtdzsyooov.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zycfv.cn/gtbyqzbmiz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ivvv.top/gtotaoyphk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinyuanbaomall.cn/gtsijahcen.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.9152youxi.cn/gtjgnrebwn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gzhubu.top/gtliwnkvfq.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinqigfzy.top/gtnpegqhfg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xingfuxueyuan.xyz/gtqworxonq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hnxiangtu.top/gthhepscqm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinyuanbaomall.cn/gthldsqtbo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ivvv.top/gtxttwoekb.html

JS:   "7".padStart(3, "0")
来源：http://hz.iojbl.cn/gtualqboqs.html

TS:   "7".padStart(3, "0")
来源：http://hz.shanyushiyangtech.top/gtcqukmlja.html

Java: String.format("%03d", 7)
来源：http://hz.kuanghao11.cn/gtbdbfufjj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinqigfzy.top/gtjfepdsav.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.daxiang520.top/gtetfxduyy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.wangshuangyany.cn/gtkgzeqnvb.html

[E11] 反转字符串
来源：http://hz.9152youxi.cn/gthzspuazi.html

Py:   s[::-1]
来源：http://hz.yj20258888.top/gtorvzdsdb.html

PHP:  strrev($s);
来源：http://hz.dashuyun.cn/gttabyymgl.html

JS:   [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gtcbjehbve.html

TS:   [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gtvcvfsmkj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.52xcode.cn/gttekzbfwe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.pycfn.com/gtliaargnh.html

Ruby: s.reverse
来源：http://hz.xuanzx.com/gtbqypubbx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.aibaodan.cn/gtevpnnemd.html

[E12] 统计某字符出现次数
来源：http://hz.guannengcc.top/gttwjzhurf.html

Py:   s.count("a")
来源：http://hz.hnxiangtu.top/gtlwcgollf.html

PHP:  substr_count($s, "a");
来源：http://hz.jianghu66.top/gtufmypyvq.html

JS:   s.split("a").length - 1
来源：http://hz.fengsongda.top/gtsnposydn.html

TS:   s.split("a").length - 1
来源：http://hz.chenzaomai.com/gtradiafvp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.guowangkeji.top/gthbawkcjw.html

Go:   strings.Count(s, "a")
来源：http://hz.fengsongda.top/gtxyufjdjv.html

Ruby: s.count("a")
来源：http://hz.zhaomingkeji.xyz/gtksjohgtn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.haohaochexian.top/gthbghzxtz.html

[E13] 逐字符遍历
来源：http://hz.shuidangran.top/gtippxkhzb.html

Py:   for ch in s: print(ch)
来源：http://hz.yuanzhike.top/gtnmeeabyt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinghuilouyu.cn/gtrwhzcyyc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.havefunace.top/gtwkswizwc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenlongwang.top/gtuauquwzd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtvrdbcofh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zdqjudy.top/gtcocvgljr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gaohongyu789.top/gtkigfrwib.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhijiandao.cn/gtcpzkpjdb.html

[E14] URL 编码与 Base64
来源：http://hz.yj202588.top/gteejcigmk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yangfankeji.com/gteescyeit.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.haohaochexian.top/gtrrhotfec.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.9152youxi.cn/gtjpcbenfz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.wangdashe.top/gtqzztxpaq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sxryk.cn/gtprootoga.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.wangshuangyany.cn/gtreyonoar.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jianghu66.top/gtcibugljp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yanxiufei.cn/gtfsumteum.html

[E15] HTML 转义 / 反转义
来源：http://hz.haohaochexian.top/gtmefdbrez.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cdnleiting.top/gtzyhjgfrl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xylfe.cn/gtxsezuqzc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.iojbl.cn/gtopwwzxtx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zdqjudy.top/gtniyhkxbz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gaohongyu789.top/gtawrpqsad.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgfzy.top/gtfrogklsz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.svipenyu.cn/gtrbwzxhbh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yvedp.cn/gtbafcojqk.html

[E16] 数字千分位
来源：http://hz.svipenyu.cn/gtifjwxcxq.html

Py:   f"{1234567:,}"
来源：http://hz.hywenlv.cn/gtmcbhhagc.html

PHP:  number_format(1234567);
来源：http://hz.jianghu66.top/gtkxjbyfvj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.snrcjt.cn/gtjrrkbfxi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj202588.top/gtclmlijcr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nanxuanxn.top/gteswlrqcc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shuidangran.top/gtogpbsgun.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ybcxt.top/gtzshlasba.html

C#:   1234567.ToString("N0")
来源：http://hz.shanyushiyangkeji.top/gtxqufakbd.html

[E17] 首字母大写
来源：http://hz.yj20258888.top/gtfhhzoldj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hongshengwenyu.top/gtxkyfhcvs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yuxming.cn/gtupkfifni.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.kuanghao11.cn/gtsridieti.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yongpay.top/gtqlbqnspd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shzxlz.cn/gtlssxxhfv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ppjwa.cn/gtsdgbjoxk.html

Ruby: s.capitalize
来源：http://hz.feifeiyinyue.top/gtrbjiqgod.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tanke756.top/gtlzwdkzlh.html

[E18] 模板占位符替换
来源：http://hz.guowangkeji.top/gtnbaejagz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jiagoushi.top/gtusgzrnbi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.mhx1999.top/gtmkcyqfwe.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.kuanghao11.cn/gtpgllrotl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuanzhike.top/gtzwzdjthq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.tanke756.top/gttehnssef.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.tianlin.xyz/gtwaxderog.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.wangdashe.top/gtfybiibdt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sufxvd.cn/gtyptycqdl.html

[E19] 多行文本按行拆分
来源：http://hz.guowangkeji.top/gtdbkslebn.html

Py:   s.splitlines()
来源：http://hz.tanke756.top/gthljwftzd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj20258.top/gtwcntkujs.html

JS:   s.split(/\r?\n/)
来源：http://hz.0kj1m.cn/gtpzrgajmt.html

TS:   s.split(/\r?\n/)
来源：http://hz.guowangkeji.top/gtdyxhpece.html

Java: s.lines().toList()
来源：http://hz.svipenyu.cn/gtdhptbdhw.html

Go:   strings.Split(s, "\n")
来源：http://hz.dianchejie.cn/gtvaoebljm.html

Ruby: s.lines
来源：http://hz.dianchejie.cn/gtnuafywnm.html

C#:   s.Split('\n')
来源：http://hz.mhx1999.top/gtpcgdznrx.html

[E20] 判断字符串是否为空
来源：http://hz.cqqwz.cn/gtgmgnpxpv.html

Py:   if not s:
来源：http://hz.pengpengdd.cyou/gtrofwugfs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ehwqpu.com/gtqxjmgvds.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.snrcjt.cn/gtmjsdypbs.html

TS:   if (s === "") {}
来源：http://hz.dianchejie.cn/gtukwsxloi.html

Java: if (s.isEmpty()) {}
来源：http://hz.pycfn.com/gteqlwtnom.html

Go:   if s == "" {}
来源：http://hz.hnqzz.top/gtczbgjylt.html

Ruby: if s.empty?
来源：http://hz.guowangkeji.top/gtizjzwngi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tianlin.xyz/gtpvnqfgpa.html

[E21] 超长截断加省略号
来源：http://hz.hywenlv.cn/gtsfclpceo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.aibaodan.cn/gtmfjmbyth.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.tian-w.cn/gtbhmqqeqi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtuscamueb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gttolgauaj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ivvv.top/gtlggqsbyl.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xuanzx.com/gtwezbqltv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zycfv.cn/gtontkxshk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.316326.xyz/gthdqbtttz.html

[E22] 字节长度与字符长度
来源：http://hz.cucudq.cn/gtmshtaebk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jyoumei.cn/gtzhwizkyk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.daria6918.cn/gtuzmxyelz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ybcxt.top/gtywlxnsrl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhijiandao.cn/gtdsxaliis.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ydzc1.top/gtzewydlhf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.52xcode.cn/gtopbbedsk.html

Ruby: s.bytesize;  s.length
来源：http://hz.birdmap.top/gtxogwvlde.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenzaomai.com/gttcgcakol.html

================================================================================
来源：http://hz.yongpay.top/gtckwlfxft.html

F. 文件与目录
来源：http://hz.hammf.cn/gtbvahemzv.html

================================================================================
来源：http://hz.guannengcc.top/gtaznvzsic.html

[F01] 读取整个文件
来源：http://hz.jqgufenzy.top/gtysumpgmc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hysaishi.cn/gtkqoorvzb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gaohongyu789.top/gtrsbvbprv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinqigfzy.top/gtanbaxsrv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.fengsongda.top/gtpnqokftj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtnusxshte.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hywenlv.cn/gtjfayljst.html

Ruby: File.read("a.txt")
来源：http://hz.daxiang520.top/gtsmraqvut.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jqgufenzy.top/gtjketrhky.html

[F02] 逐行读取文件
来源：http://hz.cheryme.top/gtqybfncli.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zycfv.cn/gtrotkftux.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yuxming.cn/gtckvjydrf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.wangshuangyany.cn/gtssdqrqha.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenlongwang.top/gtqisxiexq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sxryk.cn/gtocybxeib.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tanke756.top/gtrtnkmcla.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.haohaochexian.top/gtsrnkziyh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhaomingkeji.xyz/gtqwkjlajj.html

[F03] 写入文件（覆盖）
来源：http://hz.xuetiantiany.cn/gtybzbxots.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.havefunace.top/gtbgpttkze.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xingfuxueyuan.xyz/gtrntxdjaw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.316326.xyz/gtscjlajix.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yanxiufei.cn/gtmqfdnist.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ywan-chungtsiang.top/gtgdeiskqx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cheryme.top/gthkswpvxv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.guannengcc.top/gtwvttttmh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.redwolf501.top/gtumetqwzh.html

[F04] 追加写入文件
来源：http://hz.jinqigufen.top/gtecheefcs.html


<!-- 参考信息 -->