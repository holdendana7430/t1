代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqtdvzqs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvgnjwve.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fanxiaobao.xyz/Article/details/gixporjuf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/groykugyh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfpziclus.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fanxiaobao.xyz/Article/details/gusqqvlhg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fanxiaobao.xyz/Article/details/gpiwnmuya.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fanxiaobao.xyz/Article/details/gxzpsliky.sHtML

[C14] 泛型函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdmmcgpc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyttuqqhc.sHtML

PHP:  // 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gilmkefxq.sHtML

JS:   // 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvohlegz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcchxeytf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghnsocqtl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fanxiaobao.xyz/Article/details/gfxgfmsvl.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunjftgyk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fanxiaobao.xyz/Article/details/gviwwdgwz.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfbczltz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvekgmif.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhhwhqjp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gmudqkdjn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzuwgoztn.sHtML

Java: // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/goqdnjjqw.sHtML

Go:   // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gupqwogem.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggujlnsgc.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fanxiaobao.xyz/Article/details/gedmzneqe.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fanxiaobao.xyz/Article/details/gxohtggen.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcogghlq.sHtML

PHP:  // 无重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gwshvekro.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjuxujla.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fanxiaobao.xyz/Article/details/glyhlwysw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxtjjluz.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fanxiaobao.xyz/Article/details/gctuxraef.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjelpzfxe.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqkvxjck.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjulvdlcn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplfufkjs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhvhamgt.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrznfmtg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fanxiaobao.xyz/Article/details/gszjforoy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gxryvowaz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgekarwf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrxqoxmz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fanxiaobao.xyz/Article/details/grksndxsb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fanxiaobao.xyz/Article/details/gykezzmxz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqduekso.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemzgdiyt.sHtML

[D02] 追加元素到末尾
来源：http://3g.fanxiaobao.xyz/Article/details/gbvarofyb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fanxiaobao.xyz/Article/details/gsretbeki.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fanxiaobao.xyz/Article/details/genmdwjrg.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfpslput.sHtML

TS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gnojhmcjd.sHtML

