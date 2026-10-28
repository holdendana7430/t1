代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shanyushiyangkeji.top/gtryxynjwr.html

[R56] 远程拷贝
来源：http://hz.chenzaomai.com/gtmhuwezhy.html

scp file user@host:/path/
来源：http://hz.yangfankeji.com/gtgczskzkz.html

[R57] 远程执行命令
来源：http://hz.iojbl.cn/gtfbkbsrox.html

ssh user@host 'uptime'
来源：http://hz.chenzaomai.com/gtfduudhmt.html

[R58] 下载文件
来源：http://hz.daria6918.cn/gttkkolfzy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj20258888.top/gtsyigdhjc.html

[R59] 发 POST JSON
来源：http://hz.c1oappe.top/gtpevtnxbk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.meibo888.top/gtxzwpvmrc.html

[R60] 只看 HTTP 状态码
来源：http://hz.hysaishi.cn/gtanntvsei.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ybcxt.top/gteipjvgtg.html

[R61] 磁盘占用
来源：http://hz.yvedp.cn/gtdhpqqtmt.html

df -h;  du -sh *
来源：http://hz.meibo888.top/gtdjfuyzhl.html

[R62] 找最占空间的文件
来源：http://hz.xylfe.cn/gtsartrkit.html

du -ah . | sort -rh | head -10
来源：http://hz.kuanghao11.cn/gtakklamqc.html

[R63] 内存与进程
来源：http://hz.shzxlz.cn/gtticzprso.html

free -h;  ps aux | grep nginx
来源：http://hz.zhiwuduotai.top/gtxhhicssr.html

[R64] 结束进程
来源：http://hz.havefunace.top/gtublrafwj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tanke756.top/gtfgphlfsa.html

[R65] 查看端口占用
来源：http://hz.yuanzhike.top/gtygkbbhkm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.52xcode.cn/gtwamoamsb.html

[R66] 定时任务
来源：http://hz.wangshuangyany.cn/gtgttmjajd.html

crontab -e;  crontab -l
来源：http://hz.jinghuilouyu.cn/gteaitebpj.html

[R67] 生成随机十六进制串
来源：http://hz.xziqi.cn/gtheilwqjo.html

openssl rand -hex 16
来源：http://hz.sysykeji.top/gtabqfovep.html

[R68] 计算文件校验值
来源：http://hz.jinyuanbaomall.cn/gtrvewxltt.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ydzc1.top/gtfkrhtwyd.html

[R69] 生成随机密码
来源：http://hz.bjfxy.top/gtsmbzscwt.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinghuilouyu.cn/gttatncsdm.html

[R70] 时间戳与互转
来源：http://hz.pycfn.com/gtxydjxhft.html

date +%s;  date -d @1700000000
来源：http://hz.yueranfly.top/gtjxsyfozc.html

[R71] 日期格式化
来源：http://hz.vqdsnc.cn/gtioqisqvt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jqgfzy.top/gtyzybafuq.html

[R72] 等待端口就绪
来源：http://hz.zhengqikj.top/gtiuswrdai.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gtslewzvja.html

[R73] 分割大日志
来源：http://hz.dashuyun.cn/gtnyepvdme.html

split -l 1000 big.log part_
来源：http://hz.sxryk.cn/gtijnyejgi.html

[R74] 批量重命名
来源：http://hz.havefunace.top/gtxumaeblh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.bjfxy.top/gtecpctjle.html

[R75] 导出环境变量
来源：http://hz.52xcode.cn/gtwgyjfpod.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.52xcode.cn/gtejuawprk.html

[R76] 使用临时文件
来源：http://hz.xuanzx.com/gtxyckzvnn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinghuilouyu.cn/gtquscmaur.html

[R77] 读取用户输入
来源：http://hz.snrcjt.cn/gtyrlskhyq.html

read -rp "请输入: " ans
来源：http://hz.9152youxi.cn/gtblxxrxpx.html

[R78] 交互式菜单
来源：http://hz.gzhubu.top/gtswlcmliv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.haohaochexian.top/gtsovlaigx.html

[R79] 解析命令行选项
来源：http://hz.yuxming.cn/gtxzvjxior.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.316326.xyz/gtksmqpmrk.html

[R80] 查看脚本执行耗时
来源：http://hz.xingfuxueyuan.xyz/gterfdjema.html

time ./run.sh
来源：http://hz.sxryk.cn/gtehuanmmj.html

