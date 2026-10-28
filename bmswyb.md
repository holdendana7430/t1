代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ydjk.org.cn/gtvyaqiyyf.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj202588.top/gtikpmfaqg.html

[D17] 最大值与最小值
来源：http://hz.xuetiantiany.cn/gtgxvteghz.html

Py:   max(arr);  min(arr)
来源：http://hz.zhiwuduotai.top/gtjdrhiudk.html

PHP:  max($arr);  min($arr);
来源：http://hz.ydzc1.top/gtktnpsmjj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tian-w.cn/gtwapakerf.html

TS:   Math.max(...arr);
来源：http://hz.kuanghao11.cn/gtnbfeawjs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ivvv.top/gtpctsagwm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.quarkkingdee.top/gtxekubovd.html

Ruby: arr.max;  arr.min
来源：http://hz.snrcjt.cn/gtexdwebwi.html

C#:   list.Max();  list.Min()
来源：http://hz.xziqi.cn/gtpzbnpmma.html

[D18] 扁平化嵌套数组
来源：http://hz.yonumen.top/gtzosznszd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hfpthk.cn/gtpqxxyzah.html

PHP:  array_merge(...$nested);
来源：http://hz.sysykeji.top/gtexbzlagm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jiagoushi.top/gtavcbfwge.html

TS:   nested.flat();
来源：http://hz.hywenlv.cn/gttymmjkvy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hnqzz.top/gtnbaxhxop.html

Go:   // 手写双层循环
来源：http://hz.cashguo.top/gtntqiuvrc.html

Ruby: nested.flatten
来源：http://hz.dianchejie.cn/gtdmkxlnjd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shzxlz.cn/gtthuudzub.html

[D19] 按字段分组
来源：http://hz.zhijiandao.cn/gtuiwclmxp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ydzc1.top/gtujzboleu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shuidangran.top/gtixjjtenm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.fengsongda.top/gtrbaovunt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yueranfly.top/gtuhhmtetv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sysykeji.top/gtomzbeuln.html

Go:   // 手写 map[string][]T
来源：http://hz.quarkkingdee.top/gtikvwujue.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.daria6918.cn/gtrpsbbaxx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ywan-chungtsiang.top/gtyrdrnbba.html

[D20] 统计每个元素出现次数
来源：http://hz.cucudq.cn/gtcknhuhqb.html

Py:   Counter(arr)
来源：http://hz.yueranfly.top/gtbqwuwavv.html

PHP:  array_count_values($arr);
来源：http://hz.52xcode.cn/gtxgdrfkbs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgufenzy.top/gtdkefyzau.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yonumen.top/gtyfvhbowe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yueranfly.top/gtqipgtnvn.html

Go:   // 手写 map[T]int
来源：http://hz.nanxuanxn.top/gtvfsupoxi.html

Ruby: arr.tally
来源：http://hz.gogol.net.cn/gtrlancmzr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.quarkkingdee.top/gtclqeaonx.html

[D21] 判断是否包含某元素
来源：http://hz.xziqi.cn/gthbfoncqa.html

Py:   x in arr
来源：http://hz.bjfxy.top/gtbzfgoqqq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.aibaodan.cn/gteiawbkup.html

JS:   arr.includes(x)
来源：http://hz.chenjidiqi.icu/gtygeqlnev.html

TS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtaorjuthr.html

Java: list.contains(x)
来源：http://hz.guowangkeji.top/gtthbcoomh.html

Go:   slices.Contains(arr, x)
来源：http://hz.jianghu66.top/gtnxpaphao.html

Ruby: arr.include?(x)
来源：http://hz.cqqwz.cn/gtjvhdlnnm.html

C#:   list.Contains(x)
来源：http://hz.shzxlz.cn/gtsfxbkhwl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.pycfn.com/gtmxbigfsf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.daria6918.cn/gtdvoibvtw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cdnleiting.top/gtgkgcymkw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.guannengcc.top/gtuyqnzxlw.html

TS:   [...arr];
来源：http://hz.jinghuilouyu.cn/gtounzqtam.html

Java: new ArrayList<>(list);
来源：http://hz.chenjidiqi.icu/gtildyuowi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gaohongyu789.top/gtgyyjzptx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhijiandao.cn/gtsbkvxbfi.html

