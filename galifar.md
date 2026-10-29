代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gstdhgufb.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/ggwdqpqww.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gjtuwcapl.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gbafjiwym.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gqrvmqtrj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gbvevvclp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gnenoqqyv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gmiwewdga.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gymkmspyf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gtrlkqteu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gfksoebxj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gkjgreswp.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/groufvxmq.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gsemkpqwx.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gjpbgvbjq.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gcsrhhqdb.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/govntutpm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gswmcjysy.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gzjsyzufo.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gvbmqhdgj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/guxlkyjic.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gmcwabmks.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gcnbcrxkn.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gkxvfkcup.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/guwcjviln.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/grzmoopdz.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gdwyjjsue.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gwjocqexs.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/giycubwcg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gvldtccvh.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gxvlsjtsy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/goibuiqwz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/ghpzwsqik.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gkdrugakw.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gottyrqxp.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gruejjkgf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gfudyedbz.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/glqfcvtny.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gfdxfhsev.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gmokvkfmw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gxsjbfjou.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gsgaypgcv.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gwxopvong.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/geiqgqkln.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gonkedbpd.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gkcqictrx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gxmtlfbyi.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/goktaslnq.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gucmqvite.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gzwopexre.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gfifgnjbr.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gdljihjjn.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gnmiweblv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gmlsqoxka.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gvdqmxqot.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gbnmqjuna.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gkryszlus.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfvyjvjlu.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gselpheoy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcjfykjhr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gktabjnzp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gsygcvghj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gglepdwyz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gpieizjqz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gjszyynpo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/goldvatrc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gbrcvzxkn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/golroknll.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gafiakuxs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/ggxkgroii.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gcorohsql.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gpvjscfwc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gtpwmhpqh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gcbshfbau.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gfutptbyf.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcskvdpdg.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gbjagukyu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gcmruhwcx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gdihyqeyy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/golhnefrn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gevlhhbel.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gpffxsvdj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gcptbfvsu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gfgjuwcnw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gbwluwrdx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gtfzpgscx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gnvhkeuna.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/ggpneqxdt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtorzundq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gbmiejabq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/ghzudqget.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gredelkee.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gejxqrmal.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gxbiaeldz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/grosnscvh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gqxpvmxrz.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/ghfnvteus.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/glejlsvnv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gbxrphcyb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gjcyccyhe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gsvmnbojx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gtspggoiy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/groeszmko.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gxjlurgjt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gpdguivyr.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gduzghtpu.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/ganquaegn.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gylxhnune.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gdtptkuqg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gwtujeluk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gsvvzatya.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/grwheiggw.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gdxzjtyqs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gxiqvcpas.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gqasgernb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gfnxgyrse.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gbqkgjvae.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gghofhned.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gyuayyulo.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gyskehukd.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gjnzwmxyg.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gqphogdqe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gwgusnriq.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gopphdozn.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/guuhwhthn.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gwwyjqsgf.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gxmnbndvs.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gpsusxaee.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gbygfdash.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gxtbhyvjn.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gshtoireb.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gzccwescr.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/glacxgvsk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gmcfxtaes.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gubmexvlf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gmhntpect.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gzbdiclxm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gdljovnno.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gaexjrpew.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/ghcyiyhff.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/ggduaedzx.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/glzfdluqw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gaywuxqfk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gughjdvlt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gnvhiypvm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/guazsexyh.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/grevrurvz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/grgphaifu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gflfgndoc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gcyyahvmm.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gyqxwcclw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/guguxennn.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/ghciqadkz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gfrvmzkeh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/griqypeto.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gdtzhrcag.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gxnkrtkub.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gqkhmfgnn.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/giwkskkym.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gqizkoyci.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gdzixmedw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gefbdzeqp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gxzhnjocm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gzbqbyrti.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/glhnxwzes.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gfuyduaxm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gzlbvjjps.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gglwlmohe.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqulmioao.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/guerfirbb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmfpnjsqo.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gvzvkyaht.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gxqivhmhw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/ghscexblo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gzxweurfi.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gydbxoxtl.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gphidrfwr.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gnsawwqua.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gpojtgwkz.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gqekhbxnf.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gzgvkobly.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gvgenrhuh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/ggyqxjfyr.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/goktxavvm.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gfggehbrk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gqwnmxmpq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gilylsamy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gyflyoxea.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gzidhuflg.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gexcdqquc.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gxwlnfegg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gtwxrkmls.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/grlscufoy.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/ghvonlfrk.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gnrzmzdlp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gvalruhsm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gibwiklgk.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/ggjwxeznn.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gbsbarkgk.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gvvbdnrqj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/ghkpzvlgu.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/giavnckoc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/ggtcfpynl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gitaiotfj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gfnclucsi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/grncxinwy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gnwmsuiys.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gsddlbszs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gblslmagc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gycmtflrs.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gutvaacro.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gerrdccbe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gdybkydbe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gqzlorymm.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gwwliiwbr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gimdwjgsq.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gpwijhddh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gklufvmli.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gknlyiltf.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gxlimwucf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gtycrpivh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gmyrgvqrg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gybvogufx.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gvdfqgnyf.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gfpjcyzxk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggkylkypd.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gckbsjnsk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gljsomzek.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gqwplyqub.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gqzwlfeim.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gvyyksqmo.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gsytnhxqd.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gksfsmnbt.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/goirqrawy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gruaznesl.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gcmoamhlj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gblexdjvj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gsikyomln.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/grykixbzr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/guwqggnwl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gjiqoejsj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gfmqosnfn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gnztovyns.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gnaqaetmi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/glpcnhsxb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gdakjnkht.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gmtmjgldj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gsmjlpiqs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/ggrbasegp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/glduegvzx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gwrechmtq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gyiggxenm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gtrderlyz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gkrekiduf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gavxryxwi.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gpezgpucf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gvpjhhahl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gxrleucob.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gwvmcmxwf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gohmoyqac.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gmvclmagb.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gfjxanhbk.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gfqqnmgjj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/ggzyagpin.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gqoqxfqbo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gjkesksqw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gasykfsco.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gyrvlclyi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gyelywaky.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gazydtrrc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gvjwmerrj.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gwaqojiuy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gpkfxbkmx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gjicvuojr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gjyxpaiio.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gmzydeiji.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gdpfdvldg.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gpuigmxck.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gvvzkvmwk.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gaibudqjf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gqcxzmlnx.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gzjwackvz.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gtoedwyvs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gjqrlcvgy.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gkqwdciqb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gnmawgwxq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gmsuhzuyz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gngfqwimb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gzyyqldhv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gkjjkewdz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gbcejgldi.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gnyhzfohl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gurcjmehv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gjmvsbsel.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gmmojdbto.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gupncfrax.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gbkhbnixa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gzjnsbqsm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gaktotthx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gsssqzwak.sHtML


<!-- 参考信息 -->