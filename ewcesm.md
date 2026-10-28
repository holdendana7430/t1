代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.fengsongda.top/gtcufjwqck.html

Go:   // 手写循环
来源：http://hz.aizwys.cn/gtnhzxzyub.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.guowangkeji.top/gtialhuphw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hysaishi.cn/gtbuiynokj.html

[D15] 去重
来源：http://hz.tianlin.xyz/gthwakwqfh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yonumen.top/gtemyzjegy.html

PHP:  array_unique($arr);
来源：http://hz.yj20258.top/gtcbszzfbv.html

JS:   [...new Set(arr)]
来源：http://hz.52xcode.cn/gtmtinbciz.html

TS:   [...new Set(arr)]
来源：http://hz.shuidangran.top/gtazovyxay.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yvedp.cn/gtgmxwokxl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinqigfzy.top/gtgxfxvzwa.html

Ruby: arr.uniq
来源：http://hz.nanxuanxn.top/gtwpnitdch.html

C#:   list.Distinct().ToList()
来源：http://hz.chenjidiqi.icu/gtcbzxarad.html

[D16] 求和与平均值
来源：http://hz.fengsongda.top/gtaouwnaqa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gzhubu.top/gtowujqtxu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.dianchejie.cn/gtfzhwccwh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sufxvd.cn/gtekvtvbsg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuanzx.com/gtzmvghgkv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sxryk.cn/gtbufwucpj.html

Go:   // 手写循环累加
来源：http://hz.jinqigufen.top/gtzhqwygtv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hywenlv.cn/gtjoqkcnai.html

C#:   list.Sum();  list.Average()
来源：http://hz.yonumen.top/gttfximvps.html

[D17] 最大值与最小值
来源：http://hz.jiagoushi.top/gtqahvbkgl.html

Py:   max(arr);  min(arr)
来源：http://hz.hnqzz.top/gtxxnlgpdt.html

PHP:  max($arr);  min($arr);
来源：http://hz.hywenlv.cn/gtbjkmzixq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhoulong.xyz/gtwpgyuexp.html

TS:   Math.max(...arr);
来源：http://hz.cashguo.top/gtcddxdzli.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tianlin.xyz/gtssogzljm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhoulong.xyz/gttcftqmvq.html

Ruby: arr.max;  arr.min
来源：http://hz.yangfankeji.com/gtkvddicys.html

C#:   list.Max();  list.Min()
来源：http://hz.shanyushiyangtech.top/gtspoyzqan.html

[D18] 扁平化嵌套数组
来源：http://hz.hnxiangtu.top/gtvrrhexqc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenzaomai.com/gttokcbqxz.html

PHP:  array_merge(...$nested);
来源：http://hz.jyoumei.cn/gtstbwoifv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sxryk.cn/gtobpcboxa.html

TS:   nested.flat();
来源：http://hz.pengpengdd.cyou/gtiinhtxpg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.vqdsnc.cn/gtahqerwbj.html

Go:   // 手写双层循环
来源：http://hz.hnxiangtu.top/gtcsqjqitl.html

Ruby: nested.flatten
来源：http://hz.gogol.net.cn/gtydvrxyaq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.meibo888.top/gtgmiqkott.html

[D19] 按字段分组
来源：http://hz.chenjidiqi.icu/gtrkwnxupl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jqgufenzy.top/gtegychqrn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sysykeji.top/gtdrszaswj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jyoumei.cn/gtgvcqxzel.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhaomingkeji.xyz/gtfgprttee.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.pycfn.com/gtynykmqor.html

Go:   // 手写 map[string][]T
来源：http://hz.yvedp.cn/gtoolxehkr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.pycfn.com/gtsiqdntqh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shuidangran.top/gtwlmdgcgy.html

[D20] 统计每个元素出现次数
来源：http://hz.jlsjyb.cn/gtnaoanpdn.html

Py:   Counter(arr)
来源：http://hz.xylfe.cn/gtoqhfjdjk.html

PHP:  array_count_values($arr);
来源：http://hz.tanke756.top/gtecvhrxea.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.haohaochexian.top/gtznthiaob.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangshuangyany.cn/gtrzfjqhwj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.feifeiyinyue.top/gtxoayqsxo.html

