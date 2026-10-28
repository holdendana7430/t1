代发 wailian999

TS:   [...new Set(arr)]
来源：http://hz.shuidangran.top/gtpiffkidf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.tian-w.cn/gtjcypkdsw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tian-w.cn/gtynsxjjmm.html

Ruby: arr.uniq
来源：http://hz.pengpengdd.cyou/gtrwomoamg.html

C#:   list.Distinct().ToList()
来源：http://hz.xingfuxueyuan.xyz/gtymiemlxq.html

[D16] 求和与平均值
来源：http://hz.sxryk.cn/gtvbowpjgr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.smart0.xyz/gtvjkaykwj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenjidiqi.icu/gtrxpxfbcw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tian-w.cn/gteqqbevom.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.kuanghao11.cn/gtzrkhmohs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hfpthk.cn/gtzdqpiooz.html

Go:   // 手写循环累加
来源：http://hz.fengsongda.top/gtvneidwre.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.aibaodan.cn/gteunuhbgl.html

C#:   list.Sum();  list.Average()
来源：http://hz.smart0.xyz/gtpnmsbzic.html

[D17] 最大值与最小值
来源：http://hz.chenlongwang.top/gtaljkvidp.html

Py:   max(arr);  min(arr)
来源：http://hz.zycfv.cn/gtkzedecgb.html

PHP:  max($arr);  min($arr);
来源：http://hz.jiagoushi.top/gtvpbnhcbb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dashuyun.cn/gtyqogekyp.html

TS:   Math.max(...arr);
来源：http://hz.yanxiufei.cn/gtngonmnco.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cucudq.cn/gtmalvlebq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenlongwang.top/gtpdkyhbhh.html

Ruby: arr.max;  arr.min
来源：http://hz.yongpay.top/gtybalcojk.html

C#:   list.Max();  list.Min()
来源：http://hz.pycfn.com/gtewschfjy.html

[D18] 扁平化嵌套数组
来源：http://hz.ppjwa.cn/gtemgxnpfo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.havefunace.top/gtjdtafccz.html

PHP:  array_merge(...$nested);
来源：http://hz.jlsjyb.cn/gtnrihnrqc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yj202588.top/gtedexfgvq.html

TS:   nested.flat();
来源：http://hz.yuxming.cn/gtuyeifecm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ywan-chungtsiang.top/gtjzcobkjl.html

Go:   // 手写双层循环
来源：http://hz.meibo888.top/gtcxlcbyls.html

Ruby: nested.flatten
来源：http://hz.yonumen.top/gtnfoslmwu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinghuilouyu.cn/gtpndygbre.html

[D19] 按字段分组
来源：http://hz.yangfankeji.com/gtjrjulgku.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yuxming.cn/gtjecbjbbx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sweek.top/gtpsfhmhyv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.pycfn.com/gtzmgtnxey.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.vqdsnc.cn/gthadvhbzp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.52xcode.cn/gtqujnewpq.html

Go:   // 手写 map[string][]T
来源：http://hz.yangfankeji.com/gtlokrecgy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.havefunace.top/gtqfwkrvte.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhongyouzk.top/gtdojkntns.html

[D20] 统计每个元素出现次数
来源：http://hz.snrcjt.cn/gtaruivnyg.html

Py:   Counter(arr)
来源：http://hz.tanke756.top/gtdsztaxzo.html

PHP:  array_count_values($arr);
来源：http://hz.chenzaomai.com/gtqfcjhqjj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tianlin.xyz/gtpgaybqgy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.iojbl.cn/gtxidmqdgb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhaomingkeji.xyz/gtkulkuqzb.html

Go:   // 手写 map[T]int
来源：http://hz.mhx1999.top/gtwxbmpxje.html

Ruby: arr.tally
来源：http://hz.guannengcc.top/gtqargyyqn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yuxming.cn/gtjxfcwara.html

[D21] 判断是否包含某元素
来源：http://hz.ywan-chungtsiang.top/gthruhwxai.html

Py:   x in arr
来源：http://hz.hywenlv.cn/gtknlppzds.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yangfankeji.com/gtbsltcehw.html

JS:   arr.includes(x)
来源：http://hz.gotoacloud.top/gtumbmsdij.html