================================================================================
来源：http://hz.ydjk.org.cn/gttddinwlv.html

S. C / C++ 专题
来源：http://hz.dianchejie.cn/gttxnkhdzr.html

================================================================================
来源：http://hz.aibaodan.cn/gtzijodyfd.html

[S01] C：Hello World
来源：http://hz.ydzc1.top/gteclglngr.html

#include <stdio.h>
来源：http://hz.yj20258888.top/gtievhzjqe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.daria6918.cn/gtsimkiamk.html

[S02] C：变量与格式化输出
来源：http://hz.yanxiufei.cn/gtlrzvxwin.html

int a = 10; printf("%d\n", a);
来源：http://hz.sysykeji.top/gtmwnngwvp.html

[S03] C：读入整数
来源：http://hz.ydzc1.top/gtmssupnpl.html

int x; scanf("%d", &x);
来源：http://hz.gzhubu.top/gtbxrwfyxf.html

[S04] C：字符串复制
来源：http://hz.ydzc1.top/gtgufkhvry.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.redwolf501.top/gtmugftnth.html

[S05] C：字符串长度
来源：http://hz.ppjwa.cn/gtrgaqtstd.html

strlen(s)
来源：http://hz.cqqwz.cn/gtoprlshty.html

[S06] C：字符串比较
来源：http://hz.gogol.net.cn/gtxrdznqli.html

strcmp(a, b) == 0
来源：http://hz.pycfn.com/gttsbiiiht.html

[S07] C：数组遍历求和
来源：http://hz.jinqigfzy.top/gtvdaycykw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xinyue.icu/gtvviakoka.html

[S08] C：动态内存分配与释放
来源：http://hz.chenjidiqi.icu/gtuthwdorx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.c1oappe.top/gtiffdisxz.html

[S09] C：结构体定义与初始化
来源：http://hz.chenjidiqi.icu/gtjpiziosa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.bjfxy.top/gtrenfdsyo.html

[S10] C：指针与解引用
来源：http://hz.daria6918.cn/gtitjywrqn.html

int *p = &a;  *p = 5;
来源：http://hz.guowangkeji.top/gtatfnzsho.html

[S11] C：逐行读文件
来源：http://hz.sxryk.cn/gtbprnlesz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinghuilouyu.cn/gtpqhdrpdx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tanke756.top/gtaqonnoxo.html

fclose(f);
来源：http://hz.svipenyu.cn/gtsvqdcpxn.html

[S12] C：写文件
来源：http://hz.jinqigfzy.top/gtwcbqjyer.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.fzhhl.top/gtizrypkdf.html

[S13] C：宏定义
来源：http://hz.jyoumei.cn/gtkiqnrmlm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jiagoushi.top/gtzgoyqniz.html

[S14] C：枚举
来源：http://hz.52xcode.cn/gtkuduapxd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yueranfly.top/gtepdnwhnh.html

[S15] C：类型转换
来源：http://hz.wangdashe.top/gtjwylvdlg.html

(double) a / b
来源：http://hz.yangfankeji.com/gtqptyjwip.html

[S16] C：位操作置位
来源：http://hz.0kj1m.cn/gtubyrghvx.html

x |= (1 << 3);
来源：http://hz.sufxvd.cn/gtjjehywyr.html

[S17] C：安全拼接字符串
来源：http://hz.jinqigfzy.top/gtbfrxxfjf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cashguo.top/gtxrnizsiu.html

[S18] C：命令行参数
来源：http://hz.sysykeji.top/gtmgvhehpb.html

int main(int argc, char **argv)
来源：http://hz.vqdsnc.cn/gtvvymvesg.html

[S19] C：快速排序
来源：http://hz.meibo888.top/gtvhymwfft.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtiuyhatug.html

[S20] C：二分查找
来源：http://hz.yongpay.top/gtuwqjgdrm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gtxlnaxtjv.html

[S21] C：字符类别判断
来源：http://hz.nanxuanxn.top/gtyqniemuo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hywenlv.cn/gtlveakcwk.html

[S22] C：字符串转数字
来源：http://hz.jyoumei.cn/gtqixxllkp.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.9152youxi.cn/gtndkumxzx.html

[S23] C：随机数
来源：http://hz.jinyuanbaomall.cn/gtykzpttxh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.vqdsnc.cn/gtiajmfhho.html

[S24] C：获取本地时间
来源：http://hz.zdqjudy.top/gtmknlujrs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zycfv.cn/gtsizcwepv.html