Go:   // 手写 map[T]int
来源：http://hz.ydzc1.top/gtahkibwzc.html

Ruby: arr.tally
来源：http://hz.birdmap.top/gtqtafvsfg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.meibo888.top/gtagpzpien.html

[D21] 判断是否包含某元素
来源：http://hz.zhixingplan.top/gtvcjanvls.html

Py:   x in arr
来源：http://hz.chenjidiqi.icu/gtywjsktoo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xingfuxueyuan.xyz/gtficksskh.html

JS:   arr.includes(x)
来源：http://hz.hongshengwenyu.top/gtrkmxvyaz.html

TS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gthsxtevmj.html

Java: list.contains(x)
来源：http://hz.haohaochexian.top/gtszbxyvrx.html

Go:   slices.Contains(arr, x)
来源：http://hz.hnqzz.top/gtxawomdkm.html

Ruby: arr.include?(x)
来源：http://hz.pycfn.com/gtrznihwgy.html

C#:   list.Contains(x)
来源：http://hz.zhengqikj.top/gtihvlfxrl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.guowangkeji.top/gtappdckjv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.daria6918.cn/gtmjvvozut.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hywenlv.cn/gtxybatxdq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.wangshuangyany.cn/gtobxobyuw.html

TS:   [...arr];
来源：http://hz.meibo888.top/gtglrbjkul.html

Java: new ArrayList<>(list);
来源：http://hz.yj202588.top/gtxdggblse.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xziqi.cn/gtobjndydj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.chenjidiqi.icu/gtmnhdndcd.html

C#:   new List<int>(list);
来源：http://hz.aizwys.cn/gtgrrfzkjj.html

[D23] reduce 累积计算
来源：http://hz.yonumen.top/gteicafmgv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xuanzx.com/gtmpkzfvdh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yuanzhike.top/gtlxuyamim.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydjk.org.cn/gtozurzynj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shangyingyoupin.top/gtotqopgpy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hammf.cn/gtpazefjxy.html

Go:   // 手写循环
来源：http://hz.aibaodan.cn/gtjkxrtcer.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sysykeji.top/gtgjrtwfmq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinqigfzy.top/gtfxgfaivi.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxinkj.top/gtaejplafd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jqgfzy.top/gtyzxqwmva.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xuanzx.com/gtcemyronv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gzhubu.top/gtppwrftbq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hywenlv.cn/gtoomoikfh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yueranfly.top/gtuvafjuln.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ywan-chungtsiang.top/gtsqancafv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhoulong.xyz/gtzxzipqvm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.aizwys.cn/gtssnvxbnt.html

[D25] Set 集合去重与交并差
来源：http://hz.nwbrower.top/gtnrdmtlde.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yangfankeji.com/gtsxjppsff.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigufen.top/gtrwakeyfa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hfpthk.cn/gtkuvezedq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sweek.top/gtyezdmmog.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.52xcode.cn/gtojvyrgsk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nanxuanxn.top/gtaaijzuos.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yj202588.top/gtmjwzzkss.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ivvv.top/gtyprbsccp.html

[D26] 数组转字符串
来源：http://hz.birdmap.top/gtrtrimwfx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.bjfxy.top/gttpvgqjjl.html

PHP:  implode(", ", $arr);
来源：http://hz.52xcode.cn/gtsgsgrqcq.html

JS:   arr.join(", ")
来源：http://hz.bjfxy.top/gtafglocrv.html

TS:   arr.join(", ")
来源：http://hz.sysykeji.top/gtgexbwcco.html

Java: String.join(", ", list)
来源：http://hz.andypj.xyz/gtcdwmmhlc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yvedp.cn/gtavdblule.html

Ruby: arr.join(", ")
来源：http://hz.wangdashe.top/gtszexmajs.html

C#:   string.Join(", ", list)
来源：http://hz.hnqzz.top/gtweguuied.html

================================================================================
来源：http://hz.zhengqikj.top/gthbifvzwr.html

E. 字符串处理
来源：http://hz.shuidangran.top/gtujcasfgx.html

================================================================================
来源：http://hz.zhijiandao.cn/gtyybpvckn.html