TS:   arr.includes(x)
来源：http://hz.xuetiantiany.cn/gtskmebrkg.html

Java: list.contains(x)
来源：http://hz.shangyingyoupin.top/gtdklsnukz.html

Go:   slices.Contains(arr, x)
来源：http://hz.ybcxt.top/gtjmnjupbc.html

Ruby: arr.include?(x)
来源：http://hz.ydjk.org.cn/gtvtedxras.html

C#:   list.Contains(x)
来源：http://hz.yangfankeji.com/gtahqdagul.html

[D22] 复制数组（避免共享引用）
来源：http://hz.feifeiyinyue.top/gtqofpehgq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.vqdsnc.cn/gtwxzeyrua.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xuetiantiany.cn/gtbglkgabc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sysykeji.top/gtlcawvkpg.html

TS:   [...arr];
来源：http://hz.xuanzx.com/gtfymgzhan.html

Java: new ArrayList<>(list);
来源：http://hz.fengsongda.top/gtusfthdmg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sweek.top/gtduicyeil.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhongyouzk.top/gtsjtxuxyn.html

C#:   new List<int>(list);
来源：http://hz.xinyue.icu/gtrineyedt.html

[D23] reduce 累积计算
来源：http://hz.zhengqikj.top/gtxoeolkvt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.aibaodan.cn/gtarcjxmbj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.svipenyu.cn/gtyhkwdend.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yueranfly.top/gtjstxfbmr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shuidangran.top/gtqnnwexyi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ppjwa.cn/gtefnjocpm.html

Go:   // 手写循环
来源：http://hz.hammf.cn/gtynntlfgn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.9152youxi.cn/gtiimlxori.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jiagoushi.top/gtfnuxsvqb.html

[D24] 字典 / Map 基本操作
来源：http://hz.hammf.cn/gtpkbeojvf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gogol.net.cn/gtmqeefudu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gzhubu.top/gtrwetosqq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jqgufenzy.top/gtcupbyfbm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shangyingyoupin.top/gtqpgdiyvz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jianghu66.top/gtlttshted.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.chenjidiqi.icu/gtkwebhscr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.bjfxy.top/gtppmeeclo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.guannengcc.top/gtqebtyucs.html

[D25] Set 集合去重与交并差
来源：http://hz.zhongyouzk.top/gtpbgpvyws.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jinqigufen.top/gtudzoeaux.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zdqjudy.top/gteelvdkaa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.meibo888.top/gtnaqqaucv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.tian-w.cn/gtveauhzld.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gotoacloud.top/gtuwkxjttd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.wangdashe.top/gtgwvsiasu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sxryk.cn/gtzdxlixde.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.havefunace.top/gtbzronbdh.html

[D26] 数组转字符串
来源：http://hz.shangyingyoupin.top/gtjvcccgcw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.9152youxi.cn/gtdxmrontq.html

PHP:  implode(", ", $arr);
来源：http://hz.yonumen.top/gtupateltp.html

JS:   arr.join(", ")
来源：http://hz.zdqjudy.top/gtuvhxlqio.html

TS:   arr.join(", ")
来源：http://hz.aibaodan.cn/gtyjdurald.html

Java: String.join(", ", list)
来源：http://hz.zhixingplan.top/gtgsovmgvy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nanxuanxn.top/gtfcbvksbu.html

Ruby: arr.join(", ")
来源：http://hz.hnxiangtu.top/gtnuhgoelc.html

C#:   string.Join(", ", list)
来源：http://hz.yj20258888.top/gtwvceugqe.html

================================================================================
来源：http://hz.sysykeji.top/gtgruzcsmz.html

E. 字符串处理
来源：http://hz.tian-w.cn/gtczysghdy.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtjzlgyfqi.html

[E01] 拼接字符串
来源：http://hz.tanke756.top/gtqabzzsvo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhijiandao.cn/gtbrqbixau.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.fzhhl.top/gtfbqsrmdx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnxiangtu.top/gthfnltgis.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sweek.top/gtjccfvnkk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yj20258888.top/gtiadgdbcc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ywan-chungtsiang.top/gtwgrqluuh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yonumen.top/gtlbkyqjfb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.guannengcc.top/gtwbdmtfzf.html

[E02] 重复字符串
来源：http://hz.jiagoushi.top/gtogrrqeqt.html

