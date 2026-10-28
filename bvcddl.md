代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zycfv.cn/gtokfuoluk.html

Ruby: arr.max;  arr.min
来源：http://hz.hysaishi.cn/gtkvhhqqjf.html

C#:   list.Max();  list.Min()
来源：http://hz.tanke756.top/gtyuguawzm.html

[D18] 扁平化嵌套数组
来源：http://hz.gogol.net.cn/gteckrjspf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.wangshuangyany.cn/gtqidpweax.html

PHP:  array_merge(...$nested);
来源：http://hz.snrcjt.cn/gtjznjvsjk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cashguo.top/gtvxhfbpaf.html

TS:   nested.flat();
来源：http://hz.yj20258.top/gtwtrulozn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.iojbl.cn/gtjvahbzik.html

Go:   // 手写双层循环
来源：http://hz.jiagoushi.top/gtbrwmywfa.html

Ruby: nested.flatten
来源：http://hz.yuanzhike.top/gthciaufkh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gotoacloud.top/gtkvjlgcnh.html

[D19] 按字段分组
来源：http://hz.sysykeji.top/gtdlelrqno.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.pengpengdd.cyou/gtcrvemdgp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.0kj1m.cn/gtjstrywda.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cdnleiting.top/gtthittwlf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhoulong.xyz/gtehgfdjit.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.meibo888.top/gtfjjbuvwa.html

Go:   // 手写 map[string][]T
来源：http://hz.jyoumei.cn/gthphvqpem.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.havefunace.top/gtulhblkbw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shanyushiyangtech.top/gtlleschxn.html

[D20] 统计每个元素出现次数
来源：http://hz.shuidangran.top/gtdwkleddi.html

Py:   Counter(arr)
来源：http://hz.zhaomingkeji.xyz/gtdcyqvsdf.html

PHP:  array_count_values($arr);
来源：http://hz.yj202588.top/gtmkiljiwa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jianghu66.top/gtgwcumnmy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhijiandao.cn/gtzzjtnxqe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.9152youxi.cn/gthcxmjszc.html

Go:   // 手写 map[T]int
来源：http://hz.cucudq.cn/gtmvrjkzwl.html

Ruby: arr.tally
来源：http://hz.zhijiandao.cn/gtxbxrgput.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinqigufen.top/gtssurrjjt.html

[D21] 判断是否包含某元素
来源：http://hz.zycfv.cn/gtheavhbrf.html

Py:   x in arr
来源：http://hz.feifeiyinyue.top/gtjtdgrflq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.guannengcc.top/gtpvzhjwuu.html

JS:   arr.includes(x)
来源：http://hz.quarkkingdee.top/gtbgmlpjkd.html

TS:   arr.includes(x)
来源：http://hz.xziqi.cn/gtjlwowjkg.html

Java: list.contains(x)
来源：http://hz.ehwqpu.com/gtzdjzgtvw.html

Go:   slices.Contains(arr, x)
来源：http://hz.dianchejie.cn/gtgraiujux.html

Ruby: arr.include?(x)
来源：http://hz.jlsjyb.cn/gtrqbbffcv.html

C#:   list.Contains(x)
来源：http://hz.zhaomingkeji.xyz/gtuldisrjo.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shzxlz.cn/gtubutnndn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.kuanghao11.cn/gtaqxpcpyh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cheryme.top/gtbhpupkpn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.guannengcc.top/gtnqvkppwc.html

TS:   [...arr];
来源：http://hz.jinqigfzy.top/gtwzpvacij.html

Java: new ArrayList<>(list);
来源：http://hz.jqgufenzy.top/gtkipiqoyd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.daxiang520.top/gttgttjldt.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cashguo.top/gtbxwocihi.html

C#:   new List<int>(list);
来源：http://hz.cqqwz.cn/gtjaokiwlm.html

[D23] reduce 累积计算
来源：http://hz.mhx1999.top/gtsywmvuvz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.meibo888.top/gtujyakvau.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.havefunace.top/gtcsbwxcns.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guannengcc.top/gttpjfkuff.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cheryme.top/gtwbgmwwys.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.9152youxi.cn/gtgwtxchwp.html