[S25] C：内存拷贝
来源：http://hz.hongshengwenyu.top/gttlducpke.html

memcpy(dst, src, n);
来源：http://hz.bjfxy.top/gtadrjsouo.html

[S26] C：内存清零
来源：http://hz.hnxiangtu.top/gtpocukmms.html

memset(a, 0, sizeof a);
来源：http://hz.xylfe.cn/gtpiloehwg.html

[S27] C：定义常量
来源：http://hz.xingfuxueyuan.xyz/gtnhmkdzxc.html

const double PI = 3.14159;
来源：http://hz.chenzaomai.com/gtutzktitl.html

[S28] C：静态变量
来源：http://hz.gogol.net.cn/gtcqcafhuu.html

static int counter = 0;
来源：http://hz.sweek.top/gtrshcwvoy.html

[S29] C：变参函数
来源：http://hz.yanxiufei.cn/gtvtjacdoo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhiwuduotai.top/gtptldgnis.html

[S30] C：头文件保护
来源：http://hz.wangdashe.top/gtlvtyraye.html

#ifndef X_H
来源：http://hz.sxryk.cn/gtjaqnbvkz.html

#define X_H
来源：http://hz.dashuyun.cn/gtpcudwrqp.html

#endif
来源：http://hz.birdmap.top/gtxxljqazk.html

[S31] C++：Hello World
来源：http://hz.yj202588.top/gtggvlbmlk.html

#include <iostream>
来源：http://hz.xuanzx.com/gtokyecily.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.c1oappe.top/gtprdkpgjz.html

[S32] C++：字符串
来源：http://hz.zhaomingkeji.xyz/gteegaypqm.html

std::string s = "hi";  s += "!";
来源：http://hz.yvedp.cn/gtwbflpmhs.html

[S33] C++：vector 增删
来源：http://hz.guowangkeji.top/gtviflzkwb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jyoumei.cn/gtynxvgttd.html

[S34] C++：遍历 vector
来源：http://hz.chenjidiqi.icu/gtvisppdra.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tian-w.cn/gtngtomkch.html

[S35] C++：map
来源：http://hz.xingfuxueyuan.xyz/gtlxwffcqo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yanxiufei.cn/gtcofezzti.html

[S36] C++：unordered_map
来源：http://hz.wangshuangyany.cn/gtbghhiysy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigufen.top/gtztarjrdp.html

[S37] C++：set
来源：http://hz.hysaishi.cn/gtfmgncjjn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nanxinkj.top/gtyqqxwhfq.html

[S38] C++：排序
来源：http://hz.sysykeji.top/gtywnvrbad.html

std::sort(v.begin(), v.end());
来源：http://hz.feifeiyinyue.top/gtoifqkzfc.html

[S39] C++：自定义比较器排序
来源：http://hz.hnqzz.top/gtxhqhvvrt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.haohaochexian.top/gtqkyvulns.html

[S40] C++：查找元素
来源：http://hz.jinghuilouyu.cn/gtfccdaqjl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yonumen.top/gtqmpiucgn.html

[S41] C++：类与构造函数
来源：http://hz.ydzc1.top/gtuaajmvvb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yanxiufei.cn/gtjkuzzsyy.html

[S42] C++：继承与虚函数
来源：http://hz.tian-w.cn/gtnnykvwwy.html

class B : public Base { public: void f() override {} };
来源：http://hz.yongpay.top/gttzkidvjb.html

[S43] C++：智能指针
来源：http://hz.zhiwuduotai.top/gtvibqkeko.html

auto p = std::make_unique<int>(5);
来源：http://hz.316326.xyz/gtejtabuzv.html

[S44] C++：引用传参
来源：http://hz.ydjk.org.cn/gtaycnhyis.html

void inc(int &x) { ++x; }
来源：http://hz.iojbl.cn/gtkpjtmtkj.html

[S45] C++：lambda
来源：http://hz.xuanzx.com/gthoojjhsh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.wangdashe.top/gtmfrxcifx.html

[S46] C++：函数模板
来源：http://hz.xuetiantiany.cn/gtavyfuacf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shuidangran.top/gtposcbzeq.html

[S47] C++：结构化绑定遍历
来源：http://hz.aibaodan.cn/gtgmaqwpaw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangshuangyany.cn/gtbxmrchsx.html

[S48] C++：逐行读文件
来源：http://hz.fengsongda.top/gtrlgmeoxl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yanxiufei.cn/gtzhhxzjty.html