Py:   "ab" * 3
来源：http://hz.cqqwz.cn/gtyniesaxh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cqqwz.cn/gttkefsbzg.html

JS:   "ab".repeat(3)
来源：http://hz.yj202588.top/gtxlbljvro.html

TS:   "ab".repeat(3)
来源：http://hz.gaohongyu789.top/gtwjvrakqi.html

Java: "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtqcszcmtd.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xuetiantiany.cn/gtiyomduho.html

Ruby: "ab" * 3
来源：http://hz.smart0.xyz/gtvezmkegh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hongshengwenyu.top/gtrieronmr.html

[E03] 截取子串
来源：http://hz.cqqwz.cn/gtxilhmkdb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ppjwa.cn/gtganqryvy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cucudq.cn/gttyntkjpt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shanyushiyangtech.top/gthnkjdunx.html

TS:   s.slice(1, 4)
来源：http://hz.jqgufenzy.top/gtuvhqoeur.html

Java: s.substring(1, 4)
来源：http://hz.guannengcc.top/gtzelivebg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ydjk.org.cn/gtxvctmlch.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hammf.cn/gtbfjlmama.html

C#:   s.Substring(1, 3)
来源：http://hz.fzhhl.top/gtkaqbxykb.html

[E04] 查找子串位置
来源：http://hz.pycfn.com/gtifmfwfhx.html

Py:   s.find("x");  s.index("x")
来源：http://hz.52xcode.cn/gtujnpradn.html

PHP:  strpos($s, "x");
来源：http://hz.9152youxi.cn/gthuddppxv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yuxming.cn/gtwgrohzhd.html

TS:   s.indexOf("x")
来源：http://hz.hnqzz.top/gtgezogyso.html

Java: s.indexOf("x")
来源：http://hz.jiagoushi.top/gtnzcerkpb.html

Go:   strings.Index(s, "x")
来源：http://hz.0kj1m.cn/gtzzhbhbhy.html

Ruby: s.index("x")
来源：http://hz.jqgfzy.top/gtwowbfcci.html

C#:   s.IndexOf("x")
来源：http://hz.vqdsnc.cn/gtksxaxdns.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.tian-w.cn/gtwoerljvs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jinqigufen.top/gtiduoucea.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xinyue.icu/gtwdwautfg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cqqwz.cn/gtgvzqovbm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxinkj.top/gtvwohpwmg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gaohongyu789.top/gtrleijrdk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shanyushiyangtech.top/gtcbewcwzt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yj20258888.top/gtxewobctt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.nanxinkj.top/gtbaafnfwu.html

[E06] 替换子串
来源：http://hz.zdqjudy.top/gtxlsbcclv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jqgufenzy.top/gtwpcvbtqq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.aibaodan.cn/gtiatyytqh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtwzhvnwjc.html

TS:   s.replaceAll("a", "b")
来源：http://hz.aizwys.cn/gtfiirhutt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gtcdaubpot.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.redwolf501.top/gtqvtchoun.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.fzhhl.top/gtfmrtyyjn.html

C#:   s.Replace("a", "b")
来源：http://hz.yj20258888.top/gtujrzhafc.html

[E07] 按分隔符拆分
来源：http://hz.chenlongwang.top/gtlciblfiu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jyoumei.cn/gtqeigzhot.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.bjfxy.top/gtoblwwpxe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.chenlongwang.top/gtxmwduozq.html

TS:   s.split(",")
来源：http://hz.dashuyun.cn/gtdcuvdrox.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hysaishi.cn/gtnxxqcmcy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.iojbl.cn/gtvsfmrozh.html

Ruby: s.split(",");  s.split
来源：http://hz.cucudq.cn/gtqhghqxpi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yvedp.cn/gtqngqpjvx.html

[E08] 数组按分隔符合并
来源：http://hz.bjfxy.top/gtwdmmztks.html

Py:   ",".join(items)
来源：http://hz.jiagoushi.top/gtvfhnoyza.html

PHP:  implode(",", $items);
来源：http://hz.yuxming.cn/gtrueboxah.html

JS:   items.join(",")
来源：http://hz.dashuyun.cn/gtevhtudib.html

TS:   items.join(",")
来源：http://hz.feifeiyinyue.top/gtpfvgwxbc.html

