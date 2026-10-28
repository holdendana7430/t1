代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sufxvd.cn/gtbectujws.html

C#:   list.Sum();  list.Average()
来源：http://hz.hysaishi.cn/gtbprbyfdk.html

[D17] 最大值与最小值
来源：http://hz.xuanzx.com/gtyruyiamt.html

Py:   max(arr);  min(arr)
来源：http://hz.shuidangran.top/gtxqkqcgck.html

PHP:  max($arr);  min($arr);
来源：http://hz.ydzc1.top/gtagvptnkz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.chenlongwang.top/gtjzpoxqtr.html

TS:   Math.max(...arr);
来源：http://hz.guannengcc.top/gtisguioti.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ydzc1.top/gtpcetgsnd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.iojbl.cn/gtpasumhlk.html

Ruby: arr.max;  arr.min
来源：http://hz.jianghu66.top/gtxxzmekcr.html

C#:   list.Max();  list.Min()
来源：http://hz.316326.xyz/gtajrqgicf.html

[D18] 扁平化嵌套数组
来源：http://hz.wangshuangyany.cn/gtpyqbzgay.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.svipenyu.cn/gtqrquzymk.html

PHP:  array_merge(...$nested);
来源：http://hz.wangdashe.top/gtwgfzrppu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.gotoacloud.top/gtesrkdvvf.html

TS:   nested.flat();
来源：http://hz.jinghuilouyu.cn/gtunatghou.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenlongwang.top/gteszyefxs.html

Go:   // 手写双层循环
来源：http://hz.gaohongyu789.top/gtqvupesvg.html

Ruby: nested.flatten
来源：http://hz.jinqigufen.top/gtclgzxymh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.tian-w.cn/gtohovxwmp.html

[D19] 按字段分组
来源：http://hz.daria6918.cn/gtzyewyyfa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj20258888.top/gtabmqmahu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xingfuxueyuan.xyz/gtwncvfpqk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.kuanghao11.cn/gtqvxdvwoh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shanyushiyangtech.top/gtfqsdzjst.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenjidiqi.icu/gtvmmryuxf.html

Go:   // 手写 map[string][]T
来源：http://hz.svipenyu.cn/gtuzfsiryx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.snrcjt.cn/gtgkrzthsd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hnxiangtu.top/gtshoodghh.html

[D20] 统计每个元素出现次数
来源：http://hz.yuanzhike.top/gtfzoanmol.html

Py:   Counter(arr)
来源：http://hz.fengsongda.top/gttcpsadwr.html

PHP:  array_count_values($arr);
来源：http://hz.zhongyouzk.top/gtynidhvoz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhijiandao.cn/gtuylorzfx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hysaishi.cn/gtcnsnjkfy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.nwbrower.top/gtfiquiafn.html

Go:   // 手写 map[T]int
来源：http://hz.shzxlz.cn/gtcomvrxve.html

Ruby: arr.tally
来源：http://hz.haohaochexian.top/gtfdwlnmru.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yuanzhike.top/gthtyigpxd.html

[D21] 判断是否包含某元素
来源：http://hz.hongshengwenyu.top/gtulkapkln.html

Py:   x in arr
来源：http://hz.ywan-chungtsiang.top/gtafklkbat.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jianghu66.top/gtohdolegg.html

JS:   arr.includes(x)
来源：http://hz.gzhubu.top/gtvidnhage.html

TS:   arr.includes(x)
来源：http://hz.sysykeji.top/gtsomggycp.html

Java: list.contains(x)
来源：http://hz.ydzc1.top/gtlkzwfaze.html

Go:   slices.Contains(arr, x)
来源：http://hz.hongshengwenyu.top/gtbimznodj.html

Ruby: arr.include?(x)
来源：http://hz.nanxuanxn.top/gtzvrdhwjq.html

C#:   list.Contains(x)
来源：http://hz.xylfe.cn/gticvxlxva.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tian-w.cn/gthpagvybi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sufxvd.cn/gtbczijzjp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tian-w.cn/gtzonlsjbh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.9152youxi.cn/gtzaeeyauy.html

TS:   [...arr];
来源：http://hz.cheryme.top/gtnhbnppsv.html

