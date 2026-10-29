代发 wailian999

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwtbhlhzq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/ginomdpxn.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gnyxrdsvc.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gtlymhexc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gzgbmmfma.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gbzogcohz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gbncbebld.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gqnrfwppf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gzfcnwomc.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gmpfgrcvi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gytoxjnfg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/geffiivsi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gorzjdsdy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gwdzuiatw.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gqmqzgmge.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/grtgtazqo.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gxxhxkvwo.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gzmammzqp.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/goarpcbdy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gwyjsdnfi.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gvcnsxpmz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gmdlatduu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/ghsnhwbzm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gugqyfdcl.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gmguicbts.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gvqrmslah.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/glwxdxkog.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gydrvcisg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/glszaeivo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvpztbmdc.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gmmdvbuvn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gphdmftsw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/guwbwinoh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gnldvvjgz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gwoytbgcp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gsybbgmee.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gnuxmwlpq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gukiogksw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gnjyaknlw.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gonptmepi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/ggrohjpbc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gbhrackom.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gfybycgfi.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gsccrvpsc.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gkgnhnmlr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/grytdbxzl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gorfkzqkh.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/geodlohbc.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gzouflrpa.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/givcakobz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gzlncxhfl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gtarmykvb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gemtyjrti.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gqogoiact.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gtvyjpapi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gqwzzozdw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gxscgwzvl.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gynrgegtp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/ggfrntlhj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/geijimlna.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gngjihvem.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/ghlmtfauo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/goxccwnjs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gwpygpose.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnttdhzyx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gdyteohxx.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gwehxnxil.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gjfgqdmej.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gkjrflpom.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gvfhjcjyc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/guzvtvgjn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gcnsdbuxk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gxuohrxxd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gpdkbeanh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/ghzmukdjd.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gmmyyooyf.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gfsdssrtg.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggrylzseb.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/geofkmgqq.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gzgyrdhpa.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gmqayzkvy.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gkpbqsqhf.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gomhelrmz.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gadewmxsm.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gxdmboosk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gylicvnmy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/geogqpmks.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gqbdivyzb.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/glrvsirrl.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gybhfuugh.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gzuyjboxi.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/goffxjxwi.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gfocknqxo.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gfdqwngqy.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gbsbqrpda.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/glabvggjc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/ggsywvjrb.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gctjozvay.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gcwiomqoe.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gsyquhhjd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gudsjtywr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gynzwnfhz.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gjbuoaqht.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gtiumqjsa.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gzafxzfbt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gzkvlstqs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gvatlqbqs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gryobkvci.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gsmzszlvc.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gghmdmmqu.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gtyxrjrze.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gfmmkkaai.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/ghcdalbnb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gawzxgjoo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gbaciworg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gvmozkgdt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gervbyymd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gaxoawmvz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gkklclfpu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gggbpzxzv.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gbulciycd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/ggtsysogv.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmeadtqun.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gnilhztyv.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gcspejnch.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gbqhsqhxp.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gdmmxtirm.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gdtnrumsh.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gbbopggoe.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gcvntvhbt.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gdxcjdrhi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gsppsiqso.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gwjtpbfuq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gyoybvyyb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gyabevxrh.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gninhzfxc.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/ggccvmpuf.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gwznzjxqh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gtwnhvwzs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gvptjsfho.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gpakumlca.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gpgapakwr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/ghgnkdmrv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gbroqyxxk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gheyhgkry.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gzjczizit.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/ghpwwzawv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gflxvynad.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/glpemytpg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gntmsfaxg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gxmdvfwiw.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gnlvzkgnu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gpvtxwsgv.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gjlglsiuj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gaphbhsme.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/grwblbsuj.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gfwnewane.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gfwtollye.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gfjpwcykc.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gthjvfdck.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gsmrtxglb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gklvqkjzt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/ghdniwsoi.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gmjcfiaet.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/glhlcsvfc.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gnttqgedx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gplhorhus.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gkeinopui.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gvjfpgvzn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/glbtxvtmb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/ghvgbylvx.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gvsowqbef.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/grdxaysxz.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gtxptcnbu.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gwdqukabz.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gjyxovpcl.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gjgkymcme.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gizvkguom.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gljsobohe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/glxvpjpvb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzctpumiz.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gakfgpyog.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/guvntbkla.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gfyqthsip.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gokoujbdy.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/guegnmbqv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gcibrjshu.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gmgxlpnhb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gvohbolbv.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gpwvrulov.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gxrknxzhq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gpeikptgs.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/ghrqdnsgw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gduyfhlyh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gilcmvwgm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/ggpnsubtf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gepgslgpy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/giycycaii.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gtwpfmzlw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gszgvwrlo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gjaqkfmef.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/ggrxqueva.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gkbajomfx.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gemvddhcq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gatkcslve.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gictvuvie.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gdwrlvfis.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gzluuhpwu.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gzvyknacf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gktitbpfq.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gkxemyirr.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gptxheegw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gzazjrwus.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/ggptolsmt.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gdrjizinf.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtgyczfrg.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gcegusevs.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvyiubzd.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gggcawkze.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gstmpokhb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gljxwghvv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gsswchthk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gqfgsvpxc.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gzbjkqhkc.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gbeylzjhz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gmmpeirfl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gttwikslw.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gcibbmqsi.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gclmhjivj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gqxclsqxs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gmtvuajcz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gfdggpadp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gsihewmza.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gwizwvmee.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/ggmveuwlz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gbptajgsq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gmoelckkx.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gzdrlwivo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gaxgmvkep.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gxsbzvvtg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gjgndafmq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/grlwprhpc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gmedqmytf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gnnocndlz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gxeqjxolm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gjalbwdvs.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gjezghhzl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/ggimtbbpi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/ggyciihit.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gcwvloznx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/giebeodyk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gimywdwbp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/grfplbivt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gvtcsjukh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gxjtqdhnz.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gsqvqjsia.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gikqxntfg.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gwxqtxbyb.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gnmvzazgh.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gzdopxvto.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gxagxykkz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gucovahlp.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gwhexkfil.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gqbbxxexc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmoebooaj.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/godhfacoy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmqxgegda.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/ghhvhsxkv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gxwduleoe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gibphpsbx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gxxxqlker.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gebuepxdr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gdcaxolqo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gyvoojhze.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gmfxpxwyc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gpkpwudcy.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gwydudsgy.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gxoslfrmm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gndsykbjy.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gdrgncgmd.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gvuwvpnfx.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gqcrgnxoz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gdvcfrger.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/grpfioghw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/grggagimg.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/grjkbfbec.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gqsncfkmu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/glrhtggzl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gndsvmqjs.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gxvkzjfzu.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gldzfrvju.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gmtxkorzh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gdpdpnryf.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gubffbefb.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gthkkhtjr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gfeksgqeh.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gysbcflni.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gynmyumsm.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gutdacktp.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gwuymecsb.sHtML


<!-- 参考信息 -->