Java: String.join(",", items)
来源：http://hz.cheryme.top/gtslzgkbkh.html

Go:   strings.Join(items, ",")
来源：http://hz.yongpay.top/gtjlsszczi.html

Ruby: items.join(",")
来源：http://hz.yongpay.top/gtepoptzsb.html

C#:   string.Join(",", items)
来源：http://hz.jqgfzy.top/gthpthidqi.html

[E09] 去除所有空白字符
来源：http://hz.snrcjt.cn/gtqtypzpit.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.daria6918.cn/gtfknjdrzx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hysaishi.cn/gtomgbeyvz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gotoacloud.top/gtvgpxddld.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hysaishi.cn/gtntsqaitb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hnxiangtu.top/gtyeqwnlqi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sweek.top/gtrxgwubea.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenlongwang.top/gtiozmsqcv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhaomingkeji.xyz/gtudoadgew.html

[E10] 左侧补零 / 定长填充
来源：http://hz.haohaochexian.top/gtnhpjdeeb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.wangshuangyany.cn/gtqiomxzes.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.9152youxi.cn/gtwlaqwyhb.html

JS:   "7".padStart(3, "0")
来源：http://hz.pengpengdd.cyou/gthhdkhvap.html

TS:   "7".padStart(3, "0")
来源：http://hz.yvedp.cn/gtkzjwnvwj.html

Java: String.format("%03d", 7)
来源：http://hz.sweek.top/gtgokrwuft.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.fzhhl.top/gtzpnvhqfv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yuanzhike.top/gtpwqhdqpk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhoulong.xyz/gtzmdovgve.html

[E11] 反转字符串
来源：http://hz.fzhhl.top/gtrhbdnqgy.html

Py:   s[::-1]
来源：http://hz.yangfankeji.com/gtrmldinnd.html

PHP:  strrev($s);
来源：http://hz.yj202588.top/gtinkmwifq.html

