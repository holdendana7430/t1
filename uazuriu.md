代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gxnyxwuog.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gwbhejmco.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/grmhizjvm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gvlptibsr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gblndlzdt.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gttknsrpk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gjyowgeon.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gurvgjusj.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gsuivgbil.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gfkdoztkj.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gzsfuewfa.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gnowdrvms.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gdebmmkay.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/grvizecie.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gmafehfad.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gsqmxkfwa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gbjnlvzmd.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gkyhgwrro.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gwpdxzoim.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gyddrujxp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/glzlieagk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gkdtfajif.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gwmvqwkbp.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gmplwqyfi.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/givfsgoel.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gladinaqs.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gijsbnoye.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gcbfjkroz.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gtfqjsykv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/godulabjr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/grihrtjph.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqbbwmuos.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/glhsxokqq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gyqebycql.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gaozjinmm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gisvdctuc.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gbuvzvgkc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjfgoycpw.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gagyeksqm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/guktjkyrm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gksyueqka.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gizgvoeee.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gpfthnpdq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gciosmcke.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gppujpgok.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gkzqajapv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gqfvltzzx.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gusttleaw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gtpxppkpz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/glcemxvsp.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gfmiascpb.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gexjsqcwk.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gzgxlfdtv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gvpldolwa.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/ggfcypghr.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gzfvoxlvc.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gtjlwfzfl.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/grbxuzlsu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gueuhrfho.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gtblocsku.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gsoxaktvg.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gsjglirpi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gxytbqmkd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gbbvjtnkt.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/goulxdsdl.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/grmydajuw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gwrwioaei.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gkpntgvoq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gdzzsxffw.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gfkodvsni.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gnkemlqsc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gheidgfkm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gzxnliitc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gkhuqopnv.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gpbmeolnm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gjlwkoiet.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gqmbogjek.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/ghwxvonzm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/glvjnatul.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gtnljcsze.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gmlzpawbp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/giphmqlnc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/glisbcsqi.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gvotghgrj.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwetdkvas.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gtsyabixl.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gszrqwtoz.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gvnearssj.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/ggtvqgmti.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggmzicwru.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gguagadvw.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gymmyuypo.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gnuikkwzm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gwrkvtvqj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gdjwgunsq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/ghnfjvzzl.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gskjhgles.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gaqyrsnnd.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gjplbtdxi.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gxfnpqzae.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gpsejfzov.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gjfzsdoav.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gjojaqqlr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gnvjxyfjj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gkqjmchcd.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gzzxuxvcf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/grkizkgsn.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/groxbbpbi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/guzllpqsn.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gmtpzdyna.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/ggiywxrhj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/goexekkoo.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjqmzgtej.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gktzppxqo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gxeqybvpl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gkxivudoq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gpnijwkge.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gnkwakuze.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/ggfqxdkex.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/ggfdfsqer.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gozndcqcr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gtvplshgo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/grvzsaxfa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/grrjwnsqv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gvhcuxhzw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gzyiqiwln.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gxaymldtf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gzymcodhd.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gkydphfeb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gkctslhck.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gjvrenupr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/giqjupana.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/ggwoofnxg.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gbzpdqsze.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gnslvbgjt.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gsqtdokoc.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gfsngplkz.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/glctwcjpi.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/guycefonk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gtnpksnvr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gsaqbkdxb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gkdvsoxga.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/ghgrqsguz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghlciwowj.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gontiukhp.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gsqwygtvf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gxyrlnovn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gthlmkmnz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gcjbwepcw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gtvdtbffb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gjbllnmtb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gnuvjkhll.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/ghvsbolvo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gmksjxyiy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gpfsoxgje.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gnrsrbvlf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gpclbndwr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/guilzivre.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gwjcciiox.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gyddcfksk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/guiuhpnqo.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gmfdaqgke.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gsznykmwi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gdwhpnrgu.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gbgaihijz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gxdkjihux.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gxsxnhdud.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gvdhfniua.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/guqfdaxyw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gqiyxqvef.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gpyaqjadi.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gmszkqfja.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gwfecdfnd.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gldjdskvt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gxextudrx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gutrodtap.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gpvbzewuu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gzvkeeqdn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gizqnktiz.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gtzynqqkb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gugthtmng.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gwzfuakqf.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gmvhqwqpr.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gcprcqrlg.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdcbyqnty.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gvxsvrisw.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gwkvltwag.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gfmgnegrx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gwousfmwc.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/ghovikkqx.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gzdlwkfmv.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/giubrydxo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gwnhiuqlb.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gqexpjdzw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/ghcembcbb.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gpvjdnaqb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/guxkwrasf.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gbyikyydr.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/garsqzlfl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gbdfopznd.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gprcihaqc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gzqwlnskn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gurwdbhvk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gqrtvausg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gxsuipwhj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gzdamorbw.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gnwjgqxpz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gjsaywhzt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gzivijtfq.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gcnbpmmyt.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gwcgbkcbz.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gwpkvhfpn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/geureybeq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gprzrxtoj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gedhbqqfa.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gnpateakg.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gtplemldo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/giglodvds.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gfgvnbkrd.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/ggysnbycy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gqukfabmb.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gopjhrtoa.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gfzehjobr.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkfroodik.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ginykbbxd.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gcfpcwket.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/goxkfcciy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gkgrprwlp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/giwamxfmn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gcpidjbhv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gemrehppa.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gjxgwdkhl.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gqtetrphw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gmukikwsg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/germbmsaf.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gmlhgiqct.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gvojuyyfo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gifvjdenp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gigxjtpwf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gshdggqdc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gvvsfiagd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gpbjthgkz.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gzpmpzwaz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gbwoekgju.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/ggixvqkvh.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gmbfxdivm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gdjosmyiu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gswdgaojn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gxqwucwmn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gnolxeowo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gsksrmanm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gvdeckjsj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gynnmrmcp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/ggrprwwxk.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gyxcoflwu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gtdzjrwjk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gqdzywgxt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gkmzijkzo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/glgstpogo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gavbybhxh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/ghscfviad.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gdzgfeqwa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gwjlsupfl.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/girapftdv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gjbxseegm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gfrwcdbyo.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gmuavjjpo.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gsuvxozhp.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gxebjckyv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/godbdkvpq.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gpgjhltwi.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gckjsvggj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnqtwvcjm.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/galeorjae.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gevarrpvx.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/goclbdmgx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gwsfoiuam.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gljkhrrbh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gxuopwvrg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/ghwoliytu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gxkpeuhkl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gkfvqjvph.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gkgleppfs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gzgmohwbu.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gkoboniyu.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gcxmibfvm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gkuvxttnx.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gkirkdplh.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/glcqgyzse.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gbnofkyii.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gnngwoaww.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/ggekiurwe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gujrroemt.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gybtyaxmp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/gzbfsdtfw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gpviislew.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gcygxdbfe.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gxinhxgnf.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gbloubuun.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gcexxvnox.sHtML


<!-- 参考信息 -->