C#:   new List<int>(list);
来源：http://hz.jlsjyb.cn/gtteerdjhw.html

[D23] reduce 累积计算
来源：http://hz.nanxuanxn.top/gtyuswjgop.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.shuidangran.top/gtypegcsfl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xylfe.cn/gtswjqakdr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtpoydetds.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gtzlljyyct.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jiagoushi.top/gtytmwbqha.html

Go:   // 手写循环
来源：http://hz.xuanzx.com/gtjxjvgsfr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.quarkkingdee.top/gttfaqeubc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cashguo.top/gtygelpvhr.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhixingplan.top/gtbbznssby.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shanyushiyangkeji.top/gtupxsyabp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.pengpengdd.cyou/gtjnnuwczx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhengqikj.top/gtncsrezme.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.c1oappe.top/gtnjumoipk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sweek.top/gtfaziuswb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhixingplan.top/gtkwtavprh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shzxlz.cn/gtyfmormnq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ppjwa.cn/gtfztlulpe.html

[D25] Set 集合去重与交并差
来源：http://hz.svipenyu.cn/gthnfcytim.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.pengpengdd.cyou/gtkqcyghfj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.guannengcc.top/gtpjhnhekm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nwbrower.top/gtslixzwtj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sweek.top/gtbnddrtgk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.svipenyu.cn/gtucmnvyfh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.pycfn.com/gtgjpbfume.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.birdmap.top/gtztfvujla.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yanxiufei.cn/gtdexbxeab.html

[D26] 数组转字符串
来源：http://hz.yongpay.top/gtucacmzhq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sweek.top/gtnhpjtrrn.html

PHP:  implode(", ", $arr);
来源：http://hz.jianghu66.top/gtnlpwgkes.html

JS:   arr.join(", ")
来源：http://hz.pengpengdd.cyou/gtnhhzdkyl.html

TS:   arr.join(", ")
来源：http://hz.guowangkeji.top/gtqotmpwvg.html

Java: String.join(", ", list)
来源：http://hz.cashguo.top/gtxsqumdox.html

Go:   strings.Join(strs, ", ")
来源：http://hz.feifeiyinyue.top/gteaagtfse.html

Ruby: arr.join(", ")
来源：http://hz.xylfe.cn/gthmiakiyi.html

C#:   string.Join(", ", list)
来源：http://hz.feifeiyinyue.top/gtclcbrhyl.html

================================================================================
来源：http://hz.hysaishi.cn/gtquijjlrf.html

E. 字符串处理
来源：http://hz.xuetiantiany.cn/gtrconxtfu.html

================================================================================
来源：http://hz.zdqjudy.top/gtusmrbitr.html

[E01] 拼接字符串
来源：http://hz.pengpengdd.cyou/gtxtjdypkq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj20258.top/gtbbeefbzk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.smart0.xyz/gtwyibuwuz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hysaishi.cn/gtwjkkbaql.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yangfankeji.com/gtieavnlpo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zdqjudy.top/gtxggwgjkn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.tanke756.top/gttivbuyno.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenlongwang.top/gtdjqhdggh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hfpthk.cn/gtipqeuyju.html

[E02] 重复字符串
来源：http://hz.nwbrower.top/gtwognhjls.html

Py:   "ab" * 3
来源：http://hz.vqdsnc.cn/gtbztzumzm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yuxming.cn/gtnjhavipe.html

JS:   "ab".repeat(3)
来源：http://hz.ehwqpu.com/gtydwkitze.html

TS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtyheeayav.html

Java: "ab".repeat(3)
来源：http://hz.yonumen.top/gtxmzjthpy.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zdqjudy.top/gttuapwdjg.html

Ruby: "ab" * 3
来源：http://hz.nanxuanxn.top/gtkqjaxezh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shangyingyoupin.top/gtufrpdpti.html

[E03] 截取子串
来源：http://hz.ywan-chungtsiang.top/gtnmdcruqk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinghuilouyu.cn/gtyvlqperh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gttqcteppe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.daxiang520.top/gtvjysbckf.html

