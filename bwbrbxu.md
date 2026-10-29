代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gduvhosra.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/geaqtmbsi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gkwaubyjo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/ginedjdyv.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gpfpzeezc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/glkqjurvf.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/grdupdozx.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/ggsftktto.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gwqcavkvo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/goqxosojn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gducygrjg.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gjemtgzod.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gizvmnght.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gjvyulnat.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gqlhplvdd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gzekxtfvk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gpnpgjkfc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gwmjqhygm.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gziuxvyps.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gxzbrswke.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gooxmpyxz.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gwjvyurpt.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gunpluvhv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gqqviabbm.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gjbfwxjvf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gtylslxtw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gtifbqqfg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gdgqmmksv.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/grzypbhcr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gpxbenlpm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gaiqvbjft.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goojogwqc.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gwvlqjlpq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcugelpoz.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gaxsvpxzd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gatzoctyh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gkunwwnqb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/glmyjuyav.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gsjosxrqy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/goitrokqs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gzbdyouix.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gxefcmhmm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gqboymwnx.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gccivwtij.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gwgbolryq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/goeyotkkb.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gkcyuzvra.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/geiljwjui.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/ginrunyvj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/ghbjmypoq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gwujvqpry.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gsllzccjp.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gkottsqgy.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gkgeewqsq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gyveacslx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gdwxqzphb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gdodxmxmw.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gfjkqyzsk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/ghzsswuev.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gnkczmysm.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gnatdoaec.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/goikrkdjk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gjvachmvh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gbyamimty.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gszuumbld.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gytbookzj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/givmysucx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gvvxduyvv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gzwxbelsi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/ghlylxnxe.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gdudnohgg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gtofrjbyq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gpuekouhp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gairkwbpc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gsutsvqly.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gavkhjzax.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gplbzityu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gytzxbolu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gvrilystm.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gmmubrhjz.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gkfzjrnyx.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gsawkdsit.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/ggadalrbe.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gyacabifw.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gcytpmavx.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gwnzhjtrz.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gimiqqxno.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gixxylyyr.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gfhcjhgsm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gjztrhlye.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gopjfslsq.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/grajbolxa.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gjwrhyylp.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gkuzasilz.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gqaymzlwx.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gvsiyzmfr.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gqorafbho.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gdlujczhg.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/ggqcgujsx.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gyjwysjxe.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/guxqbeyes.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gokufofxc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gobfwludq.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gnmgflsmb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gfakbawet.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/goztqrjrl.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gwtixkylm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gwoulcdnm.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gdrvnooju.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gfjzvifto.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gnhwsqmba.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/ggppqdpnv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gmruvmvbu.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/ghdpwvwnx.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gmtdbzfjy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gjlsascfi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gqkoqkixa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gdwjtaoei.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gatppcntj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gnuwariuu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gpyfyfwhp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gpqcwkqra.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gomkzijrs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gghmitnts.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gbpwvzany.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gcpuzuxdz.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gnlomfmty.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gczovlvav.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gqsssruak.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/glbovvfkz.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gdpobeeub.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gueuvhtlp.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gsraadhln.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gtngaegwa.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gncizqkvq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gabrrtdft.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gdxvmfkqq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gthfgwadk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gfapyloqo.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gbsgxlczg.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gnluvsoct.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gjmeixlul.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gqpbjufxz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gfsrlorqs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/ghqeylvik.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ggnqoerqq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gqohckwcd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/ganbsqyrr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gxpnehipf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gpaijnkqu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/grdqsfypr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gflmddjre.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/grzidjliv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmjayeznc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwrmbagha.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gzfdokvhs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/guorndqzj.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gdkevddtm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/ghftpeerp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gdamjgzyu.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gixbqoiyf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/guxogxnkz.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gluzbxgiy.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gwnrlewtu.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gunfnldxu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gndiidrza.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gfgtolkai.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gjxqhwmrq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gbkygwyrq.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gtbyggswm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gmpfmqibg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwiupcbzd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gtyvedood.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gcstvludx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/ggvsiqwog.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/glyderhfg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gjpnqywhe.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gpqnymfwc.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gbflnnytd.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gzbaaegqh.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gfikklhif.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gfsrgyugz.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gaifgxerx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/ghjvlwvih.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/guaycrdvh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gnqclktoo.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gedbppwnd.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gaeowddme.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gsjajvlkx.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gjsnxgvhl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gjmqcaoua.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gawqpxemo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gijmmufwo.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gcvacyxzy.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/giyspxqqa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gbakoqygq.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gjjpzevbx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gyoaecwnw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gcykdmgqs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/ghrqfmkib.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gutihkicw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gxwspkabo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gwnzhxcjs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gcgdmvfyh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gzfwgvkao.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/glugdsjaz.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gqvygends.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gtaoymoqp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gupngzgbr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gxpuyiapi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gnuuutobn.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gkovasknx.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gyshiniwt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gpzbkjcwv.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gwgsvvxzp.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gpewaqqlb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gimumbmoh.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/guoybihxa.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gmoxpkboq.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/guimrftgi.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gzqhxcaox.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/grqjtvnbq.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/ggvtodvdp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/govccresd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/ghwmyyixy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gkwinprrm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gplmonczl.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gimwytruo.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gatzoqwok.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gqdbxvnde.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gjmycsfcd.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gnpkecfks.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gwhibqobd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gwbrihgas.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/goaqltzcn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gznzjytrh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/glzrcwqum.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gfyhrfwvt.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/giqvqmfhu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gzwtxjvri.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gnyprdwwn.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gofxipnmf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gmghprvrf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gddzpenhf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gzaobmzjh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gjatrjxwl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gvtnltyrm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gbmidfemx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gqxswxztt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gngkdhnjm.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gypqrcefq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/glbbdzpxy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/ggbghqylo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/givwpowqa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/ggkumxxsr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gusqiaihd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gryfqjlir.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gmxnnypuh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gfwzhxagj.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gjqnyjmxa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gkmcjmyxk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzrmohqnd.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gyzzonjoh.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gcnrxsode.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gexkgymht.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gmolcwtkq.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gqebheque.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gjxjsgmmy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guwfpsvuj.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/ghkxvlbdf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwgbxnkok.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gbvnuuoni.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/grrrekung.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gmqapjrjt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gaafxdqkf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gomxhgtae.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gdcngkwad.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gyzurkevn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gsnvaelll.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/graxgxlvw.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gzpkiashf.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gzvqongbv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/getyimvfr.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/ggiwxissz.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjysikai.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/ghznfkecv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/guohecaph.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gylxirpza.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gtxoxagvj.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/glsiaxixc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/ghhvschra.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gcbotvzjl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gebcivxua.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gmesoipab.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gsaelweer.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gwwjlfvom.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gruzadnnf.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gnogszwdn.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gzmtgzviw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gfjkimiqo.sHtML


<!-- 参考信息 -->