Java: new ArrayList<>(list);
来源：http://hz.guowangkeji.top/gtwtmkzywx.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenlongwang.top/gtbwhjhbde.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ydzc1.top/gtnhtublhz.html

C#:   new List<int>(list);
来源：http://hz.snrcjt.cn/gtymdghkxl.html

[D23] reduce 累积计算
来源：http://hz.hfpthk.cn/gtqilltbbc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cashguo.top/gtcjosadjv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.dianchejie.cn/gtbwurguay.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.9152youxi.cn/gthsspxtaa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.wangshuangyany.cn/gtipfsjghr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.iojbl.cn/gtnbmljsmb.html

Go:   // 手写循环
来源：http://hz.hongshengwenyu.top/gttelgbhls.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cucudq.cn/gtfypuiwfk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.dianchejie.cn/gtwhofyzit.html

[D24] 字典 / Map 基本操作
来源：http://hz.hammf.cn/gtajtappah.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jlsjyb.cn/gtwepkxfuy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sweek.top/gtywrfpten.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ybcxt.top/gtysymzhwy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xuanzx.com/gtxexkuikn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhiwuduotai.top/gtdtuivxmm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shanyushiyangkeji.top/gtcfwwrryi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yueranfly.top/gtcxrlklpv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.dashuyun.cn/gtzxxbjvia.html

[D25] Set 集合去重与交并差
来源：http://hz.jlsjyb.cn/gtebwydhib.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jiagoushi.top/gtqbgttiou.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.wangdashe.top/gtauxbfeuc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ivvv.top/gtowymshca.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xuetiantiany.cn/gtbytharjq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.daria6918.cn/gtekysrzry.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hammf.cn/gtvzdonztz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sufxvd.cn/gtnoiuandd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jqgufenzy.top/gtakcfheke.html

[D26] 数组转字符串
来源：http://hz.andypj.xyz/gtqnmvepgy.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zdqjudy.top/gtlbmybwrh.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgufenzy.top/gtkswmgujj.html

JS:   arr.join(", ")
来源：http://hz.quarkkingdee.top/gtlfcvfjta.html

TS:   arr.join(", ")
来源：http://hz.daxiang520.top/gttxqdobvj.html

Java: String.join(", ", list)
来源：http://hz.dianchejie.cn/gtslbzjznh.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gotoacloud.top/gtsjjiipmm.html

Ruby: arr.join(", ")
来源：http://hz.yanxiufei.cn/gthsylpkyd.html

C#:   string.Join(", ", list)
来源：http://hz.zhijiandao.cn/gtetfmccyz.html

================================================================================
来源：http://hz.c1oappe.top/gtolpqapwh.html

E. 字符串处理
来源：http://hz.jinqigufen.top/gtquusefne.html

================================================================================
来源：http://hz.yonumen.top/gturtdtgcd.html

[E01] 拼接字符串
来源：http://hz.zdqjudy.top/gtmpaezlzv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ydzc1.top/gtqbwrxhxx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yongpay.top/gtaldgnlhi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cucudq.cn/gtzwfhcnum.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nwbrower.top/gtpyexkzhw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jianghu66.top/gtvzrnybbx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.wangdashe.top/gtdhddjixm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.feifeiyinyue.top/gtpaiskxek.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shzxlz.cn/gttxwecvbu.html

[E02] 重复字符串
来源：http://hz.ydjk.org.cn/gtoqibqmxg.html

Py:   "ab" * 3
来源：http://hz.zycfv.cn/gthqtdqdkz.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yonumen.top/gtcsqavdip.html

JS:   "ab".repeat(3)
来源：http://hz.gotoacloud.top/gtqrlkssnc.html

TS:   "ab".repeat(3)
来源：http://hz.yj202588.top/gtbuieefcu.html

Java: "ab".repeat(3)
来源：http://hz.meibo888.top/gtrksuizdy.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yuxming.cn/gthnofpppp.html

Ruby: "ab" * 3
来源：http://hz.xinyue.icu/gtqpbwqxcr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nwbrower.top/gtwoqitzcj.html

[E03] 截取子串
来源：http://hz.nanxinkj.top/gtwbyrskpm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhijiandao.cn/gtpvdmltvs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xuanzx.com/gtvvnlpqgp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shuidangran.top/gtlalnetor.html