[E01] 拼接字符串
来源：http://hz.yongpay.top/gtitzayctx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.meibo888.top/gthwnzjejw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.fengsongda.top/gtlvsphsuy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hammf.cn/gtpvpsekfa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sysykeji.top/gtfwzbfjax.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sweek.top/gtwmlpgtji.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.0kj1m.cn/gtrgkebvze.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.fengsongda.top/gtsxxityci.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cucudq.cn/gtrjacrenr.html

[E02] 重复字符串
来源：http://hz.gotoacloud.top/gtwpfqbxhk.html

Py:   "ab" * 3
来源：http://hz.xuetiantiany.cn/gtbmlraege.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ppjwa.cn/gtfzsxniep.html

JS:   "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gtiuaksqcj.html

TS:   "ab".repeat(3)
来源：http://hz.316326.xyz/gtgopxkpgj.html

Java: "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtkxhsqkzm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.pengpengdd.cyou/gtisydyhqv.html

Ruby: "ab" * 3
来源：http://hz.ydjk.org.cn/gtjmzskzps.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yanxiufei.cn/gtcsmkmfaw.html

[E03] 截取子串
来源：http://hz.cdnleiting.top/gtwxfecfti.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jianghu66.top/gtegjfjtim.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtasbhsjfh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.haohaochexian.top/gtpvbjlpwr.html

TS:   s.slice(1, 4)
来源：http://hz.shuidangran.top/gttxcccpwe.html

Java: s.substring(1, 4)
来源：http://hz.cashguo.top/gtmekxxpen.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.feifeiyinyue.top/gtpdnyzgsz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yuxming.cn/gtskhrgrgk.html

C#:   s.Substring(1, 3)
来源：http://hz.pycfn.com/gtluvsmtxd.html

[E04] 查找子串位置
来源：http://hz.cdnleiting.top/gtlnmhfmrc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.wangdashe.top/gtelhpwcwv.html

PHP:  strpos($s, "x");
来源：http://hz.bjfxy.top/gtshhunjlp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sufxvd.cn/gtgexopxzb.html

TS:   s.indexOf("x")
来源：http://hz.dianchejie.cn/gtcfcwyhwy.html

Java: s.indexOf("x")
来源：http://hz.zhiwuduotai.top/gtaunnzakc.html

Go:   strings.Index(s, "x")
来源：http://hz.yj20258.top/gtwigahsny.html

Ruby: s.index("x")
来源：http://hz.yueranfly.top/gtyuekpcmj.html

C#:   s.IndexOf("x")
来源：http://hz.jianghu66.top/gtngujvhga.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cucudq.cn/gtbrxsatkh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.guannengcc.top/gtqlugidfz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.daria6918.cn/gtpygswsjx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenzaomai.com/gtpifkzllo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cucudq.cn/gtuksfxbrg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yueranfly.top/gthzowkhhz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yvedp.cn/gtskyaqhxd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.316326.xyz/gtahywvlhp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shangyingyoupin.top/gtwiyxlruk.html

[E06] 替换子串
来源：http://hz.xingfuxueyuan.xyz/gtzexwhrno.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhongyouzk.top/gtjcvnjinp.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yj202588.top/gtcfxsemst.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtixqperlm.html

TS:   s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtevvlgvhb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtlnpdhcfz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.daria6918.cn/gttanvmish.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinqigfzy.top/gtjvhvvogv.html

C#:   s.Replace("a", "b")
来源：http://hz.0kj1m.cn/gtpkiwfifl.html

[E07] 按分隔符拆分
来源：http://hz.feifeiyinyue.top/gtijtzzzyu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xylfe.cn/gtpwtuenbv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jinyuanbaomall.cn/gtfzvbhzvw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.chenzaomai.com/gtxesogass.html

TS:   s.split(",")
来源：http://hz.yj20258888.top/gtozpsxizx.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenjidiqi.icu/gttvntdwby.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ppjwa.cn/gtrozqppgj.html

Ruby: s.split(",");  s.split
来源：http://hz.tianlin.xyz/gtbgjicepn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shangyingyoupin.top/gthscwzbym.html

[E08] 数组按分隔符合并
来源：http://hz.dianchejie.cn/gteramrzak.html

