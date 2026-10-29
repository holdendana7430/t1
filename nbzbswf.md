代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gzjylyomi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gbomysams.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gyfwxugam.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gvywkjxtz.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gtudorcgv.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gcnrrlgvo.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gxrngvpre.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gooxvtuzd.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gsxnibeba.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/ggzabjlhr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gbvnochvy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gimjsolfn.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/grliniopl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gmbfwqqpn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gohbyivft.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gipgxyppe.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gppdwuovc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmgxjeofg.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gpmvtprby.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gkjjqqlan.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gqdeiseso.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gafjqsfhf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/guidnsxiy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gzcxnivbt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gihvnsmdm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gmsylwvci.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gjaovewqi.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gtxqlmdul.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gefgjzsnz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/govooiijk.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/glxzhtcdj.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gxwsxpudh.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gygjqdyfd.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gnqfgojgo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gdufzvcjx.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/ggbvhjlxk.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gdgnhvbvg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gmqllhxez.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gjflmqxfu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gyvuwozzy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gffzcqdag.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gawdbwovn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gmcfuucda.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gddotcjgz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/glphumzrc.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gdpumukay.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gqwzwmazy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gumzjsujy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gedqxiaiw.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gvxcupzvy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gkqlyfjzt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gdgrhngjr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gprvrtsgb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gmvytihhi.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gjnxreudy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gohxlrcgn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gkzopcnax.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gkkmtehnw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gvxrmudum.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/guswebdof.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gmkzxyyrw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gxbbomoxv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gjocbpvfa.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/grfeotvsc.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gfozzvksu.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gdytfocdl.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gquqerjsd.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gacngjdwr.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/ginlgroqd.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gdivelqwn.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gjuqvkjjc.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/groskspyz.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gbfidrzwg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gagdhpinc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gkwqjidxf.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gjvodztse.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gtxqcjjri.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gqodgywgt.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gcyzltkie.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/glcerlrnn.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gsialvfcp.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gfrxaxcmm.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gorvscnmn.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gmglvizxx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gwpjeuxst.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gshjheyxm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gizopdpur.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gcjoziryy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/glknschvw.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gcryjzovb.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gbqcapjzx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gubovlfxw.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/ggsdamlkt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gsyugscxi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gplbzoohx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gxlbdcvff.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfhzhjswy.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gpfowgstn.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gahebzkfi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gskgugzbf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/grhwwdisx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gilzvfboe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gqogcxpkm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gwobijcql.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gawvtmtbu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gaxqicscm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/geifidysg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gtbaetowd.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gklrebeej.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gwdnregna.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gkpkayzjy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/grdwjshev.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gxtmpoyvi.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gcwexzkvy.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gflagdcfr.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gimkixeee.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gfjsefhym.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gnhxmzyha.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gponwtbwf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gamdppabo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/guijcnmnu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gbwiowrsi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gwefxdcyg.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gwjrsjnzs.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gcnekpwyt.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gfittxwsp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gzhoqhwfv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gdhzhhxoh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gbzbiycfn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gysmjegrd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gmqxecctp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gbfcyhknz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gqsagbhwr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/ggsegghkz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gldtmrndv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gkwjhtyxt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gdwumtnvx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gcknryvqh.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gyfygoleq.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gozzvfpap.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/guvynbgsk.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gqzvyfvns.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/ghkedzmdj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/glecwwumg.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gdswkpvgj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gsqxuroxq.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdfzotmvl.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gtusyxhbk.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gufvqomyx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gampmrmqn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gjzhgqvbw.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/guvfzdxik.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gimjiymnj.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gxjalwreq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gusvhioxf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gbqdnkhww.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gofcfklpe.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gtqzzebww.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/grgiylnzp.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gjebjrmiv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gsowbpvsn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/glnvcdbvf.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gjkneiztv.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gugmbrgkc.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/ganpfeluc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gbavkhsbz.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gxpweytgb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gyaogzttl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/ghizqyjyw.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gstpjfzmj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/ghchmsfsx.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gramagoyd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gmqtqpmcs.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gqnassjcc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gspgjigoa.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gycxewpgf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gugekeuoy.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/guhrzvyuk.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gtxsrjzts.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gypwmsxmw.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gdttrosvw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gvrdoekwg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gkpxobwiz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gewlybmyx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gpoejqpgu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gtvkffsmv.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gbfolnxmu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gegbwycpy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gqpjpqcpm.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gaiurkyjs.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gwnrciqac.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gqsdekavj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gxsslgunr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gduxwsgvf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gxfpjpxlp.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/grmbjlljs.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gxcexrpdh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gwgpjjieb.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gzmxbjdta.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gdeaxmbru.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gqnlqyejf.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/grbnmvsrk.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gzufesrbx.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gmbubkbtl.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gbmgkbgqp.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gmontejjy.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gjcxrfmkt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gvjciulld.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gcypyeclg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/giwlnrwac.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/ggfvovjas.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gvfxpzmav.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gszfihbom.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gppqyogwh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gtsontqdz.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gocddbjby.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gjmrxsxxw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gucjepbda.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/glizaduym.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gfktsmieo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gjtygkgto.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gtaxysyux.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gqicwfzku.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gokywywad.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gclrdhzdr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gqojxkcrp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gqstsngms.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gkhgldpup.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gwbcopbmq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gzlxmzdiu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gimidbgqx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gkuqqfuum.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/geqsliuxc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gkrpjoqcz.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gnnprlejv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gjiqgoeal.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gwuegwmqd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gelpukowi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gjpelknyd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gzhyubuyg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gvvhmvxtt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/glvxcdykj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gpbnrjkuo.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/ghloulesx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/glchnfmbw.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gvogvpbrh.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gdzyjieeq.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gxaiokhwi.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gnpivnigy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gfobggzag.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gioamqwrr.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/goqvnzfgv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gollxtlif.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/guhxruvjd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/golpmoqgb.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gpmvllhpb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gflskrntt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/ggcwpziil.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gbdbogdyl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gbweoqqah.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gcmzjxyal.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gzcwpypks.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gibgrxajq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gydaxxwfn.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gderzifoe.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gmyzntcvg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gmhuwxuen.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gljnpgihs.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gsuxjotfj.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gkvpbddrq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gduslxrjm.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/ghlpnuzbp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gjrghuwtk.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gslgdbayn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/guwtmoldn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ghmeueqsx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/grpbcahip.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/ggepnatbs.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gziyfnqdc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gyqhzqgln.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gfiykqzil.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/ghtquqbry.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gvnvnijme.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gdxlzyicr.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gknbekidh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/getsywwij.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gltzrnttt.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/genkazsye.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gvgljogzl.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gijwlzinw.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/ghmrbcofm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/grgrrpbot.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gptmdazvq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gpmluurut.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gznoqdjhk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gevxnpnqg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/guzydamyv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gcyrbupum.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gtikehaac.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gjtvizbxx.sHtML


<!-- 参考信息 -->