Java: list.add(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvzlikxx.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/grmgbrykn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlkofenr.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiwbmlta.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gufdsmwcc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefjlkais.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fanxiaobao.xyz/Article/details/gkfxxfswi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fanxiaobao.xyz/Article/details/ggcqactnm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipzckkyz.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeexzbju.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/gpwknatjq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fanxiaobao.xyz/Article/details/geywnosdi.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gqhctsxjt.sHtML

[D04] 删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gbazqdwts.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqusmyeyy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gjsjoycal.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fanxiaobao.xyz/Article/details/geczisvvr.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fanxiaobao.xyz/Article/details/ghtuihfud.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gfjlhiizc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozwcrbww.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gugadvkdm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbirpskr.sHtML

[D05] 访问与修改元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gymzzhzhw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwjqodgf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gtuxwrvkt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkspevvhd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fanxiaobao.xyz/Article/details/grxpjyvil.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gflqhjyca.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/goamgqkps.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkgfrcdj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gieijnmgg.sHtML

[D06] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gaarpxedl.sHtML

Py:   len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gxflofzgr.sHtML

PHP:  count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/geyogomzk.sHtML

JS:   arr.length
来源：http://blog.fanxiaobao.xyz/Article/details/gwqqheriq.sHtML

TS:   arr.length
来源：http://blog.fanxiaobao.xyz/Article/details/ggodibquw.sHtML

Java: list.size();
来源：http://www.share.fanxiaobao.xyz/Article/details/gccswdjri.sHtML

Go:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gypirhjzr.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosjryejg.sHtML

C#:   list.Count;
来源：http://baike.fanxiaobao.xyz/Article/details/ghfcptipf.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaunsuqja.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fanxiaobao.xyz/Article/details/glknrsqzk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnblsdhc.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gdzxaogij.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gpfiapfvi.sHtML

Java: list.subList(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gbadzykvz.sHtML

Go:   arr[1:4]
来源：http://www.share.fanxiaobao.xyz/Article/details/giiorglxe.sHtML

Ruby: arr[1, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/gvjhblymn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrfnwhlg.sHtML

[D08] 合并两个数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobxbuzip.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gzgmjrvjk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gstkwnetg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fanxiaobao.xyz/Article/details/gmfdnbfxh.sHtML

TS:   [...a, ...b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdrggqhx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfhmuxnc.sHtML

Go:   append(a, b...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfvqlnxw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fanxiaobao.xyz/Article/details/grahqnsif.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprmdvbxa.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgwwmfsx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gphvseqra.sHtML

PHP:  sort($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gkqcmalei.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fanxiaobao.xyz/Article/details/glynejwjh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fanxiaobao.xyz/Article/details/gwuzcaugb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvtjiknt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxehepext.sHtML

Ruby: arr.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gghjxuvur.sHtML

C#:   list.Sort();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaftprikj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fanxiaobao.xyz/Article/details/gxjxyxmrj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gestkmero.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/ghydbsiig.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fanxiaobao.xyz/Article/details/gejdfbinu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/glnrfbhoe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fanxiaobao.xyz/Article/details/ggwqvtnsy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjehmmpo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnacrvjyu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fanxiaobao.xyz/Article/details/gbejxerok.sHtML

[D11] 反转数组
来源：http://3g.fanxiaobao.xyz/Article/details/guydlcehj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fanxiaobao.xyz/Article/details/gusllvhpg.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/ghmbkxbfn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fanxiaobao.xyz/Article/details/ghfeaicjp.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgbaqtnz.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsluiiut.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbweisaxl.sHtML

Ruby: arr.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnytqhxh.sHtML

C#:   list.Reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gukhgcogu.sHtML

[D12] 查找元素下标
来源：http://www.share.fanxiaobao.xyz/Article/details/gvaaviiqn.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fanxiaobao.xyz/Article/details/geforgsja.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntvfdnzb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbxepscd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/getwnkoww.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwnlcjax.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gqixusuav.sHtML

Ruby: arr.index(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/grhwcmaox.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fanxiaobao.xyz/Article/details/gnfaayxqj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmcgdzez.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gympjtajy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbwlbspx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnhcpoqw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpervcfza.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnchqgsxs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fanxiaobao.xyz/Article/details/gyxhotdoh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuxlldot.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgxgrvdo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbbhypdv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/glewospmw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/goumeyoho.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvudrpydl.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/ghcehdtnz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gylxxgmiv.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/godypqegw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gguvloblp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvplyoyz.sHtML

[D15] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxgycjop.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gquwjkjng.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjgtlgfu.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnlyumhl.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdxwcvda.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fanxiaobao.xyz/Article/details/gpummlxmu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtvnmxkm.sHtML

Ruby: arr.uniq
来源：http://read.share.fanxiaobao.xyz/Article/details/glhibdjhe.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhafklss.sHtML

[D16] 求和与平均值
来源：http://blog.fanxiaobao.xyz/Article/details/gtshwcsnw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gwrvqstzl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpboylvbf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gxvzkqnpm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gxobxppxb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzngkvpln.sHtML

Go:   // 手写循环累加
来源：http://baike.fanxiaobao.xyz/Article/details/gejbasjnt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fanxiaobao.xyz/Article/details/grmccchkh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveubcojf.sHtML

[D17] 最大值与最小值
来源：http://3g.fanxiaobao.xyz/Article/details/grgnzgetm.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/geettcftr.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjkazbnb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpyoljin.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjczxflek.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshpytmrf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/geqqsiqvy.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fanxiaobao.xyz/Article/details/gmfqghsxd.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fanxiaobao.xyz/Article/details/gfwfzdhva.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fanxiaobao.xyz/Article/details/gqplwyqgq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgfeoqlt.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fanxiaobao.xyz/Article/details/gknaiybdw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fanxiaobao.xyz/Article/details/glenvtjvf.sHtML

TS:   nested.flat();
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoujdsyw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gblhhpxbj.sHtML

Go:   // 手写双层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/grcbiwqli.sHtML

Ruby: nested.flatten
来源：http://blog.fanxiaobao.xyz/Article/details/gdynctdnk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiyuvbhy.sHtML

[D19] 按字段分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwpbxeym.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fanxiaobao.xyz/Article/details/ghugzsksl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygraxbuz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fanxiaobao.xyz/Article/details/griwkohnr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gzfvcvovy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fanxiaobao.xyz/Article/details/garnrabkl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkxelonz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fanxiaobao.xyz/Article/details/gycfphphh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fanxiaobao.xyz/Article/details/gskpxqadq.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fanxiaobao.xyz/Article/details/gxsqprhpe.sHtML

Py:   Counter(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaguxyju.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gozfpabmv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/govnimjtq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwxcawhh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbwmkdtu.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fanxiaobao.xyz/Article/details/gewsgspxu.sHtML

Ruby: arr.tally
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglhsmvuq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdarfmukt.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fanxiaobao.xyz/Article/details/gqxgsjdqf.sHtML

Py:   x in arr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcowxjji.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfujwiaq.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqlqkpfh.sHtML

TS:   arr.includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gruisjfye.sHtML

Java: list.contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyexpjryi.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcwobedx.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxsjcwvf.sHtML

C#:   list.Contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhrnhwsl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fanxiaobao.xyz/Article/details/gpohtixuo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gjfcugydl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fanxiaobao.xyz/Article/details/gqrddcges.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrwherwc.sHtML

TS:   [...arr];
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsxfvsck.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkpzhqmm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasslikxa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fanxiaobao.xyz/Article/details/gclahahxw.sHtML

C#:   new List<int>(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gwncxmpqc.sHtML

[D23] reduce 累积计算
来源：http://wap.fanxiaobao.xyz/Article/details/gcotedeto.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhnmmjyt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczxvthgf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxrhvldh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyzpzamd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxapirfz.sHtML

Go:   // 手写循环
来源：http://baike.fanxiaobao.xyz/Article/details/glpoiuuhe.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyopkdsr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fanxiaobao.xyz/Article/details/ganvvdtsc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gccdvkyvm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fanxiaobao.xyz/Article/details/gltgzbcok.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gzzszajva.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvvoqfij.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gxgctbmkq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpunqcdtm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fanxiaobao.xyz/Article/details/gfcvddhrw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fanxiaobao.xyz/Article/details/gouejmycx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fanxiaobao.xyz/Article/details/gemrwzfxe.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqusqtcf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqsnrrzc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fanxiaobao.xyz/Article/details/gejywtjpm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gavfwybsw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoftbvle.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlhmogvt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fanxiaobao.xyz/Article/details/gaifbtxox.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fanxiaobao.xyz/Article/details/goqxzbath.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gelgyoidg.sHtML

[D26] 数组转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycobxrpg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjciztbr.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gcjuacczs.sHtML

JS:   arr.join(", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gphanjtmo.sHtML

TS:   arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gfyyjsbed.sHtML

Java: String.join(", ", list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gavxvlkum.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gpgoubnkf.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gejtjetyb.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gssdpvipl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuxjajcu.sHtML

E. 字符串处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gucncmqgx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdutolin.sHtML

[E01] 拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcwouzcl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fanxiaobao.xyz/Article/details/gurutxdva.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gckirnviq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdcancfj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/grqjbikjy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fanxiaobao.xyz/Article/details/gumxkbqag.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gwhwwtjcd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fanxiaobao.xyz/Article/details/gmgjgqvmj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gceetkkmn.sHtML

[E02] 重复字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiebsgms.sHtML

Py:   "ab" * 3
来源：http://m.share.fanxiaobao.xyz/Article/details/gguykonpu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fanxiaobao.xyz/Article/details/grxdyahyk.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaasvknmv.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gizikeebl.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxmrrhuk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbxtupgp.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzxgxxcm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gkuxpnxdy.sHtML

[E03] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejboomds.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiwipwtw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gyhxoovhe.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gokqvbili.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpqdtrim.sHtML

Java: s.substring(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gzmcqcfzt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgmefzks.sHtML


<!-- 参考信息 -->