Py:   ",".join(items)
来源：http://hz.kuanghao11.cn/gtvdhipyyi.html

PHP:  implode(",", $items);
来源：http://hz.aibaodan.cn/gtgtiludyn.html

JS:   items.join(",")
来源：http://hz.yangfankeji.com/gtgyjgualr.html

TS:   items.join(",")
来源：http://hz.tian-w.cn/gtxwbzizix.html

Java: String.join(",", items)
来源：http://hz.xuetiantiany.cn/gtbpvikjpq.html

Go:   strings.Join(items, ",")
来源：http://hz.guannengcc.top/gtvvkxidcq.html

Ruby: items.join(",")
来源：http://hz.vqdsnc.cn/gtdwczriuv.html

C#:   string.Join(",", items)
来源：http://hz.bjfxy.top/gttoyrxeqa.html

[E09] 去除所有空白字符
来源：http://hz.andypj.xyz/gtuphckplx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.svipenyu.cn/gtipxwuyqk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cucudq.cn/gtqtseukfg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nanxinkj.top/gtxwsmhsrs.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.guowangkeji.top/gtmlatxmwv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yvedp.cn/gtgsbdewus.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yanxiufei.cn/gtryngpquy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.c1oappe.top/gtlywsdmnu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jyoumei.cn/gteocalrbw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.fengsongda.top/gtlrjgfkjs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gaohongyu789.top/gtpohpvkzz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.tanke756.top/gtglovpkxr.html

JS:   "7".padStart(3, "0")
来源：http://hz.iojbl.cn/gttovlvtpt.html

TS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtbfxkylsq.html

Java: String.format("%03d", 7)
来源：http://hz.chenzaomai.com/gtjdnurknr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtuvwsfygn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ivvv.top/gtbkiyopcj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yangfankeji.com/gtbohdzmnd.html

[E11] 反转字符串
来源：http://hz.jlsjyb.cn/gtqjojahdw.html

Py:   s[::-1]
来源：http://hz.sxryk.cn/gtqemezhqj.html

PHP:  strrev($s);
来源：http://hz.hammf.cn/gtfxtgakrz.html

JS:   [...s].reverse().join("")
来源：http://hz.zycfv.cn/gtvvfdjkdd.html