while (std::getline(in, line)) { }
来源：http://hz.shangyingyoupin.top/gtarmljzdz.html

[S49] C++：写文件
来源：http://hz.chenzaomai.com/gtfvdqchht.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhaomingkeji.xyz/gtcxwfrztk.html

[S50] C++：格式化数字
来源：http://hz.zhongyouzk.top/gtsqxfxfyt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.birdmap.top/gtegrgxenq.html

[S51] C++：显式类型转换
来源：http://hz.nanxinkj.top/gtfpzqcvwt.html

static_cast<double>(a) / b
来源：http://hz.jyoumei.cn/gtctdlslwb.html

[S52] C++：const 与 noexcept
来源：http://hz.shzxlz.cn/gtjoencqhi.html

int size() const noexcept { return n_; }
来源：http://hz.sysykeji.top/gtsgrergku.html

[S53] C++：移动语义
来源：http://hz.jyoumei.cn/gtjzecliyk.html

std::vector<int> w = std::move(v);
来源：http://hz.xylfe.cn/gtzbmivcrf.html

[S54] C++：异常处理
来源：http://hz.chenjidiqi.icu/gtesbodllo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.kuanghao11.cn/gtmtosdkbq.html

[S55] C++：结构化绑定
来源：http://hz.smart0.xyz/gtbtbhzoks.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.fzhhl.top/gtaipsphfn.html

[S56] C++：optional
来源：http://hz.shanyushiyangkeji.top/gtwluwakon.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jianghu66.top/gtigxqlxzj.html

[S57] C++：编译期常量
来源：http://hz.yongpay.top/gtnsqrxjsw.html

constexpr int N = 10;
来源：http://hz.jinqigfzy.top/gtjymyxfhl.html

[S58] C++：命名空间
来源：http://hz.hnqzz.top/gtmrmnqzlu.html

namespace ns { int f() { return 1; } }
来源：http://hz.redwolf501.top/gtaazfbjlc.html

[S59] C++：静态断言
来源：http://hz.smart0.xyz/gtdbplmygq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cashguo.top/gtnyupkaze.html

[S60] C++：遍历并删除元素
来源：http://hz.gzhubu.top/gtkjtqfqio.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ybcxt.top/gtnlpijlqr.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtqevkvuuu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cdnleiting.top/gtnrqrchik.html

================================================================================
来源：http://hz.tianlin.xyz/gtzlzrpshh.html

[T01] Kotlin：Hello World
来源：http://hz.ppjwa.cn/gtmvsjlixs.html

println("Hello")
来源：http://hz.meibo888.top/gtnusomowt.html

[T02] Kotlin：变量
来源：http://hz.xuetiantiany.cn/gtnotbzvve.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ppjwa.cn/gthtzqwrhw.html

[T03] Kotlin：字符串模板
来源：http://hz.gotoacloud.top/gtnloxifvy.html

"值: $b"
来源：http://hz.gaohongyu789.top/gtcregbvpu.html

[T04] Kotlin：空安全
来源：http://hz.havefunace.top/gtpprrraqo.html

val n: String? = null;  n?.length
来源：http://hz.aizwys.cn/gtrywnquap.html

[T05] Kotlin：when 表达式
来源：http://hz.zdqjudy.top/gtnbpbfunc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yj20258.top/gtwphwunlt.html

[T06] Kotlin：集合映射
来源：http://hz.zycfv.cn/gtevkoectu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sufxvd.cn/gtrzhfuuhn.html

[T07] Kotlin：集合过滤
来源：http://hz.vqdsnc.cn/gtoxvyyylb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shzxlz.cn/gtctissupp.html

[T08] Kotlin：数据类
来源：http://hz.daxiang520.top/gtjedeupmj.html

data class User(val name: String, val age: Int)
来源：http://hz.zdqjudy.top/gtidocywvp.html

[T09] Kotlin：扩展函数
来源：http://hz.ppjwa.cn/gterbulwln.html

fun String.exclaim() = this + "!"
来源：http://hz.ybcxt.top/gtltlflzfl.html

[T10] Kotlin：默认参数
来源：http://hz.svipenyu.cn/gtwtldvpmh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xziqi.cn/gtvcjwlcxt.html

[T11] Kotlin：协程
来源：http://hz.xylfe.cn/gthtqbmsvl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xziqi.cn/gtguivyqnn.html