TS:   s.slice(1, 4)
来源：http://hz.svipenyu.cn/gtjmlluszd.html

Java: s.substring(1, 4)
来源：http://hz.tianlin.xyz/gtfggvfbid.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jiagoushi.top/gtthkxqbue.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yj20258888.top/gtgbwikrez.html

C#:   s.Substring(1, 3)
来源：http://hz.hywenlv.cn/gttquenrhv.html

[E04] 查找子串位置
来源：http://hz.0kj1m.cn/gtuadbcfrp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hywenlv.cn/gtxacvvjnk.html

PHP:  strpos($s, "x");
来源：http://hz.yanxiufei.cn/gthuunxrfv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hysaishi.cn/gtuvynmrno.html

TS:   s.indexOf("x")
来源：http://hz.zhijiandao.cn/gtohrjykkc.html

Java: s.indexOf("x")
来源：http://hz.zhoulong.xyz/gteylxpqqs.html

Go:   strings.Index(s, "x")
来源：http://hz.meibo888.top/gthjoscsjx.html

Ruby: s.index("x")
来源：http://hz.gogol.net.cn/gttwquvymi.html

C#:   s.IndexOf("x")
来源：http://hz.hysaishi.cn/gtrtxzvtrb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ehwqpu.com/gtucfhmapq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jinqigufen.top/gtefeoqcbs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ybcxt.top/gtcznakhpq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xinyue.icu/gtmsjnxguy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yangfankeji.com/gtscnviohc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.wangshuangyany.cn/gtqmaoqofc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nanxinkj.top/gtygmutocm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.andypj.xyz/gtbzvumevg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.nwbrower.top/gtxktyrudr.html

[E06] 替换子串
来源：http://hz.gotoacloud.top/gttflspgqd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hywenlv.cn/gtutjarfpt.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xuetiantiany.cn/gtknsllool.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtnfcohamz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtibcanzfs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtshihoeox.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gaohongyu789.top/gtuamhupar.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xuanzx.com/gtykpbzalq.html

C#:   s.Replace("a", "b")
来源：http://hz.pycfn.com/gtsaglwblo.html

[E07] 按分隔符拆分
来源：http://hz.zhixingplan.top/gtcgqjjjfd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sweek.top/gttguqunel.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yonumen.top/gteupvwrnq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhoulong.xyz/gtpmnzplyf.html

TS:   s.split(",")
来源：http://hz.ybcxt.top/gtszoacbod.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinghuilouyu.cn/gtybzggivr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cqqwz.cn/gtuydplwxe.html

Ruby: s.split(",");  s.split
来源：http://hz.jiagoushi.top/gtefybjqej.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.fengsongda.top/gtfusstcfg.html

[E08] 数组按分隔符合并
来源：http://hz.shuidangran.top/gtaumxlyig.html

Py:   ",".join(items)
来源：http://hz.guannengcc.top/gtfojtpecr.html

PHP:  implode(",", $items);
来源：http://hz.sufxvd.cn/gtqgosebec.html

JS:   items.join(",")
来源：http://hz.0kj1m.cn/gtzapsdhzx.html

TS:   items.join(",")
来源：http://hz.hywenlv.cn/gtjeisuvrd.html

Java: String.join(",", items)
来源：http://hz.xinyue.icu/gtvtymnpef.html

Go:   strings.Join(items, ",")
来源：http://hz.wangdashe.top/gtmeesjuwb.html

Ruby: items.join(",")
来源：http://hz.xylfe.cn/gtlhllhley.html

C#:   string.Join(",", items)
来源：http://hz.bjfxy.top/gtyiywyund.html

[E09] 去除所有空白字符
来源：http://hz.zycfv.cn/gtgbsbfjlf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.daxiang520.top/gtfseaqtpr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.feifeiyinyue.top/gtxyqzldmm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hfpthk.cn/gtawelwdcx.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zycfv.cn/gtzgchmndp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.redwolf501.top/gtmtzdgmim.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jinqigufen.top/gtnnojeuaf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cashguo.top/gtlusshxrv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ybcxt.top/gtdgofrldz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guowangkeji.top/gtesixyymj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.havefunace.top/gtfoovmgfv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.iojbl.cn/gtckusemcm.html

