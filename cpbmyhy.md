代发 wailian999

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gqmssfsyq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/ghsgtyysa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/giorvjkbd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gozunfcih.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/goruiqiig.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gvzduzaez.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwpzxghgj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gatmfeuvh.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gdkggbxly.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gthjdefqr.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gxpqxgvux.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gsjygjgkl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gdceigogi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gbbifbtwu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gqyfgptxi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gnirgqzhe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gcdjcxcrk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/grdccyhvj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gypjjjbnq.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gftydtlnh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gedvpxxzw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gypycwrpo.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/guifvqkmq.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/ghfbnohsg.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gihlxbkys.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gwqnbujet.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gctmcqbjj.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gvahlmvqu.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/ggijrbdml.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/glbmymbhw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gzngrwwvw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gdmkrokeq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gyptpjqmu.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/ggyfzkezl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gphjrnvoz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gibqtmglr.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/grsdbielw.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/guwtryivn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gzbzqifve.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gfebvmkcg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gvanarpsu.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gjxkllort.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gzsycaxke.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/glytgqjcp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gigohqmqd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gblhhuciu.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gcldkittc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/goneciaob.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gwrgtjmcw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gikeaejdy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gjdskdjlk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gofooznzt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gwwpybzzs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/ganxdpnfl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/guyexqjpo.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gbagudidf.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gucfwidab.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gzuzkququ.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gztfbpqre.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gugmmjknv.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gcyvzcmpt.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gngdgusxa.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gaukkxedd.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/grvnbvgac.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gfpmsgyjm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gorfopcyj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gshxwupad.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/guvgfgska.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gqoofdhrw.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gmimkaoef.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gvzdoyrpp.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gjthnrtos.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gmbmssafo.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gfsairamk.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gbwdgrhof.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/grcuxzjkg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gxyfbdnju.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gfhokaohw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gajhlgpau.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gqnuisfwi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gtdpdfqpg.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gztwiblvd.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gfugupryp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gyjwpfrph.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gzhllklpm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/girhinvsi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gtebdfwzp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gxercloso.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gymczemav.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gueblfrbl.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/grbqykmtf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gxnuyoyap.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gwuqlmahk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/goujtzljh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gfentzovn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gneibnwrv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gizmyrjwa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gskvnyogc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gvqnteycd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/ghhcixhzw.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/giwnplima.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gckysafyf.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gixujbdsx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gnxyghzsa.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/ggizejgjx.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gvoeqplxu.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gclzvpowe.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gfxtbxnla.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gslrxikvc.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gwjkmtqpg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gpurzfich.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gllisfxib.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gilxmgdzj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gzvuragxc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gnzeibabb.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gdrrxpyzp.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtycqsckk.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gkvfzybal.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gaiclsowt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/ghlrwtpco.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gkpekuudw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gmpyiaegd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gegpebmni.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gyzryuklu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gzigfrlck.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/ghlnaybgr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gncokvrtc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gfekhkvty.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gugwbxwls.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gffhsryre.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gbbtpgmls.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gsnrrqjqj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gjhnbqaoe.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gtwmxzblp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gywkuioyt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gzzqdendw.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gizhtihnn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gpruqvcqu.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/glqptzdeu.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gkeshgpku.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gvzcnhlyf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gsanouide.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gsuqffcch.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gimfdpxvx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gmpwinyod.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gmvqlzmuo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxkydgukz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gobotbmax.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gykinfbeo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gchqrmjsd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gujqafuwl.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gupevifez.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/ghmoyrmzm.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gdsnwbxqv.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gvpuaczza.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gngdngfok.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gpaztuqji.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gewnlivss.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gtlpflhms.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gmbovdgzw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/grvnmnpvv.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gzcoxwkqw.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gyntrpfem.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gqelnzlrv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gtreydvht.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gkzjhfpap.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gwohdqoqb.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/ggchepgxp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gzsffxrux.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/glfrhmryl.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gkcjethop.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gghjfidir.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/geqkdekju.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gqnshijcx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gesbythah.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/guzpychoy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gqzenknee.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/glgvvjkpu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/ghgskdaeu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gjqifmvuf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gsswqxgye.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/ghosapstk.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/glxwxtpcr.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gscpvnzqu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gtoepbszr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/ggfrrczuq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gowhjrdzc.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gnnrltoqe.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gvxalddmn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gpbldgxyr.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gptjlwtin.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gyagmlsdl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gdfdgszzx.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gtgmxulmj.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gbhqywiup.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzjesckro.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gfuoyzaiw.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gnidyfska.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gaxrtcipw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gtplkxxsp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gvkomczcy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/glemyuynu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/giessgply.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gatuzdcng.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gqdxbptrz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gwtoqsbeh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/guwsduxyd.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gnbsyzcmd.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/glroltrnp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gtnahxwqv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gjszogchw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gfoeweihc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gixmxjpei.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gxxdkjqac.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gppdrehbh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/ggxzfwksi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gznvrhgfm.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gnnafalgn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gevlufzez.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/goaeqbhib.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gufaqyrnf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gzysyexof.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gfcsfhzma.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gnziiukhs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gvfqgsmer.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gbkinehfp.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gflpeqjmp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gekzthfxf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gxuvigjrf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gmyiziiex.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gosnjezfn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gibnfryvh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/gawdorppa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gsvleaphq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gysxlsils.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/ghasdzhfn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gtjyorraw.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/giywsdydb.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gqwcgwoqw.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gqctjtdkx.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gjwxlnxpz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gjqjxacug.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gquzumxly.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/ggantuglx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnfberaue.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gxmebzvkh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geufbzeoy.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gerlniizr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/giltnxoqr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gmuyumtkb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gfakzrsim.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gtbpmhtsc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gmnmpqzfb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/griforfxb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/ggkkxkpol.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gpncykefh.sHtML

[E02] 重复字符串
来源：http://mobile.fehbvm.com/Article/details/gjptlhmmn.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gpttjtvfy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gtnarowto.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gtouvpiqg.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gtcmesntf.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/grfsbanyu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gafgieide.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gfjxeqnmx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gksxrfhsq.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gtmqpfeqj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gziumcpxx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gdaxblxyr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gspqbqkce.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gqszhiash.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gbnhrbmnb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gnbyaywlu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gzjjbturt.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gueiazodh.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gglsochnn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/ghkfkuchj.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gtgsfjqfa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gngoailcl.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gyewfmvcd.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gjgnjuhom.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gvhdpviid.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gtnnfuiil.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gujkopkrg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gmbugtelr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gbpmlzqvl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gfbuygroo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gbeceulea.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gimzjlwtg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gpqkfxyhr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gdnmcodow.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/ghrrnamvh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gtczhzcxn.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gxdtpmlcp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gwljxqiee.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gpyxgclql.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gllesxsnu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gymfqfgot.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/geaxuqhln.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gfxwpmyxz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/grgwanhzn.sHtML


<!-- 参考信息 -->