TS:   s.slice(1, 4)
来源：http://hz.nanxinkj.top/gtajkoliav.html

Java: s.substring(1, 4)
来源：http://hz.yvedp.cn/gtsspwaaja.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yj20258.top/gtzbunywsb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nanxuanxn.top/gtlodmrtdn.html

C#:   s.Substring(1, 3)
来源：http://hz.gzhubu.top/gteetnlvzl.html

[E04] 查找子串位置
来源：http://hz.svipenyu.cn/gtqhvpuloq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yueranfly.top/gtrnkfuzwt.html

PHP:  strpos($s, "x");
来源：http://hz.bjfxy.top/gttlqibyqi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.nanxuanxn.top/gtmbodukbl.html

TS:   s.indexOf("x")
来源：http://hz.cdnleiting.top/gtnwdunjyq.html

Java: s.indexOf("x")
来源：http://hz.meibo888.top/gtpianmvxn.html

Go:   strings.Index(s, "x")
来源：http://hz.ydjk.org.cn/gtapywfgee.html

Ruby: s.index("x")
来源：http://hz.jlsjyb.cn/gtsrrfpusr.html

C#:   s.IndexOf("x")
来源：http://hz.mhx1999.top/gtddiucted.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ppjwa.cn/gtvgmllvpm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhengqikj.top/gtrgpuvgah.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.feifeiyinyue.top/gtrzimnamd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.aizwys.cn/gtwattnhca.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yonumen.top/gtrajmhvga.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.c1oappe.top/gtmbckigns.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cashguo.top/gtsbyiista.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.andypj.xyz/gtuiyxdcgx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.bjfxy.top/gtbaclpfwp.html

[E06] 替换子串
来源：http://hz.zdqjudy.top/gttpmczgue.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.dianchejie.cn/gtejfofzoa.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zdqjudy.top/gtsslregia.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtsdzxudne.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtkvhiurcc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gthxyvkeby.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinqigfzy.top/gtuhidcrfg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.snrcjt.cn/gtsbopjvuu.html

C#:   s.Replace("a", "b")
来源：http://hz.xuetiantiany.cn/gtzkodnmdl.html

[E07] 按分隔符拆分
来源：http://hz.xziqi.cn/gtxoodcgmv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinyuanbaomall.cn/gtqjdksymy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhijiandao.cn/gtxnxnslzb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shangyingyoupin.top/gttradtssy.html

TS:   s.split(",")
来源：http://hz.shanyushiyangtech.top/gtugklhtlu.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.fzhhl.top/gtlutxmrok.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.aizwys.cn/gtgmhkyqfw.html

Ruby: s.split(",");  s.split
来源：http://hz.nwbrower.top/gtjvxalqql.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.meibo888.top/gtkwygrshf.html

[E08] 数组按分隔符合并
来源：http://hz.ywan-chungtsiang.top/gtwccqyiht.html

Py:   ",".join(items)
来源：http://hz.kuanghao11.cn/gtstshytou.html

PHP:  implode(",", $items);
来源：http://hz.tianlin.xyz/gtztmqgchy.html

JS:   items.join(",")
来源：http://hz.hfpthk.cn/gtaohnerir.html

TS:   items.join(",")
来源：http://hz.daria6918.cn/gtffrvmjcr.html

Java: String.join(",", items)
来源：http://hz.yj20258888.top/gtyzpbbjit.html

Go:   strings.Join(items, ",")
来源：http://hz.dianchejie.cn/gtvafwdpfo.html

Ruby: items.join(",")
来源：http://hz.yongpay.top/gtoppqczvv.html

C#:   string.Join(",", items)
来源：http://hz.c1oappe.top/gtormuruhe.html

[E09] 去除所有空白字符
来源：http://hz.sysykeji.top/gtvyzpyeys.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hywenlv.cn/gtitdmrgnl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hnxiangtu.top/gtfpehswhd.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.svipenyu.cn/gtdntzqxhv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj202588.top/gtiqgwvacy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.meibo888.top/gtcgoupmhq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.mhx1999.top/gttukctlhl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.bjfxy.top/gtqlwarsrx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hfpthk.cn/gticvxqjtg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhixingplan.top/gtfmpxnvym.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhijiandao.cn/gtxulqvrhq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhoulong.xyz/gtskvgwdvm.html