Go:   // 手写循环
来源：http://hz.gzhubu.top/gtnvqykiyq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenjidiqi.icu/gtmtflaarx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.smart0.xyz/gtajpwtudk.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhengqikj.top/gttxeuykrh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ivvv.top/gtjsesxowi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hammf.cn/gtjasekwnp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.fengsongda.top/gtnipkrigh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hfpthk.cn/gtuuszxjvh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.redwolf501.top/gtiiluyghu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.quarkkingdee.top/gtcfymovyv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhaomingkeji.xyz/gtdnadumbr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ywan-chungtsiang.top/gttpqltwhn.html

[D25] Set 集合去重与交并差
来源：http://hz.nwbrower.top/gtgxqjedai.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.havefunace.top/gtjaxethac.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ehwqpu.com/gtkzobyrlq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.pycfn.com/gtgqydmrag.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhongyouzk.top/gterbaglmo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.316326.xyz/gtjrvdqnys.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.quarkkingdee.top/gtwcbdcoyf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.birdmap.top/gtjsszijxu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ydzc1.top/gthcrcdaqg.html

[D26] 数组转字符串
来源：http://hz.aizwys.cn/gtyzarhzrm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.fzhhl.top/gtllszputo.html

PHP:  implode(", ", $arr);
来源：http://hz.gaohongyu789.top/gtjctxzlyk.html

JS:   arr.join(", ")
来源：http://hz.haohaochexian.top/gtluovbfeu.html

TS:   arr.join(", ")
来源：http://hz.ydzc1.top/gtfpdsbptk.html

Java: String.join(", ", list)
来源：http://hz.wangshuangyany.cn/gtpzgjmqit.html

Go:   strings.Join(strs, ", ")
来源：http://hz.mhx1999.top/gtkvygbhax.html

Ruby: arr.join(", ")
来源：http://hz.yonumen.top/gtgbobsenf.html

C#:   string.Join(", ", list)
来源：http://hz.gaohongyu789.top/gtmesrjqzh.html

================================================================================
来源：http://hz.xuanzx.com/gtazoxmdoh.html

E. 字符串处理
来源：http://hz.9152youxi.cn/gtxcmmomgi.html

================================================================================
来源：http://hz.sufxvd.cn/gtnnbyjmsn.html

[E01] 拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtmervkgsq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.kuanghao11.cn/gtbrpilspb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinqigfzy.top/gtivlwdbxb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.dashuyun.cn/gtxpuszchj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenlongwang.top/gtirxyhqvw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yangfankeji.com/gtiqkscohh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.haohaochexian.top/gtqseuczco.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tian-w.cn/gthqpefryd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.fzhhl.top/gtcrerdhto.html

[E02] 重复字符串
来源：http://hz.zycfv.cn/gtnrlkphks.html

Py:   "ab" * 3
来源：http://hz.yvedp.cn/gtxoazubhy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cashguo.top/gtbgnrcgvt.html

JS:   "ab".repeat(3)
来源：http://hz.chenjidiqi.icu/gtrumjlkin.html

TS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtbzkhuaca.html

Java: "ab".repeat(3)
来源：http://hz.tian-w.cn/gtppksfrpf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.chenjidiqi.icu/gtnsoevcys.html

Ruby: "ab" * 3
来源：http://hz.ivvv.top/gtyozhtoxo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yangfankeji.com/gtvpnhbwzb.html

[E03] 截取子串
来源：http://hz.kuanghao11.cn/gtvhpnpmyw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhaomingkeji.xyz/gtstzfzgox.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.sysykeji.top/gtkguhmxrh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jlsjyb.cn/gtwmopbpik.html

TS:   s.slice(1, 4)
来源：http://hz.guowangkeji.top/gtlkmymuwi.html

Java: s.substring(1, 4)
来源：http://hz.zhoulong.xyz/gtibmbefnp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.quarkkingdee.top/gtgoafrxqd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.snrcjt.cn/gtqskxlpgf.html

C#:   s.Substring(1, 3)
来源：http://hz.aibaodan.cn/gtvuiasxdx.html

[E04] 查找子串位置
来源：http://hz.xingfuxueyuan.xyz/gtlicxqjzt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yj202588.top/gtumzpmznl.html