[T12] Kotlin：解构声明
来源：http://hz.yuanzhike.top/gtmthwiwnc.html

val (a, b) = Pair(1, 2)
来源：http://hz.meibo888.top/gtaxtejpmg.html

[T13] Kotlin：只读 Map
来源：http://hz.gotoacloud.top/gtdqqgrcnj.html

val m = mapOf("a" to 1)
来源：http://hz.ybcxt.top/gtnlkphpul.html

[T14] Kotlin：循环
来源：http://hz.daria6918.cn/gtfvuknaap.html

for (i in 1..10) println(i)
来源：http://hz.fzhhl.top/gtxfppiesb.html

[T15] Kotlin：接口
来源：http://hz.guannengcc.top/gtxmhcwjby.html

interface Shape { fun area(): Double }
来源：http://hz.xylfe.cn/gtrxcjeaty.html

[T16] Swift：Hello World
来源：http://hz.gaohongyu789.top/gtgsyzipgl.html

print("Hello")
来源：http://hz.nanxuanxn.top/gticoxkphy.html

[T17] Swift：变量与常量
来源：http://hz.yvedp.cn/gtcxcjuccx.html

var a = 1;  let b = 2
来源：http://hz.chenzaomai.com/gthwrzlvlz.html

[T18] Swift：字符串插值
来源：http://hz.ivvv.top/gtjtsreecg.html

"值: \(b)"
来源：http://hz.xylfe.cn/gtcrcufeid.html

[T19] Swift：可选绑定
来源：http://hz.ppjwa.cn/gtwtsnfmbu.html

if let n = opt { print(n) }
来源：http://hz.pycfn.com/gtkloghemk.html

[T20] Swift：数组操作
来源：http://hz.shzxlz.cn/gtqjeyypao.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.iojbl.cn/gtwgazibcu.html

[T21] Swift：遍历
来源：http://hz.jqgufenzy.top/gtrhzdwter.html

for x in a { print(x) }
来源：http://hz.guowangkeji.top/gtvgnhaasy.html

[T22] Swift：字典
来源：http://hz.zycfv.cn/gtvhfdbxck.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.aibaodan.cn/gtmxttqyal.html

[T23] Swift：函数
来源：http://hz.andypj.xyz/gtdxncumga.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.vqdsnc.cn/gtuygtoncc.html

[T24] Swift：闭包
来源：http://hz.redwolf501.top/gtyghshumn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hywenlv.cn/gthhmokcmv.html

[T25] Swift：结构体
来源：http://hz.svipenyu.cn/gtyitmrpsb.html

struct P { var x: Int }
来源：http://hz.jlsjyb.cn/gtxdadzjfp.html

[T26] Swift：类与重写
来源：http://hz.jyoumei.cn/gtubtgezio.html

class A: Base { override func f() {} }
来源：http://hz.316326.xyz/gtfhdtepez.html

[T27] Swift：错误处理
来源：http://hz.xinyue.icu/gtusttsrpd.html

do { try f() } catch { print(error) }
来源：http://hz.guannengcc.top/gtwwubcfdl.html

[T28] Swift：枚举
来源：http://hz.zdqjudy.top/gtqlgdciue.html

enum Color { case red, green }
来源：http://hz.316326.xyz/gtyjiimpwe.html

[T29] Swift：guard 提前返回
来源：http://hz.sxryk.cn/gtpugpkblu.html

guard let x = opt else { return }
来源：http://hz.chenlongwang.top/gtqumoxilf.html

[T30] Swift：协议
来源：http://hz.sweek.top/gtvwzzpgrz.html

protocol Shape { func area() -> Double }
来源：http://hz.zhaomingkeji.xyz/gthdqcewid.html

[T31] Lua：Hello World
来源：http://hz.tianlin.xyz/gtxvsmqyvp.html

print("Hello")
来源：http://hz.hnqzz.top/gtljswlcyg.html

[T32] Lua：局部变量
来源：http://hz.xuanzx.com/gtekctoolt.html

local a = 1
来源：http://hz.ivvv.top/gtxpkofhyu.html

[T33] Lua：表（数组）
来源：http://hz.shangyingyoupin.top/gtoyjpsweg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.haohaochexian.top/gtxdusuyig.html

[T34] Lua：遍历表
来源：http://hz.9152youxi.cn/gtknvvauph.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gaohongyu789.top/gttnkuqbba.html

[T35] Lua：字典表
来源：http://hz.daria6918.cn/gtiqfvised.html