JS:   "7".padStart(3, "0")
来源：http://hz.316326.xyz/gtttrrvjte.html

TS:   "7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gtfkcjwfnz.html

Java: String.format("%03d", 7)
来源：http://hz.sweek.top/gtxdursivz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhixingplan.top/gtnxmlchxt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sufxvd.cn/gtndihbjlg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shangyingyoupin.top/gtoupzbcfu.html

[E11] 反转字符串
来源：http://hz.dashuyun.cn/gtatvxkgdd.html

Py:   s[::-1]
来源：http://hz.jinghuilouyu.cn/gtcnsuzkpa.html

PHP:  strrev($s);
来源：http://hz.yvedp.cn/gtsrmibhnw.html

JS:   [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtsivfegvj.html

TS:   [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtzizarmvb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.0kj1m.cn/gtkqxfwmgb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zdqjudy.top/gtcvabhyaf.html

Ruby: s.reverse
来源：http://hz.birdmap.top/gtmukgnhlj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cdnleiting.top/gtsallaqhe.html

[E12] 统计某字符出现次数
来源：http://hz.xuetiantiany.cn/gtdsvrzoxc.html

Py:   s.count("a")
来源：http://hz.hywenlv.cn/gtaoqnuyjs.html

PHP:  substr_count($s, "a");
来源：http://hz.zhoulong.xyz/gtmtfpveyp.html

JS:   s.split("a").length - 1
来源：http://hz.jyoumei.cn/gtqnbqvaga.html

TS:   s.split("a").length - 1
来源：http://hz.zhiwuduotai.top/gtyxabdhrw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.c1oappe.top/gtettbwktg.html

Go:   strings.Count(s, "a")
来源：http://hz.nwbrower.top/gtdqvxnbxw.html

Ruby: s.count("a")
来源：http://hz.shangyingyoupin.top/gtvoavylhq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.c1oappe.top/gtwhezsrkx.html

[E13] 逐字符遍历
来源：http://hz.9152youxi.cn/gtivxjlzbk.html

Py:   for ch in s: print(ch)
来源：http://hz.jinyuanbaomall.cn/gtmfpaixot.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.quarkkingdee.top/gtkqhmwzpe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tian-w.cn/gtfqzahacd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gtwsvgjyqv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.guowangkeji.top/gtyhgjmepr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ywan-chungtsiang.top/gtwnfrjtkl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.iojbl.cn/gtfqqlkccp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sxryk.cn/gtgxqhkooi.html

[E14] URL 编码与 Base64
来源：http://hz.yonumen.top/gtwqfwociq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.pengpengdd.cyou/gtfbylddoe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nwbrower.top/gtujadyhfv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.aizwys.cn/gtekefrwlk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xuanzx.com/gtrgksbvqa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.birdmap.top/gtoddklrqd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xuetiantiany.cn/gtramuqeua.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhiwuduotai.top/gtzeyzaeto.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.pengpengdd.cyou/gtzhreiupf.html

[E15] HTML 转义 / 反转义
来源：http://hz.gaohongyu789.top/gtfcltcloe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hywenlv.cn/gttxhnxxck.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinqigfzy.top/gtmrllbrww.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cdnleiting.top/gtfuwbcgml.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.birdmap.top/gtvudkbndn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ybcxt.top/gtaazhlpex.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sxryk.cn/gtqhcxlmrc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.daria6918.cn/gtwdctkbkd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aizwys.cn/gtpvelcvwa.html

[E16] 数字千分位
来源：http://hz.zhengqikj.top/gtqvenrhql.html

Py:   f"{1234567:,}"
来源：http://hz.sysykeji.top/gtpnvudqfn.html

PHP:  number_format(1234567);
来源：http://hz.yuanzhike.top/gtyowphxzh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.tian-w.cn/gtiiqbkeet.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jianghu66.top/gtavmvxggy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.mhx1999.top/gtrcjsdbva.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhiwuduotai.top/gtxohmhafh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hammf.cn/gtftxaoguy.html

C#:   1234567.ToString("N0")
来源：http://hz.nanxinkj.top/gtaesfqbgt.html

[E17] 首字母大写
来源：http://hz.chenzaomai.com/gtgvbkgkto.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ydjk.org.cn/gtogulauaz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ybcxt.top/gtujcfwlir.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ivvv.top/gtygacxcob.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhongyouzk.top/gthfujsheo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sweek.top/gtuatyaxgh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.daxiang520.top/gtjuhevrkv.html

Ruby: s.capitalize
来源：http://hz.redwolf501.top/gtxqacxdag.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jqgfzy.top/gtlsxcotsa.html

[E18] 模板占位符替换
来源：http://hz.sysykeji.top/gtpvqhegxe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xuetiantiany.cn/gtzqmksgmy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jqgufenzy.top/gtlrkutvyn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenjidiqi.icu/gttkvggvun.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zdqjudy.top/gtwfckupzj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xuetiantiany.cn/gtaqsvehey.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.quarkkingdee.top/gtbkpttocf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cashguo.top/gthbbyfekf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ehwqpu.com/gtqgkpjaae.html

[E19] 多行文本按行拆分
来源：http://hz.zhoulong.xyz/gtabcfzwlb.html

Py:   s.splitlines()
来源：http://hz.kuanghao11.cn/gtnrdgtstq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.haohaochexian.top/gtidjkqmrt.html

JS:   s.split(/\r?\n/)
来源：http://hz.jianghu66.top/gtrxvqrodm.html

TS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gtdyixzmgw.html

Java: s.lines().toList()
来源：http://hz.zhijiandao.cn/gtaduwioyd.html

Go:   strings.Split(s, "\n")
来源：http://hz.svipenyu.cn/gtoaursxqf.html

Ruby: s.lines
来源：http://hz.kuanghao11.cn/gthdtfwxyw.html

C#:   s.Split('\n')
来源：http://hz.hnqzz.top/gtbzqquydh.html

[E20] 判断字符串是否为空
来源：http://hz.yonumen.top/gtmcjnqjhu.html

Py:   if not s:
来源：http://hz.redwolf501.top/gtkecjsfzk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigfzy.top/gtsdoburjo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jianghu66.top/gtgujbdoxi.html

TS:   if (s === "") {}
来源：http://hz.xingfuxueyuan.xyz/gtngdqupti.html

Java: if (s.isEmpty()) {}
来源：http://hz.sysykeji.top/gtczocfqer.html

Go:   if s == "" {}
来源：http://hz.chenlongwang.top/gtkqebpier.html

Ruby: if s.empty?
来源：http://hz.hnqzz.top/gtejfjrxyb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.dianchejie.cn/gtxevhikay.html

[E21] 超长截断加省略号
来源：http://hz.xuetiantiany.cn/gtjmoppwaq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.vqdsnc.cn/gtysgtnnih.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jqgfzy.top/gtgoghzstx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtpncbecod.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtqwsoduql.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtctduxeub.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.fengsongda.top/gtuplzwjqc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtniqiixuw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gaohongyu789.top/gttpekubyo.html

[E22] 字节长度与字符长度
来源：http://hz.chenlongwang.top/gtyzdxhbsa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yueranfly.top/gtmpiypmhe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuanzhike.top/gtrxyxhkao.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yanxiufei.cn/gtzrraecjx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.316326.xyz/gtznhywubm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenlongwang.top/gtisvdwbrl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ywan-chungtsiang.top/gttrmzgvfi.html

Ruby: s.bytesize;  s.length
来源：http://hz.gotoacloud.top/gtzimqhlpq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.andypj.xyz/gtncwuxohp.html

================================================================================
来源：http://hz.yonumen.top/gtcgemvnez.html

F. 文件与目录
来源：http://hz.cashguo.top/gtwnjpyuhn.html

================================================================================
来源：http://hz.zhiwuduotai.top/gttcvfkmzy.html

[F01] 读取整个文件
来源：http://hz.zhiwuduotai.top/gtwwbmlakw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ydjk.org.cn/gtbzyjbjjl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yvedp.cn/gtwphzeaqc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zycfv.cn/gtialyisrq.html


<!-- 参考信息 -->