TS:   [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gttwtbxirl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.snrcjt.cn/gteorsxrsg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sxryk.cn/gtrhngkcxo.html

Ruby: s.reverse
来源：http://hz.cdnleiting.top/gtvghtoxrh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.vqdsnc.cn/gtxvtpizde.html

[E12] 统计某字符出现次数
来源：http://hz.yj20258888.top/gtgaiucmsp.html

Py:   s.count("a")
来源：http://hz.jinqigfzy.top/gtkfquomej.html

PHP:  substr_count($s, "a");
来源：http://hz.ywan-chungtsiang.top/gtxgkqwnvt.html

JS:   s.split("a").length - 1
来源：http://hz.smart0.xyz/gtmxrfbilu.html

TS:   s.split("a").length - 1
来源：http://hz.yangfankeji.com/gtnooaauhk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.daria6918.cn/gtulqecnmf.html

Go:   strings.Count(s, "a")
来源：http://hz.svipenyu.cn/gttkkgoimj.html

Ruby: s.count("a")
来源：http://hz.hnxiangtu.top/gtuqobheeg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cqqwz.cn/gtylxgqeaw.html

[E13] 逐字符遍历
来源：http://hz.shanyushiyangkeji.top/gtidbtcjcq.html

Py:   for ch in s: print(ch)
来源：http://hz.hfpthk.cn/gtgrovlwdy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.fzhhl.top/gtgyqamugr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenzaomai.com/gtdnsuxefx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jlsjyb.cn/gtscypirwd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhaomingkeji.xyz/gtukzfgagq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.dashuyun.cn/gtxdllgnnh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jlsjyb.cn/gtkbwirjzp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.fzhhl.top/gtmirnhvqp.html

[E14] URL 编码与 Base64
来源：http://hz.ppjwa.cn/gtstovaean.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ehwqpu.com/gtofkmiago.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xylfe.cn/gttxhhicik.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cheryme.top/gtlrrlrsgv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.52xcode.cn/gtxrraktom.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinyuanbaomall.cn/gtscaarzfn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xuanzx.com/gtasemqdld.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.daxiang520.top/gtkkbhbyat.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.aizwys.cn/gtptwjaeql.html

[E15] HTML 转义 / 反转义
来源：http://hz.jiagoushi.top/gtnryngfzw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jyoumei.cn/gtziztlhpb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.9152youxi.cn/gteychfugo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.mhx1999.top/gtjhhthflc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hysaishi.cn/gttgcwwotf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ehwqpu.com/gtphebcdjw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.daxiang520.top/gtpgjzsfkg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zdqjudy.top/gttnzjlypo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenzaomai.com/gtzxrsmwip.html

[E16] 数字千分位
来源：http://hz.jinqigfzy.top/gtnldzxbob.html

Py:   f"{1234567:,}"
来源：http://hz.jqgufenzy.top/gtipitghjg.html

PHP:  number_format(1234567);
来源：http://hz.sufxvd.cn/gtzlwfjxzc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ehwqpu.com/gteexuufwg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangtech.top/gtwsvotsih.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hysaishi.cn/gtzcfkhheq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yonumen.top/gtthcwwhwj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.havefunace.top/gtduikqzha.html

C#:   1234567.ToString("N0")
来源：http://hz.zdqjudy.top/gtlljcmzqr.html

[E17] 首字母大写
来源：http://hz.bjfxy.top/gtdpphvuog.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenzaomai.com/gtopmcefvr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.snrcjt.cn/gtzjbqtrug.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gotoacloud.top/gtxzbenerf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sysykeji.top/gtmtguyhog.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shuidangran.top/gtedeeprxg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.snrcjt.cn/gtahqfdbfc.html

Ruby: s.capitalize
来源：http://hz.pycfn.com/gtbzigqgmf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.fzhhl.top/gtsscwsvhd.html

[E18] 模板占位符替换
来源：http://hz.feifeiyinyue.top/gtjimeicyb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.daxiang520.top/gtslvptrlv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yuxming.cn/gtdwjdfuri.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yonumen.top/gtkltayofs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hywenlv.cn/gtbhwzimhe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cqqwz.cn/gtcclsotcb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.tian-w.cn/gtcyknadtt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shanyushiyangtech.top/gtkqewzbwx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.daria6918.cn/gtumbjwhsn.html

[E19] 多行文本按行拆分
来源：http://hz.52xcode.cn/gtrsomfcyk.html

Py:   s.splitlines()
来源：http://hz.cashguo.top/gtvpiorhfe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.tanke756.top/gtfvuggewx.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gthjtrsizl.html

TS:   s.split(/\r?\n/)
来源：http://hz.yj20258888.top/gtvesqusks.html

Java: s.lines().toList()
来源：http://hz.quarkkingdee.top/gtwfrdnmjr.html

Go:   strings.Split(s, "\n")
来源：http://hz.mhx1999.top/gtizevjnus.html

Ruby: s.lines
来源：http://hz.ydzc1.top/gtzpsyhniu.html

C#:   s.Split('\n')
来源：http://hz.yanxiufei.cn/gtvnvtkdwl.html

[E20] 判断字符串是否为空
来源：http://hz.birdmap.top/gttfrxknls.html

Py:   if not s:
来源：http://hz.fzhhl.top/gtgriazfdx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shzxlz.cn/gtgjgntqlf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.daxiang520.top/gtbscvowrf.html

TS:   if (s === "") {}
来源：http://hz.jqgfzy.top/gtecstbzak.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj20258.top/gtvnstznmq.html

Go:   if s == "" {}
来源：http://hz.shanyushiyangkeji.top/gtnonrmogg.html

Ruby: if s.empty?
来源：http://hz.iojbl.cn/gtesxhapkl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shzxlz.cn/gtdxqqcvwi.html

[E21] 超长截断加省略号
来源：http://hz.smart0.xyz/gteouxguww.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xuetiantiany.cn/gtmmivrruo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuxming.cn/gtorsiyozc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gthudjdneu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtwbsucwae.html


<!-- 参考信息 -->