local d = { a = 1 };  d.b = 2
来源：http://hz.birdmap.top/gtdhmwadrk.html

[T36] Lua：函数
来源：http://hz.feifeiyinyue.top/gtukuwntjo.html

function add(a, b) return a + b end
来源：http://hz.tianlin.xyz/gtgxsrwpph.html

[T37] Lua：字符串拼接
来源：http://hz.ydzc1.top/gtppewtqte.html

"a" .. "b"
来源：http://hz.shanyushiyangtech.top/gtpiihbsdd.html

[T38] Lua：条件
来源：http://hz.gotoacloud.top/gtrcpisppl.html

if x > 0 then print("正") end
来源：http://hz.hysaishi.cn/gtrnzfwoug.html

[T39] Lua：模式匹配
来源：http://hz.yueranfly.top/gthxjpffqp.html

string.find(s, "%d+")
来源：http://hz.jqgfzy.top/gtproilyzw.html

[T40] Lua：元表
来源：http://hz.jianghu66.top/gtzhugjqiv.html

setmetatable({}, { __index = base })
来源：http://hz.vqdsnc.cn/gtmfrupgtp.html

[T41] Perl：Hello World
来源：http://hz.pengpengdd.cyou/gtsvsgaygy.html

print "Hello\n";
来源：http://hz.cheryme.top/gtcanmiirv.html

[T42] Perl：变量类型
来源：http://hz.hammf.cn/gtuslykylk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jqgufenzy.top/gtlxxytkyn.html

[T43] Perl：字符串插值
来源：http://hz.316326.xyz/gtaicvrbvy.html

"值: $a"
来源：http://hz.kuanghao11.cn/gtlcuesagu.html

[T44] Perl：条件
来源：http://hz.yangfankeji.com/gtrivnwkzz.html

if ($a > 0) { print "正"; }
来源：http://hz.cashguo.top/gtrwfejnvu.html

[T45] Perl：数组遍历
来源：http://hz.jinqigufen.top/gtkakwrpof.html

for my $x (@arr) { print $x; }
来源：http://hz.hammf.cn/gtuqmepplp.html

[T46] Perl：哈希操作
来源：http://hz.daxiang520.top/gtuiejhrxa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shanyushiyangkeji.top/gtlbscwuct.html

[T47] Perl：正则捕获
来源：http://hz.gogol.net.cn/gtcwyoovjv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sufxvd.cn/gtrpynjskk.html

[T48] Perl：正则替换
来源：http://hz.zdqjudy.top/gtydfuvtvd.html

$s =~ s/old/new/g;
来源：http://hz.yvedp.cn/gtzepbdldh.html

[T49] Perl：函数
来源：http://hz.hnqzz.top/gtbahubnjl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cashguo.top/gtircnxlva.html

[T50] Perl：逐行读文件
来源：http://hz.xziqi.cn/gtydcrutgm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.nwbrower.top/gtdpvzvtle.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.9152youxi.cn/gtmokzaskw.html

[T51] Scala：Hello World
来源：http://hz.jqgufenzy.top/gtlaujjyyp.html

println("Hello")
来源：http://hz.yonumen.top/gtssxqctrb.html

[T52] Scala：变量
来源：http://hz.haohaochexian.top/gtzbkzjdlw.html

val a = 1;  var b = 2
来源：http://hz.wangdashe.top/gtbfduwqbx.html

[T53] Scala：字符串插值
来源：http://hz.sysykeji.top/gtdlzmdwjk.html

s"值: $b"
来源：http://hz.fzhhl.top/gtvrmdsbua.html

[T54] Scala：集合映射
来源：http://hz.shanyushiyangtech.top/gtrkarfzyd.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jinyuanbaomall.cn/gtxskgjior.html

[T55] Scala：集合过滤
来源：http://hz.haohaochexian.top/gtjvpvvivp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ivvv.top/gtwflxlmtd.html

[T56] Scala：样例类
来源：http://hz.jiagoushi.top/gtjuuqnrrf.html

case class User(name: String, age: Int)
来源：http://hz.snrcjt.cn/gtjahlrxwv.html

[T57] Scala：模式匹配
来源：http://hz.jqgfzy.top/gtiztadwes.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.nanxuanxn.top/gtzckhuhza.html

[T58] Scala：函数定义
来源：http://hz.ybcxt.top/gtprxsngzp.html


<!-- 参考信息 -->