JS:   [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtfvpqkbpm.html

TS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtlwjaaspd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.daxiang520.top/gtlylgulcg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.fzhhl.top/gtlefbruzk.html

Ruby: s.reverse
来源：http://hz.kuanghao11.cn/gtdlesoudl.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xingfuxueyuan.xyz/gtusmdwmyw.html

[E12] 统计某字符出现次数
来源：http://hz.xingfuxueyuan.xyz/gtfyiergus.html

Py:   s.count("a")
来源：http://hz.cdnleiting.top/gtklzgkczi.html

PHP:  substr_count($s, "a");
来源：http://hz.yanxiufei.cn/gtkmbcqxpi.html

JS:   s.split("a").length - 1
来源：http://hz.yueranfly.top/gtmljwnqjd.html

TS:   s.split("a").length - 1
来源：http://hz.ybcxt.top/gtudakyazu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hnqzz.top/gtnlilkcii.html

Go:   strings.Count(s, "a")
来源：http://hz.smart0.xyz/gtwlqrvzzk.html

Ruby: s.count("a")
来源：http://hz.dashuyun.cn/gtckxdqefs.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tian-w.cn/gthdmddxns.html

[E13] 逐字符遍历
来源：http://hz.xuetiantiany.cn/gtqlluobto.html

Py:   for ch in s: print(ch)
来源：http://hz.chenlongwang.top/gthkohhash.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xziqi.cn/gtjdapqrnn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gtqinufhum.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jyoumei.cn/gtinfaeyoa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.c1oappe.top/gtijwbzcmq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.kuanghao11.cn/gtmoqzbtjh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cheryme.top/gtvjljtuzd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhengqikj.top/gtdgghwpvl.html

[E14] URL 编码与 Base64
来源：http://hz.shanyushiyangkeji.top/gtjdoxhhte.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xuanzx.com/gtaonwvuvr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.andypj.xyz/gtxhvuahes.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gogol.net.cn/gtbdcsodaa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.daria6918.cn/gtzpodayow.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shangyingyoupin.top/gtiwjkrsxm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.birdmap.top/gtkfpwbtqc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gaohongyu789.top/gtqfswvrrm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shuidangran.top/gtytvebebu.html

[E15] HTML 转义 / 反转义
来源：http://hz.redwolf501.top/gteoqoeoob.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xinyue.icu/gtqiigbaqp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ppjwa.cn/gtmtjieddv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj20258.top/gtwdbvvgbx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shanyushiyangkeji.top/gtmxlqfigc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhongyouzk.top/gtghictofh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenjidiqi.icu/gtlwrvbhuk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ybcxt.top/gtgleybfeg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aizwys.cn/gtqgcavrhe.html

[E16] 数字千分位
来源：http://hz.quarkkingdee.top/gtrsmmwfid.html

Py:   f"{1234567:,}"
来源：http://hz.zhaomingkeji.xyz/gtilivjvqv.html

PHP:  number_format(1234567);
来源：http://hz.iojbl.cn/gtydointzi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.feifeiyinyue.top/gtcqgxgtgk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258.top/gtxdsjzcqn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yueranfly.top/gtmeophfzv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhoulong.xyz/gtoubmyzmq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.wangshuangyany.cn/gtewszsoew.html

C#:   1234567.ToString("N0")
来源：http://hz.c1oappe.top/gtijqhwdxr.html

[E17] 首字母大写
来源：http://hz.mhx1999.top/gtrvylsjjh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sweek.top/gtdkhqkbuc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zdqjudy.top/gtwixegfwz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtffdbpeon.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cdnleiting.top/gtxemecdlo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hongshengwenyu.top/gtbftufmwh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yonumen.top/gtfwfxsdrr.html

Ruby: s.capitalize
来源：http://hz.bjfxy.top/gtlizbkdnj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gotoacloud.top/gtxjwafqhn.html

[E18] 模板占位符替换
来源：http://hz.snrcjt.cn/gtjohdoazr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yanxiufei.cn/gtuaatqmrv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jlsjyb.cn/gtazlwhior.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.redwolf501.top/gtlswnpmhy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shzxlz.cn/gtkmdbuurb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.52xcode.cn/gtocxbfqop.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gotoacloud.top/gtjujwasyz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yuanzhike.top/gtuohqdkca.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.dashuyun.cn/gtjjcsfyvd.html

[E19] 多行文本按行拆分
来源：http://hz.tianlin.xyz/gtnjkztkax.html

Py:   s.splitlines()
来源：http://hz.zhijiandao.cn/gteklyrlht.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sufxvd.cn/gtqszgaolj.html

JS:   s.split(/\r?\n/)
来源：http://hz.zdqjudy.top/gttjtmzbtl.html

TS:   s.split(/\r?\n/)
来源：http://hz.gzhubu.top/gtwbvfihob.html

Java: s.lines().toList()
来源：http://hz.chenlongwang.top/gteszhayge.html

Go:   strings.Split(s, "\n")
来源：http://hz.meibo888.top/gtppsaykck.html

Ruby: s.lines
来源：http://hz.quarkkingdee.top/gtkirlrqlx.html

C#:   s.Split('\n')
来源：http://hz.yj202588.top/gtcmeadgpg.html

[E20] 判断字符串是否为空
来源：http://hz.xinyue.icu/gtpmfklryk.html

Py:   if not s:
来源：http://hz.bjfxy.top/gtmkswruyw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhaomingkeji.xyz/gtblskqtqs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yueranfly.top/gttldwdzki.html

TS:   if (s === "") {}
来源：http://hz.yanxiufei.cn/gtziylwadk.html

Java: if (s.isEmpty()) {}
来源：http://hz.bjfxy.top/gtbnrmrqdg.html

Go:   if s == "" {}
来源：http://hz.gogol.net.cn/gtzybegoyj.html

Ruby: if s.empty?
来源：http://hz.gaohongyu789.top/gtljovoood.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sweek.top/gthnrjdpte.html

[E21] 超长截断加省略号
来源：http://hz.jinqigufen.top/gtsjtojzop.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhiwuduotai.top/gtzmzrpplu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jqgfzy.top/gtdekectrz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtuxzupfzb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gtiqtvuzfy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtlqveauze.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ydzc1.top/gtlknwfutt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.aibaodan.cn/gthigtkxvh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.9152youxi.cn/gtshymksbr.html

[E22] 字节长度与字符长度
来源：http://hz.xuetiantiany.cn/gttvakunbc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shanyushiyangkeji.top/gtetctepav.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tianlin.xyz/gteqyxezjw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtibxbyqkc.html


<!-- 参考信息 -->