PHP:  strpos($s, "x");
来源：http://hz.yanxiufei.cn/gtxtlewgct.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jinqigfzy.top/gtvmfbrqmu.html

TS:   s.indexOf("x")
来源：http://hz.ehwqpu.com/gtvwohurmb.html

Java: s.indexOf("x")
来源：http://hz.nanxuanxn.top/gttytcoxuc.html

Go:   strings.Index(s, "x")
来源：http://hz.zhengqikj.top/gthbeoehch.html

Ruby: s.index("x")
来源：http://hz.yj20258.top/gtkswcevnm.html

C#:   s.IndexOf("x")
来源：http://hz.chenzaomai.com/gtpcwzqfiv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.svipenyu.cn/gtkvobsjyd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.tian-w.cn/gtmtzmfcvw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinghuilouyu.cn/gtvuhpnpfq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.birdmap.top/gtahtvefhw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.0kj1m.cn/gtqknpyjri.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cqqwz.cn/gtoefvpssl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ppjwa.cn/gtkibqsvxq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yuxming.cn/gticrblhgp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.svipenyu.cn/gtqihlfbie.html

[E06] 替换子串
来源：http://hz.havefunace.top/gtcydhoqbs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.fengsongda.top/gtsavtrzoj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xuanzx.com/gtieucysad.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtzrzuwnay.html

TS:   s.replaceAll("a", "b")
来源：http://hz.52xcode.cn/gtyvjefgnn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtdmvzlrqh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yuxming.cn/gtquzabyns.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ivvv.top/gtxihruhka.html

C#:   s.Replace("a", "b")
来源：http://hz.cashguo.top/gtmbbcufgu.html

[E07] 按分隔符拆分
来源：http://hz.wangdashe.top/gthgvhobeo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hnqzz.top/gtqkeqngey.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.bjfxy.top/gtrphnhadg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.aibaodan.cn/gtedhrmrds.html

TS:   s.split(",")
来源：http://hz.zhiwuduotai.top/gtbdgsmzxf.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhengqikj.top/gtklooazyi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.feifeiyinyue.top/gtlxnkzpky.html

Ruby: s.split(",");  s.split
来源：http://hz.ywan-chungtsiang.top/gtruecyjfb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.aibaodan.cn/gtuevvmsvj.html

[E08] 数组按分隔符合并
来源：http://hz.svipenyu.cn/gtueybndxj.html

Py:   ",".join(items)
来源：http://hz.yanxiufei.cn/gtusgtzdsx.html

PHP:  implode(",", $items);
来源：http://hz.c1oappe.top/gtsfhqvnam.html

JS:   items.join(",")
来源：http://hz.cdnleiting.top/gtbhacbzjl.html

TS:   items.join(",")
来源：http://hz.shangyingyoupin.top/gtmzxhzcxm.html

Java: String.join(",", items)
来源：http://hz.hfpthk.cn/gtaogbmiua.html

Go:   strings.Join(items, ",")
来源：http://hz.aibaodan.cn/gtizurgtvg.html

Ruby: items.join(",")
来源：http://hz.0kj1m.cn/gtxzgshmbu.html

C#:   string.Join(",", items)
来源：http://hz.yuanzhike.top/gtbdqfrugc.html

[E09] 去除所有空白字符
来源：http://hz.xuanzx.com/gticrnrhau.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.chenlongwang.top/gtepdprvkt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinghuilouyu.cn/gthmkpqudu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yanxiufei.cn/gtbwssibbr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yonumen.top/gtmkorpbmq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.52xcode.cn/gtaaayoqjb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.chenlongwang.top/gtqsrdyfht.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhiwuduotai.top/gtzmdrstjj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.tianlin.xyz/gtlkbmjiar.html

[E10] 左侧补零 / 定长填充
来源：http://hz.fengsongda.top/gtrmribhdn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.quarkkingdee.top/gtyrgkgfrx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ivvv.top/gtfgqxqlht.html

JS:   "7".padStart(3, "0")
来源：http://hz.bjfxy.top/gtlfpmmksx.html

TS:   "7".padStart(3, "0")
来源：http://hz.iojbl.cn/gtfxlnfuau.html