JS:   "7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtffahnrkp.html

TS:   "7".padStart(3, "0")
来源：http://hz.yongpay.top/gtxvbvxqat.html

Java: String.format("%03d", 7)
来源：http://hz.ppjwa.cn/gtjtibwhay.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sweek.top/gtgnaiqdks.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.andypj.xyz/gtrsvythql.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xuetiantiany.cn/gtxkxdrrws.html

[E11] 反转字符串
来源：http://hz.tian-w.cn/gtzoqbhhlf.html

Py:   s[::-1]
来源：http://hz.dashuyun.cn/gtlnxlecsw.html

PHP:  strrev($s);
来源：http://hz.guannengcc.top/gtlthdrine.html

JS:   [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtnllagkbx.html

TS:   [...s].reverse().join("")
来源：http://hz.havefunace.top/gtrrctcfka.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ppjwa.cn/gtlpqlrjlq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.bjfxy.top/gtpevcqjqe.html

Ruby: s.reverse
来源：http://hz.0kj1m.cn/gttvcmqlfj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cdnleiting.top/gtqjvpfrwp.html

[E12] 统计某字符出现次数
来源：http://hz.daxiang520.top/gtprcvulip.html

Py:   s.count("a")
来源：http://hz.xylfe.cn/gtxaebpbjm.html

PHP:  substr_count($s, "a");
来源：http://hz.yuxming.cn/gtrqsqrgbm.html

JS:   s.split("a").length - 1
来源：http://hz.yj20258.top/gtihjcxtkj.html

TS:   s.split("a").length - 1
来源：http://hz.dianchejie.cn/gtsuktnngk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hywenlv.cn/gtyrgmyiif.html

Go:   strings.Count(s, "a")
来源：http://hz.sufxvd.cn/gtryugjqxj.html

Ruby: s.count("a")
来源：http://hz.nanxuanxn.top/gterphjlwa.html

C#:   s.Count(c => c == 'a')
来源：http://hz.9152youxi.cn/gtweqjvarr.html

[E13] 逐字符遍历
来源：http://hz.wangshuangyany.cn/gtcnaetpnh.html

Py:   for ch in s: print(ch)
来源：http://hz.zhijiandao.cn/gtcqqhynmy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yj20258888.top/gtaembbdtv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.mhx1999.top/gtbiuimjbk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dashuyun.cn/gtgjcqomtz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yj20258.top/gthmbghsmp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.pycfn.com/gtzykrzgez.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.tianlin.xyz/gtlodidqbz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.pengpengdd.cyou/gtecbrypks.html

[E14] URL 编码与 Base64
来源：http://hz.xinyue.icu/gtdztvwipd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.quarkkingdee.top/gtzytrrzfm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhixingplan.top/gtvewoipnz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.svipenyu.cn/gtglkjsskf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sweek.top/gtqtniuyai.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sxryk.cn/gtofmxlcsv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shuidangran.top/gtnqpmyiac.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhixingplan.top/gthbedfguw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinghuilouyu.cn/gtvzrkxher.html

[E15] HTML 转义 / 反转义
来源：http://hz.meibo888.top/gtehtcvsty.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xylfe.cn/gtwfibxxsx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.vqdsnc.cn/gtsyyvsdrq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.vqdsnc.cn/gtmyeejyin.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhongyouzk.top/gtdonjrdqo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sweek.top/gtufzhysos.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cheryme.top/gtanahxatq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.wangdashe.top/gtwakctrca.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.pycfn.com/gtdlugnwgu.html

[E16] 数字千分位
来源：http://hz.quarkkingdee.top/gtpehvzqhk.html

Py:   f"{1234567:,}"
来源：http://hz.guannengcc.top/gtccitflqj.html

PHP:  number_format(1234567);
来源：http://hz.iojbl.cn/gtlnxwpehs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gotoacloud.top/gttlywgqqh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fzhhl.top/gtqssvrpwv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhijiandao.cn/gtunfatvcf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nanxuanxn.top/gtaqnwjejj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cashguo.top/gtqwvuorpx.html

C#:   1234567.ToString("N0")
来源：http://hz.zhijiandao.cn/gtasptpgkt.html

[E17] 首字母大写
来源：http://hz.jqgfzy.top/gtmfgambjq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nwbrower.top/gtkcygtxvp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sweek.top/gtbseslyrq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuanzx.com/gthuawpdkj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guowangkeji.top/gtgzuczkza.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daria6918.cn/gtkaeuenjo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ppjwa.cn/gtzhgpqjzn.html

Ruby: s.capitalize
来源：http://hz.316326.xyz/gtlrfzfyqf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258.top/gtvfcirqsd.html

[E18] 模板占位符替换
来源：http://hz.shanyushiyangkeji.top/gtuhlxluwv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ydzc1.top/gtaztqpgmw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xylfe.cn/gtlpxizwyq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.havefunace.top/gtynobbvra.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yueranfly.top/gtodjyhuuw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hongshengwenyu.top/gtaeajahwb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.daxiang520.top/gtyjdbahuy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sxryk.cn/gtsvqhqplb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.gzhubu.top/gttfzcfaja.html

[E19] 多行文本按行拆分
来源：http://hz.havefunace.top/gtiuuvfjlg.html

Py:   s.splitlines()
来源：http://hz.hammf.cn/gtjhmhprwo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xziqi.cn/gtmmotvvjx.html

JS:   s.split(/\r?\n/)
来源：http://hz.ppjwa.cn/gtlxoqbslk.html

TS:   s.split(/\r?\n/)
来源：http://hz.tanke756.top/gtdjmsjubd.html

Java: s.lines().toList()
来源：http://hz.zhijiandao.cn/gtqxfuurnj.html

Go:   strings.Split(s, "\n")
来源：http://hz.guannengcc.top/gtslrunhyt.html

Ruby: s.lines
来源：http://hz.yueranfly.top/gttbtmukle.html

C#:   s.Split('\n')
来源：http://hz.bjfxy.top/gtzsqyiqde.html

[E20] 判断字符串是否为空
来源：http://hz.daria6918.cn/gtiayxmzdg.html

Py:   if not s:
来源：http://hz.fengsongda.top/gthwhkshus.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.dashuyun.cn/gtdweikmbz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.aibaodan.cn/gtfqsqouox.html

TS:   if (s === "") {}
来源：http://hz.xinyue.icu/gtypkdhjwr.html

Java: if (s.isEmpty()) {}
来源：http://hz.hongshengwenyu.top/gtyikuahbp.html

Go:   if s == "" {}
来源：http://hz.ydzc1.top/gtcjpullgw.html

Ruby: if s.empty?
来源：http://hz.pycfn.com/gteihnomzo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shanyushiyangkeji.top/gtxadencgc.html

[E21] 超长截断加省略号
来源：http://hz.fengsongda.top/gtztizvcqs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhoulong.xyz/gtoyaolbif.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.chenzaomai.com/gtcbuopufv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtveaxddtf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtdhuuvnjy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sxryk.cn/gtvzxdgzyd.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.c1oappe.top/gtorzpsomt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.kuanghao11.cn/gtbrfjqbsx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yuxming.cn/gtdebrqctr.html

[E22] 字节长度与字符长度
来源：http://hz.chenzaomai.com/gtosnhimhe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenlongwang.top/gtcyfsdpij.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.svipenyu.cn/gtqwpxmsgd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gtaichpbjg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtvaiukscs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cucudq.cn/gtuonbdsqc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ybcxt.top/gtdxxftwpx.html

Ruby: s.bytesize;  s.length
来源：http://hz.yvedp.cn/gtkpzgjefk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yvedp.cn/gtcymhmonm.html

================================================================================
来源：http://hz.yvedp.cn/gtgbmamuqu.html

F. 文件与目录
来源：http://hz.hywenlv.cn/gtdasfxguv.html

================================================================================
来源：http://hz.gzhubu.top/gtksgxlfoq.html

[F01] 读取整个文件
来源：http://hz.jyoumei.cn/gtqzpisxfh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.smart0.xyz/gtfflnrvrh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sxryk.cn/gtvifwoodw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cqqwz.cn/gtuxztlbev.html


<!-- 参考信息 -->