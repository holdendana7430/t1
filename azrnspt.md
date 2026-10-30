代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gdmnjuuur.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gqeejarol.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gihoqtccb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gvusfhapf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gycflrhjk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gdtyptagv.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gwpwnauwo.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gddajtaks.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gscxgpkjw.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gehzezvfd.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gypfsmeza.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gkmnnaxow.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gaqvjtvay.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gmqhruklr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gxljirtny.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gzcfnkhlc.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gkjylprrq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gcdiydjli.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gdxyxuvbr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gadzmchgc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gmotpowft.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giduvelbs.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/geonnbnau.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gybpvvxik.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gaznwmodl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gafdjbmjs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/geazxsale.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gxoahjeki.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gsoaqtvct.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gngggkbkk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gzomzyfws.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gkhzyuhro.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gsltmcpeq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gprvexntw.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gdhbunfzb.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gccsdywap.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gvohajajg.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/ghblvfysq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/ghpsddeym.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gindyuuhi.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gsdxewctu.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gswtqyywp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gjpeoodfs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gnujukoju.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gqwgqzeza.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gpvxyycyo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/glqhissfx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gyozslezn.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gjsedbuzn.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gmkddnofv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gqfvfojey.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gmiucfkay.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gfksklvkw.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gpipwbzzg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gxwsqfgtt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gewzobmib.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gwdpyiilu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gbdwdtjxj.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gvxzoqdbo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gzivylwmn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/garkrnqvp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gvlnqofuj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gmjawhbwa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gkbrnnyfz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gjahknnur.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gipdqqxib.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gmltrlsba.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gottloakh.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gflisghdv.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gwhbygzet.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gohqhsoqx.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gfdfklqnz.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gokjcejhy.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gtzighujq.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gvgafguwi.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gktvqabyv.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/geyzqstlg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/ghlilgkhu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gqsfvyvfo.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gmclkdidv.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gzfjscldz.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/ghmcnbnnh.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gzeegtlvn.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gxhicuzfr.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gtzzsvrwv.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gzsnriwrx.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gzlzbdoef.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gtiiamuwf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gtvykyloz.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gvelqpopn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gkqkfdryq.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/grybnhwqd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gipcpvfjq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gkpqqtyzs.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/grdruxszn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gmisivtli.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gkborecpf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/geaypgbms.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gpbpzlyws.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gbvogcwkn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxxdsonjf.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gavdjkppa.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gvqtwmwhe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gkqlgjrqi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gwogddpgw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gipltxrtb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gortcjtel.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gilwaaanq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gcoijaduy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gihzdicex.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gmscaifrd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gjbvqahqx.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gikfsbyhp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gbnpmzesh.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gjgjrgctp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/goqerogzk.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gtplvsuin.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gzxyldujb.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gpgdnryjg.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/glerkfzyb.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gtoghjszw.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/ghqglbxee.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gzpdqgreu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gtzfcsnnk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/ghgilfpuf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gqvcxozhx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/guxgoeeon.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gqlmtjcvs.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gojcftypb.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gdqbojhra.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gklbiktwe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gmdwdvbpn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gfdlwezzh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gedmqwdgw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gplpfrtce.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gyzbdanjf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gufmzncjb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gyrrgxsov.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gtupmwtks.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/glinpxzev.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gjcsmenou.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggiafdtes.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gdeggzdoj.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gevmmshte.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gmvwzzoyb.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gsrtcnmfw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/goqhdedpm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gbzaavrgl.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gnvdcxkmq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gwbjhmmct.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gicrqvxdv.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gjrkgeapj.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/ggqdybotg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gzowbcngs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gbvusdytu.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gkovmoyxv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbrqhtosa.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gcooajnwi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gjskaivnl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gmdizlwkv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gbaydsgcn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gqlmwkpea.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/ghoupwlif.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gkpohhacu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gkcvryvtk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/garrzwltu.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gklaeitii.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gjzdbujqn.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gsonjrort.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/grrwogbdo.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/giebhvrmy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gthyvqkxm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gragsnhpz.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gbeamsylo.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gljyqdvuf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gkwxlmcmh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gjyxfbkwl.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/ghtnlzeap.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gajknobah.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/ghpfgqmsu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gkzyzwajo.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gzolwzlnv.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gnygtubwy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gghrijygi.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/ggehjuqpb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gszrnxebs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gupxbnini.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gvgfxaqxz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gkdhrxkke.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/giyptfwlu.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gvefndysp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gzyrklwit.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gbhxrhfjz.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gynrcbfhc.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/grinqyxkl.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gbcqaxwnw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gxknzhupr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gwtthmzcx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gbexqlecp.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gvcuhglwt.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gjfcmbldj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gcwbalhyf.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gvyjrywnr.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gjhkigdfi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gxuubdldq.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gmbjardfp.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gdzkurlsz.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gdxwctgea.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gxobulvsn.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/goksgcbmq.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gzctzbqlp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gehwglsec.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/grpqyiwyu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gpylhonms.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwpgunruh.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/ghvbiqiub.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gpgsnuswn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gffzklmzu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gcosokbrq.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gjiwuaglv.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gjeytiqwq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/grdqsujpn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gbosctxrj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gwwnwodkm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gemdrapsa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gqeuohpon.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/guwzntqcx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gwgnzhinu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gvbcvmewo.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gbcgsscob.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gbaofljbj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gzuatigjy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gvujfhezg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gjecmhpni.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/grfpanoxb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gvyfflysw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gwtvcuxeu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gpxtjboee.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gboxekfgf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/grxpsdvrh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gdalpvepj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gllfwufjh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/giyfyabhj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gggcfdism.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gwsbxvvsj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gbfnlizbr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gtdlfjphu.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gwzumpvsb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gnkhkluyp.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gacmahfjk.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/glfasqbqo.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gbtajeubi.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/goiwjnanq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gibivsogy.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gdlseedgw.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gvtuoyzmk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaxqkuysw.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gyqeaobji.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/geuomlara.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gxblvmbqq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gucdtkige.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gxhyhmvgc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/grqwbtrfo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gtvmekvdp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gtqhgrcvo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gufkyzcqb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gkwgfvpbo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/guqlremel.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gizmwfyrl.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gzdontpjn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gtqpiyqls.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gcrkmngjl.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/ghheoxnlz.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gzpjsqict.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gwyycjudg.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gzunfjhsx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gaiegrqsy.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gawmhyfrb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gynibxxwl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gbvogyxch.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gqxkgenek.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/guexffiqy.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/grzxgmpwu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/glukykusc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gcfqsmwdq.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gbyvvlygg.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gmjxinikb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gglmzwavt.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gjuwdgimd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gnhlnmjfr.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gkxyxmngs.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gccmxsjdq.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/ggffgqbed.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/grgbkrfnf.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gekjeuyxw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/giwrsjfri.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gfbmyjoyt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gggkdarqi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gdeaxlzwl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gzxhymstd.sHtML


<!-- 参考信息 -->