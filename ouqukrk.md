代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gxtxltgzm.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gzqxhipwd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gsqswwxye.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gyglojlrz.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gpnuxxotp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gmzlvvads.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gemgmfsxe.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gpavwahzm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gsubtrgmp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gkiiggrtb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gtscxoshr.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gtjgjjrlg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gegkufoig.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gnqwnorie.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gratlbacp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gmxshovkt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/ggdxyjglf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glrtmzdgj.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gmtnzrkrw.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gxmgbttrc.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gjzaoghbq.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gchatseem.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/girpolnld.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/grqdpcjyt.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/ginzosnnk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gaekrwcgw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/guwzgoiyz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gvomvsdgp.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/ghhlvvfsf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gzeeucfkk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfuchsjby.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gljhauori.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gywdqbdey.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggremrhsb.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/ggopwmrvv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gnnbudbrx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/glgsaoqro.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gbpzkssxm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gjyxlufml.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/glspampph.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gvjzbdhts.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gucwqrctq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gxqbfvxir.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gowzyewlo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gtmdsrfqy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gaubttyra.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gnbdljqkr.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gsponngeq.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gkqolcais.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/ggaxgkcbl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gcpqhbegc.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/geititqeu.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/grqvayimu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjwhkyjcd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gtjmqrkos.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gekbutwpm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gsgoxllgn.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gfpzcuujr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/geuxfatye.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/geyxwbsyr.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/glvzrxjqr.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gebyvogoc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/giqrykzys.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glwqtimcu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gvtklhyal.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/ggcupytum.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gjnsknnlw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gicangvqi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/ggliczdsd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gifghynmc.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/ggxfinitf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gruyqcogg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gxockoiak.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gfhwhfgqx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/geqwrcyti.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/ghiompkqo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gytbmaiuu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/glxsscqwc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/ghsonorie.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gbbxcjjzn.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gksjhnaiw.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gfjuxdppv.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/guvuegxzs.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gnstlovgt.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gniyzwmyu.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/ghuwhpseo.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gpagcxrdm.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gbcicukhu.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gvlmbipyk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gbydllqtj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gzjsyxnoo.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gfsyaqgif.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gurwgfpfs.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gvurtsmnu.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gwjjnhfko.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gejrbubcl.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gxcwllytb.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gwkscstqo.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gpjhoeshl.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gngdbbpgu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gjeheqvpe.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gwpwkgdrn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gpfrxbtes.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gkpbimdsu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gjrjilwpo.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/goinfeevc.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/glogykwda.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/girujxanm.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwpfoisbm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gaqxazwhj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gaefwnrlf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gnsugprui.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfbkwkjxv.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gepykqrlq.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gkmzepywk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gbdyhkjsw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gglxwantz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/glonmtovx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/ggnyvydqj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gdmipicsp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gjwhkhjuh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gkrqrwxys.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gessubbqv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gcmrcnuyj.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gocozeruo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/ggmsgerwq.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gbyxsapjn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/ghyfflcbw.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gnvopmuku.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gphvzzlnb.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gocspfbcd.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gpnnubmyu.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gflzyeerc.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/grncweqjc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gexrdexth.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gpzybuoeo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gjthzlvqi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gmdxdcrtf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gpysbcyjt.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gdjofrtvp.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gmqlyngqu.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gfmyqfjja.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/glmowabqu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gzgdpeknx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/glahkwmfh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gvbslobdg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gvhuomnai.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gpcxqievn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gwnancyrl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gtaxnkgwu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/grixsvcag.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gunymzmxr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gemuosbqo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsbymqpcq.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gknczmnaw.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gtblrusxv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/girsfvvdk.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gjefjxobk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gknkuwbwf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gnhtrwwla.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gscysknnt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gtzsreucx.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/golzevirw.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gbuttzbhm.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/ggdrwzbeg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/goizolxtc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/ghzlodznf.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gxkbhcqak.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/ghpblrojz.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gwnuuicap.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggdqzmwid.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gdcauitdz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gfznompmp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gekehmoru.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gwrnjiazd.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gqvkmqfev.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gaorbqrwo.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/guxrcfdtq.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gghpbkkqp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gjvjftrsr.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggymoikpw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gzswmntsr.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gpetsvket.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gdzcmdjzh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gyxnzejey.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gnngnydix.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gepzklutn.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gwyhpzyqq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gmbigcaxw.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gekwpndbc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/goxdfxipd.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gjnearkdq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gepsxuzdv.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/goejiulgm.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gbcgniscc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gfxjydncm.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gbmdhplst.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gmmhgmcau.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/ghleslces.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gvtenvjku.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/genkrlhfv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gngulghkq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gskhvulvz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gpzxuaorq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gyeltzlqn.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gkpwlsekk.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gqqixikdl.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gtoniuytu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/goynjover.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gtnpyvycf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gpfcusfjp.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gtliqsitp.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gpoonggsx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gxfisjglc.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gxloizoqv.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/goonvjzbq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gzgkluibj.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gwdmsmyjm.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/grsfxewdl.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gzqbvnbzp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gpodcrxkl.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gqijpnrid.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gldvspzrh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gfmxynxff.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gdrmcdmcn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/grhxnrqsv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gggnjafjl.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gwhltwdfo.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gehhdmaln.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gityzznif.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gsbjroxwj.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/grmrkcdkg.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/ggubdwlme.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gajljeplb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gpjbrklfu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gjjoedasj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gfhymgzrp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/geymqfyff.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gzgrsmqru.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gftmubbxz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gtogntisp.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gllxagfak.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gpmcdrlaf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gghejorvf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gpryrqbtu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gftipdeeo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gaxdrpujw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gmknqibto.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gsgsethbu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gxpeopjsu.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gtbqnzsts.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gskvjstlu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/ghhiczoqw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gesnayvpr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/ggpwnvjmj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gmcwrkzdu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gaqvxjttg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gdyzaqpcr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gfqoteryw.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbqshvehf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gympjpuus.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gftrdayiw.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/ghzggfhxj.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gcingytay.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gohhzhcsl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gnxhbpetl.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/glqqwjyte.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gowbckwya.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gepnzwjnb.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gxhchitos.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghwoubsiq.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gzuhnunmn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gjfhkaexl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gqrhamixx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/govtvxmvz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gulocttgz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/ggscoofsv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gdnehjjfr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gdpnchxfo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gaeimcnik.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gotvspurr.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gvzoogbzv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gdpdiaznu.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gpesufegf.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gcynpdsis.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/ghgbspygv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gyehrhsun.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gjwzirclq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/grxmucejx.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/glgrfglcu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gsjegoiiu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/ghwqlzyhs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gfoydkkgz.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gyyaafuej.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gnxrnhcnl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gcsanxlvv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gnpkfcbnj.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gnbplhaix.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gxvrpntsy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/glclzoizk.sHtML


<!-- 参考信息 -->