Java: String.format("%03d", 7)
来源：http://hz.svipenyu.cn/gtolxbrhlk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.9152youxi.cn/gtrplcwhpc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtnldkjlxk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenjidiqi.icu/gtomwatfxd.html

[E11] 反转字符串
来源：http://hz.yongpay.top/gtuqjlgcml.html

Py:   s[::-1]
来源：http://hz.guowangkeji.top/gtiwfopbbp.html

PHP:  strrev($s);
来源：http://hz.zhiwuduotai.top/gtfmugeeey.html

JS:   [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtxxujxqmd.html

TS:   [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtfhpjadbp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cheryme.top/gtefssirbk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ppjwa.cn/gtmmxuinln.html

Ruby: s.reverse
来源：http://hz.zhoulong.xyz/gthekayhsk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dashuyun.cn/gtycqbypri.html

[E12] 统计某字符出现次数
来源：http://hz.ybcxt.top/gttkpeswps.html

Py:   s.count("a")
来源：http://hz.hywenlv.cn/gtaixbymxp.html

PHP:  substr_count($s, "a");
来源：http://hz.yongpay.top/gtvkumsalj.html

JS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gtjdniyhwm.html

TS:   s.split("a").length - 1
来源：http://hz.havefunace.top/gtfoppvvlr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinyuanbaomall.cn/gtjtqzlvpk.html

Go:   strings.Count(s, "a")
来源：http://hz.xingfuxueyuan.xyz/gttifzctrs.html

Ruby: s.count("a")
来源：http://hz.zhiwuduotai.top/gtfvmxdgzq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhongyouzk.top/gtlqqibwmo.html

[E13] 逐字符遍历
来源：http://hz.xuetiantiany.cn/gtiiosihup.html

Py:   for ch in s: print(ch)
来源：http://hz.daxiang520.top/gtfbohqwqz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yj202588.top/gtzotmaqlr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cdnleiting.top/gthjarwjli.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangshuangyany.cn/gtpwwgdyem.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ywan-chungtsiang.top/gtzcmsxdob.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.52xcode.cn/gtczsdupor.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinghuilouyu.cn/gtvsfurapi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhiwuduotai.top/gtczpnizih.html

[E14] URL 编码与 Base64
来源：http://hz.birdmap.top/gtutngczbx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhongyouzk.top/gtpfjrluyn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.havefunace.top/gtkdrttirb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.dianchejie.cn/gtknysvezf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fzhhl.top/gtasuitvpa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangdashe.top/gtstvfdzba.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yuxming.cn/gtiqbskrdz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhengqikj.top/gtkongmfzk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.tanke756.top/gtgryasqfy.html

[E15] HTML 转义 / 反转义
来源：http://hz.shanyushiyangtech.top/gtowycknwn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jqgfzy.top/gttfjjvsdz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenlongwang.top/gtjkmnncsk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yongpay.top/gtaviiljfm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ydzc1.top/gthnluttct.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenzaomai.com/gtwfophpld.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yonumen.top/gtsrsizqrq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xuanzx.com/gtxbvlyxgw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.daxiang520.top/gtjyoopemo.html

[E16] 数字千分位
来源：http://hz.xuanzx.com/gtzgtaivwh.html

Py:   f"{1234567:,}"
来源：http://hz.yongpay.top/gtdymqbrww.html

PHP:  number_format(1234567);
来源：http://hz.quarkkingdee.top/gtufbvnxme.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hywenlv.cn/gtdzanniwf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhijiandao.cn/gtaixzunes.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ydjk.org.cn/gtbkodnpxx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gaohongyu789.top/gtoozkndhx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gzhubu.top/gtcaiwcttk.html

C#:   1234567.ToString("N0")
来源：http://hz.birdmap.top/gtbskomrjo.html

[E17] 首字母大写
来源：http://hz.zhijiandao.cn/gtqgvfbvop.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hfpthk.cn/gtskjcbuqd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sxryk.cn/gtmcyenpzj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xziqi.cn/gtqqaemnwt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgufenzy.top/gtybddvpwu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yj20258888.top/gtrpajalbg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yuxming.cn/gtmrmobxnq.html

Ruby: s.capitalize
来源：http://hz.jiagoushi.top/gtvcxqrmra.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tian-w.cn/gtxnvslubp.html

[E18] 模板占位符替换
来源：http://hz.yanxiufei.cn/gtlopknmwz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xziqi.cn/gtinnbamdu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ydjk.org.cn/gtxhavoyrx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.dianchejie.cn/gtudjsrpzu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tianlin.xyz/gtbrurhjcn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.andypj.xyz/gtdvkdaovk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhixingplan.top/gtxnfcwkze.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gaohongyu789.top/gtolrncaml.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ehwqpu.com/gttuvkqhas.html

[E19] 多行文本按行拆分
来源：http://hz.xylfe.cn/gtnfprvhao.html

Py:   s.splitlines()
来源：http://hz.yueranfly.top/gtcfqdmvxz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shanyushiyangkeji.top/gtmbouqrdq.html

JS:   s.split(/\r?\n/)
来源：http://hz.cucudq.cn/gtbmxvjcxw.html

TS:   s.split(/\r?\n/)
来源：http://hz.pengpengdd.cyou/gtsswoecyw.html

Java: s.lines().toList()
来源：http://hz.guowangkeji.top/gtmtxvvbgg.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj20258888.top/gtwyohzaeu.html

Ruby: s.lines
来源：http://hz.aizwys.cn/gtixavpbsz.html

C#:   s.Split('\n')
来源：http://hz.316326.xyz/gtfksikgsd.html

[E20] 判断字符串是否为空
来源：http://hz.yueranfly.top/gtcesgkyob.html

Py:   if not s:
来源：http://hz.havefunace.top/gtscnsyynv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigufen.top/gtbptbqtrq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinyuanbaomall.cn/gtxcodepts.html

TS:   if (s === "") {}
来源：http://hz.jiagoushi.top/gtlrptclsw.html

Java: if (s.isEmpty()) {}
来源：http://hz.dianchejie.cn/gttlotrlrk.html

Go:   if s == "" {}
来源：http://hz.jianghu66.top/gtcgmiyqel.html

Ruby: if s.empty?
来源：http://hz.fengsongda.top/gtoblazuve.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xziqi.cn/gtzhfqbqlj.html

[E21] 超长截断加省略号
来源：http://hz.jinqigfzy.top/gtqxwdqgbm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.bjfxy.top/gtrwzkeesn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yonumen.top/gtizelmogw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtzdfntwfk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtoycwiyav.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gtyxzfargl.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhixingplan.top/gtlglhseut.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtugtdlzrn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tanke756.top/gtsfrzpzuc.html

[E22] 字节长度与字符长度
来源：http://hz.xziqi.cn/gthnnqotqh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.kuanghao11.cn/gthcyauytn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guannengcc.top/gtiukcmhqi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xziqi.cn/gtovofsuqu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydjk.org.cn/gtneiwvpjf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sxryk.cn/gtuyguenli.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yanxiufei.cn/gtkitirbin.html

Ruby: s.bytesize;  s.length
来源：http://hz.nanxinkj.top/gtxxvetrot.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cucudq.cn/gtczjbwggd.html

================================================================================
来源：http://hz.snrcjt.cn/gtlssnnaeo.html

F. 文件与目录
来源：http://hz.jqgfzy.top/gtmtambmlx.html

================================================================================
来源：http://hz.fengsongda.top/gtrldyviae.html

[F01] 读取整个文件
来源：http://hz.jinyuanbaomall.cn/gtjpcppbwz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.shuidangran.top/gtsifhxdus.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gaohongyu789.top/gtrcnixeeg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ybcxt.top/gtkuukfsmr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jianghu66.top/gtwrnkcrmv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtmcbfqcra.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yanxiufei.cn/gtstlkofnd.html

Ruby: File.read("a.txt")
来源：http://hz.zhijiandao.cn/gtsmalgofh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gogol.net.cn/gtmibymrys.html

[F02] 逐行读取文件
来源：http://hz.yvedp.cn/gtsgtulyul.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.52xcode.cn/gtfaqknakw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shanyushiyangtech.top/gtnuvvufyo.html


<!-- 参考信息 -->