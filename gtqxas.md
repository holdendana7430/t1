代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhengqikj.top/gtydhhnxjq.html

[R56] 远程拷贝
来源：http://hz.hfpthk.cn/gtgznxwsqp.html

scp file user@host:/path/
来源：http://hz.xylfe.cn/gtdxszawyf.html

[R57] 远程执行命令
来源：http://hz.ivvv.top/gtjykhlkkb.html

ssh user@host 'uptime'
来源：http://hz.hnxiangtu.top/gtiaijqzrt.html

[R58] 下载文件
来源：http://hz.jqgufenzy.top/gtrywxdwjr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jianghu66.top/gtspgvyjzm.html

[R59] 发 POST JSON
来源：http://hz.andypj.xyz/gtmzgcbfvw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jqgfzy.top/gtpvkconxp.html

[R60] 只看 HTTP 状态码
来源：http://hz.gaohongyu789.top/gtxeoywibg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.kuanghao11.cn/gtvnwqajqr.html

[R61] 磁盘占用
来源：http://hz.aibaodan.cn/gtahivmxtz.html

df -h;  du -sh *
来源：http://hz.shanyushiyangtech.top/gtvbkshueq.html

[R62] 找最占空间的文件
来源：http://hz.yj20258.top/gtvntvqyho.html

du -ah . | sort -rh | head -10
来源：http://hz.yuxming.cn/gtdgduzyqk.html

[R63] 内存与进程
来源：http://hz.zhiwuduotai.top/gtthzzjgts.html

free -h;  ps aux | grep nginx
来源：http://hz.pycfn.com/gtqogipsub.html

[R64] 结束进程
来源：http://hz.gogol.net.cn/gtfgdvsxsx.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gogol.net.cn/gtvcbbhqfx.html

[R65] 查看端口占用
来源：http://hz.dianchejie.cn/gtwgzrgrkl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.fzhhl.top/gtiabnifii.html

[R66] 定时任务
来源：http://hz.xuanzx.com/gtlchmwnkr.html

crontab -e;  crontab -l
来源：http://hz.wangshuangyany.cn/gtoztxtkzb.html

[R67] 生成随机十六进制串
来源：http://hz.cucudq.cn/gtlgcjvwrf.html

openssl rand -hex 16
来源：http://hz.yj20258888.top/gtwozgtsys.html

[R68] 计算文件校验值
来源：http://hz.hnqzz.top/gtzioelbsl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhengqikj.top/gtqigmavsc.html

[R69] 生成随机密码
来源：http://hz.smart0.xyz/gtfytbjeey.html

head -c 16 /dev/urandom | base64
来源：http://hz.pycfn.com/gtutzjlcde.html

[R70] 时间戳与互转
来源：http://hz.bjfxy.top/gtlwrwxvug.html

date +%s;  date -d @1700000000
来源：http://hz.tanke756.top/gtvsgnifac.html

[R71] 日期格式化
来源：http://hz.yueranfly.top/gtpttqgxri.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinqigfzy.top/gtpkrryomv.html

[R72] 等待端口就绪
来源：http://hz.feifeiyinyue.top/gtzldbqrxj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtutjjythe.html

[R73] 分割大日志
来源：http://hz.svipenyu.cn/gtmrvqzgpj.html

split -l 1000 big.log part_
来源：http://hz.52xcode.cn/gtfuomnzgy.html

[R74] 批量重命名
来源：http://hz.kuanghao11.cn/gtfiyrcsqw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhengqikj.top/gtctodulfz.html

[R75] 导出环境变量
来源：http://hz.zhengqikj.top/gtsubygtax.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhengqikj.top/gtedhvylkh.html

[R76] 使用临时文件
来源：http://hz.mhx1999.top/gtbvzrkesi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cashguo.top/gtwzyyswym.html

[R77] 读取用户输入
来源：http://hz.yuxming.cn/gtecnksgro.html

read -rp "请输入: " ans
来源：http://hz.jinqigufen.top/gtvizhhftj.html

[R78] 交互式菜单
来源：http://hz.andypj.xyz/gtqgajtohm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tianlin.xyz/gtefddjefj.html

[R79] 解析命令行选项
来源：http://hz.shzxlz.cn/gttotaengq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenjidiqi.icu/gtlanqrtka.html

[R80] 查看脚本执行耗时
来源：http://hz.yvedp.cn/gtlawekbxc.html

time ./run.sh
来源：http://hz.yueranfly.top/gtrdofavhc.html

================================================================================
来源：http://hz.chenlongwang.top/gtxteifsjm.html

S. C / C++ 专题
来源：http://hz.jiagoushi.top/gtxmdqhzry.html

================================================================================
来源：http://hz.hysaishi.cn/gtmhmyllkw.html

[S01] C：Hello World
来源：http://hz.xuanzx.com/gtmhmatjgl.html

#include <stdio.h>
来源：http://hz.zycfv.cn/gtuvahlwdt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cdnleiting.top/gtnxlmvnqs.html

[S02] C：变量与格式化输出
来源：http://hz.feifeiyinyue.top/gthxdwucfi.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhiwuduotai.top/gtgnpwwebr.html

[S03] C：读入整数
来源：http://hz.hywenlv.cn/gtvmigzqfm.html

int x; scanf("%d", &x);
来源：http://hz.smart0.xyz/gtfasctgvo.html

[S04] C：字符串复制
来源：http://hz.zhoulong.xyz/gtdrkcsptf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hongshengwenyu.top/gtgxdfdohe.html

[S05] C：字符串长度
来源：http://hz.yangfankeji.com/gtpbytekmb.html

strlen(s)
来源：http://hz.hnxiangtu.top/gtuafwlelb.html

[S06] C：字符串比较
来源：http://hz.zhijiandao.cn/gtfcnwxedc.html

strcmp(a, b) == 0
来源：http://hz.ybcxt.top/gtagvmqkjp.html

[S07] C：数组遍历求和
来源：http://hz.hfpthk.cn/gtmcevevnv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nwbrower.top/gtdprniisg.html

[S08] C：动态内存分配与释放
来源：http://hz.jqgfzy.top/gtmlpktigu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigfzy.top/gtunfwtdaq.html

[S09] C：结构体定义与初始化
来源：http://hz.chenlongwang.top/gtlzjfzsum.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xuetiantiany.cn/gtfbnyobyc.html

[S10] C：指针与解引用
来源：http://hz.jlsjyb.cn/gtdwjsloce.html

int *p = &a;  *p = 5;
来源：http://hz.hnqzz.top/gtqdnmbrqt.html

[S11] C：逐行读文件
来源：http://hz.daria6918.cn/gtityvsroa.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.pycfn.com/gtiotrqtgm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenlongwang.top/gtzmcwxeol.html

fclose(f);
来源：http://hz.cdnleiting.top/gtlphyujzy.html

[S12] C：写文件
来源：http://hz.ydzc1.top/gtyggnsjec.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jianghu66.top/gthirssfqt.html

[S13] C：宏定义
来源：http://hz.cqqwz.cn/gtwznugpik.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xylfe.cn/gtxvdfmvfq.html

[S14] C：枚举
来源：http://hz.guannengcc.top/gtdtwvhtvs.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ywan-chungtsiang.top/gtvwykalbm.html

[S15] C：类型转换
来源：http://hz.0kj1m.cn/gtrsnshsyq.html

(double) a / b
来源：http://hz.kuanghao11.cn/gtpvrupjmx.html

[S16] C：位操作置位
来源：http://hz.wangdashe.top/gtnuronrte.html

x |= (1 << 3);
来源：http://hz.tianlin.xyz/gtvyolecfd.html

[S17] C：安全拼接字符串
来源：http://hz.jiagoushi.top/gtcvwfogva.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yanxiufei.cn/gtrcybwrqm.html

[S18] C：命令行参数
来源：http://hz.hnqzz.top/gtswcibjcc.html

int main(int argc, char **argv)
来源：http://hz.shanyushiyangtech.top/gttjnufqlo.html

[S19] C：快速排序
来源：http://hz.guowangkeji.top/gtvpurxdjm.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenjidiqi.icu/gtvzajvusr.html

[S20] C：二分查找
来源：http://hz.jiagoushi.top/gtnvtausqz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.guowangkeji.top/gteufwwkfd.html

[S21] C：字符类别判断
来源：http://hz.sxryk.cn/gtcigmdtkj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.316326.xyz/gtqyqlttdg.html

[S22] C：字符串转数字
来源：http://hz.shuidangran.top/gtjpqiqwcn.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yvedp.cn/gtdlljzvff.html

[S23] C：随机数
来源：http://hz.jinqigfzy.top/gthkqvgtkl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xuanzx.com/gtvngmiiuj.html

[S24] C：获取本地时间
来源：http://hz.xingfuxueyuan.xyz/gtonjgqdmk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258888.top/gtloexldxe.html

[S25] C：内存拷贝
来源：http://hz.dashuyun.cn/gtmqpwlzsu.html

memcpy(dst, src, n);
来源：http://hz.gogol.net.cn/gtsmgmlgyi.html

[S26] C：内存清零
来源：http://hz.0kj1m.cn/gtbzthcfsc.html

memset(a, 0, sizeof a);
来源：http://hz.chenlongwang.top/gttnsgvoxd.html

[S27] C：定义常量
来源：http://hz.aizwys.cn/gtpneahggj.html

const double PI = 3.14159;
来源：http://hz.c1oappe.top/gtudmgqwmn.html

[S28] C：静态变量
来源：http://hz.yueranfly.top/gtrnevxmdk.html

static int counter = 0;
来源：http://hz.yuanzhike.top/gtgkgvueiy.html

[S29] C：变参函数
来源：http://hz.yangfankeji.com/gtfhleopmz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yj202588.top/gtwttqepcv.html

[S30] C：头文件保护
来源：http://hz.kuanghao11.cn/gtrvcrwelr.html

#ifndef X_H
来源：http://hz.ivvv.top/gtkaonucfy.html

#define X_H
来源：http://hz.jqgfzy.top/gtuddgrcpc.html

#endif
来源：http://hz.hywenlv.cn/gtnrjemvqp.html

[S31] C++：Hello World
来源：http://hz.tanke756.top/gtmvwzbrod.html

#include <iostream>
来源：http://hz.jinyuanbaomall.cn/gtyhlenwvc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.guannengcc.top/gtngzleodz.html

[S32] C++：字符串
来源：http://hz.fengsongda.top/gttkakzysd.html

std::string s = "hi";  s += "!";
来源：http://hz.birdmap.top/gtypfqzmca.html

[S33] C++：vector 增删
来源：http://hz.aibaodan.cn/gtldofuagx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.wangdashe.top/gtgcivpaiz.html

[S34] C++：遍历 vector
来源：http://hz.xuetiantiany.cn/gtowbfvapu.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.guannengcc.top/gtuethptiw.html

[S35] C++：map
来源：http://hz.pengpengdd.cyou/gtzaoyxyfm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhiwuduotai.top/gtgcoyyxlw.html

[S36] C++：unordered_map
来源：http://hz.yonumen.top/gtslrbnqad.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gtgnzklpbc.html

[S37] C++：set
来源：http://hz.chenjidiqi.icu/gtruytlcop.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinqigfzy.top/gtlnosqugf.html

[S38] C++：排序
来源：http://hz.yangfankeji.com/gtpdivalmj.html

std::sort(v.begin(), v.end());
来源：http://hz.hammf.cn/gtyhdizwav.html

[S39] C++：自定义比较器排序
来源：http://hz.xinyue.icu/gtxlktnozq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cucudq.cn/gtickauyuj.html

[S40] C++：查找元素
来源：http://hz.guannengcc.top/gtznhrswqk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.haohaochexian.top/gtlcscycvs.html

[S41] C++：类与构造函数
来源：http://hz.snrcjt.cn/gtmhdibxhc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.dashuyun.cn/gtfgzztomm.html

[S42] C++：继承与虚函数
来源：http://hz.shanyushiyangtech.top/gtjwfrgkrr.html

class B : public Base { public: void f() override {} };
来源：http://hz.xinyue.icu/gtbxoybxpc.html

[S43] C++：智能指针
来源：http://hz.sxryk.cn/gtwjjaeuln.html

auto p = std::make_unique<int>(5);
来源：http://hz.xinyue.icu/gtlnbcomdv.html

[S44] C++：引用传参
来源：http://hz.yueranfly.top/gteojvfaxi.html

void inc(int &x) { ++x; }
来源：http://hz.cheryme.top/gtphykudys.html

[S45] C++：lambda
来源：http://hz.zhengqikj.top/gtkacnpmrm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.wangdashe.top/gtjaansclw.html

[S46] C++：函数模板
来源：http://hz.shzxlz.cn/gtciorqdsi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jyoumei.cn/gtmokdtaxt.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnqzz.top/gtjuqtaagp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangshuangyany.cn/gtwhcxgtbf.html

[S48] C++：逐行读文件
来源：http://hz.sysykeji.top/gtcqgezjpt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.iojbl.cn/gtoxfmijpq.html

while (std::getline(in, line)) { }
来源：http://hz.c1oappe.top/gtprglpzgi.html

[S49] C++：写文件
来源：http://hz.zhijiandao.cn/gtiafxsdcs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yangfankeji.com/gtdczhlirr.html

[S50] C++：格式化数字
来源：http://hz.hfpthk.cn/gtvdxdregc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhoulong.xyz/gtumwtwzcx.html

[S51] C++：显式类型转换
来源：http://hz.tianlin.xyz/gtqcqbatkx.html

static_cast<double>(a) / b
来源：http://hz.gogol.net.cn/gtayulxsgz.html

[S52] C++：const 与 noexcept
来源：http://hz.xingfuxueyuan.xyz/gtdjruuniu.html

int size() const noexcept { return n_; }
来源：http://hz.cqqwz.cn/gttqmtoyue.html

[S53] C++：移动语义
来源：http://hz.xylfe.cn/gtfkergmxp.html

std::vector<int> w = std::move(v);
来源：http://hz.ydjk.org.cn/gthhxkoyuo.html

[S54] C++：异常处理
来源：http://hz.hnqzz.top/gtlafzybnd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinghuilouyu.cn/gtptikwlou.html

[S55] C++：结构化绑定
来源：http://hz.chenjidiqi.icu/gtsxpbviux.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xingfuxueyuan.xyz/gtmctajwmu.html

[S56] C++：optional
来源：http://hz.shzxlz.cn/gtqdvpyotc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zycfv.cn/gticvfsjgj.html

[S57] C++：编译期常量
来源：http://hz.zhiwuduotai.top/gtdwwqnmzz.html

constexpr int N = 10;
来源：http://hz.jyoumei.cn/gtnrkhhqyo.html

[S58] C++：命名空间
来源：http://hz.redwolf501.top/gtsyiizjka.html

namespace ns { int f() { return 1; } }
来源：http://hz.yonumen.top/gtzepkvzqv.html

[S59] C++：静态断言
来源：http://hz.nwbrower.top/gtpjwsunkl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ywan-chungtsiang.top/gtuzfwwkwm.html

[S60] C++：遍历并删除元素
来源：http://hz.snrcjt.cn/gtftdknlvb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.c1oappe.top/gtgbartzgo.html

================================================================================
来源：http://hz.meibo888.top/gtsaplqrhb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sweek.top/gtwamcwhfv.html

================================================================================
来源：http://hz.9152youxi.cn/gtdwxdnxsa.html

[T01] Kotlin：Hello World
来源：http://hz.kuanghao11.cn/gttkmwuonq.html

println("Hello")
来源：http://hz.hammf.cn/gtqksjjbjx.html

[T02] Kotlin：变量
来源：http://hz.wangshuangyany.cn/gtlcmohfyv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xingfuxueyuan.xyz/gthvynimei.html

[T03] Kotlin：字符串模板
来源：http://hz.nwbrower.top/gtrjwczjzh.html

"值: $b"
来源：http://hz.smart0.xyz/gteqobtlhx.html

[T04] Kotlin：空安全
来源：http://hz.nanxinkj.top/gtiaajdlbj.html

val n: String? = null;  n?.length
来源：http://hz.yonumen.top/gtvutpozqj.html

[T05] Kotlin：when 表达式
来源：http://hz.xylfe.cn/gteglzyldn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.guannengcc.top/gtpcwscdmo.html

[T06] Kotlin：集合映射
来源：http://hz.nanxinkj.top/gtybiuzxxa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yangfankeji.com/gtpedfvizh.html

[T07] Kotlin：集合过滤
来源：http://hz.hnxiangtu.top/gtkpzmchlk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.bjfxy.top/gtlvmizsda.html

[T08] Kotlin：数据类
来源：http://hz.yj20258.top/gtuxzvffyd.html

data class User(val name: String, val age: Int)
来源：http://hz.gaohongyu789.top/gtxmxaloza.html

[T09] Kotlin：扩展函数
来源：http://hz.snrcjt.cn/gttqqhxjsm.html

fun String.exclaim() = this + "!"
来源：http://hz.0kj1m.cn/gtzhfqeayj.html

[T10] Kotlin：默认参数
来源：http://hz.jqgufenzy.top/gttcnnvvoy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhongyouzk.top/gtwxouwsfj.html

[T11] Kotlin：协程
来源：http://hz.52xcode.cn/gtfpfifdqs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.dashuyun.cn/gtelwvutmz.html

[T12] Kotlin：解构声明
来源：http://hz.yuxming.cn/gtirepjjqo.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenjidiqi.icu/gtdojbzsxh.html

[T13] Kotlin：只读 Map
来源：http://hz.shanyushiyangtech.top/gtawkmroax.html

val m = mapOf("a" to 1)
来源：http://hz.zhiwuduotai.top/gtlzjuspox.html

[T14] Kotlin：循环
来源：http://hz.jqgufenzy.top/gtfebqqljy.html

for (i in 1..10) println(i)
来源：http://hz.nanxinkj.top/gtfnqacirx.html

[T15] Kotlin：接口
来源：http://hz.gogol.net.cn/gtgzjdckah.html

interface Shape { fun area(): Double }
来源：http://hz.yj20258888.top/gtaakewhlj.html

[T16] Swift：Hello World
来源：http://hz.havefunace.top/gtqnjipeqk.html

print("Hello")
来源：http://hz.zhaomingkeji.xyz/gtbgvphfmt.html

[T17] Swift：变量与常量
来源：http://hz.dashuyun.cn/gtfpdybvpl.html

var a = 1;  let b = 2
来源：http://hz.jiagoushi.top/gtyrccyauk.html

[T18] Swift：字符串插值
来源：http://hz.zycfv.cn/gttlzleivl.html

"值: \(b)"
来源：http://hz.zhongyouzk.top/gtoiswpnqb.html

[T19] Swift：可选绑定
来源：http://hz.c1oappe.top/gtkjuigwga.html

if let n = opt { print(n) }
来源：http://hz.havefunace.top/gtprkrybqu.html

[T20] Swift：数组操作
来源：http://hz.havefunace.top/gtkjlqnxth.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gotoacloud.top/gtcwrqtbdp.html

[T21] Swift：遍历
来源：http://hz.ybcxt.top/gtrpwkqdfh.html

for x in a { print(x) }
来源：http://hz.c1oappe.top/gtmsmxqers.html

[T22] Swift：字典
来源：http://hz.cqqwz.cn/gtyctnxrwq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hywenlv.cn/gtwxryhooo.html

[T23] Swift：函数
来源：http://hz.mhx1999.top/gtzhrekhgn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.andypj.xyz/gtitwfpbva.html

[T24] Swift：闭包
来源：http://hz.gogol.net.cn/gtoornxzln.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhixingplan.top/gtxseqzupc.html

[T25] Swift：结构体
来源：http://hz.gogol.net.cn/gthtjccsmx.html

struct P { var x: Int }
来源：http://hz.gotoacloud.top/gtacjvnsgt.html

[T26] Swift：类与重写
来源：http://hz.yj20258.top/gtxjigwobo.html

class A: Base { override func f() {} }
来源：http://hz.gzhubu.top/gtgehdcpns.html

[T27] Swift：错误处理
来源：http://hz.xziqi.cn/gtzldncgzb.html

do { try f() } catch { print(error) }
来源：http://hz.shangyingyoupin.top/gthaemjghr.html

[T28] Swift：枚举
来源：http://hz.nanxinkj.top/gtopbvputs.html

enum Color { case red, green }
来源：http://hz.hnxiangtu.top/gtvudiiqmi.html

[T29] Swift：guard 提前返回
来源：http://hz.hysaishi.cn/gtgmxywfqz.html

guard let x = opt else { return }
来源：http://hz.aibaodan.cn/gtdfwbkvyk.html

[T30] Swift：协议
来源：http://hz.jinqigufen.top/gtvofsgdjb.html

protocol Shape { func area() -> Double }
来源：http://hz.daxiang520.top/gtqbzhdssf.html

[T31] Lua：Hello World
来源：http://hz.guannengcc.top/gtjtnwjsuj.html

print("Hello")
来源：http://hz.shangyingyoupin.top/gtocrzcgxu.html

[T32] Lua：局部变量
来源：http://hz.ppjwa.cn/gtxjagxohg.html

local a = 1
来源：http://hz.jianghu66.top/gtzzroqmge.html

[T33] Lua：表（数组）
来源：http://hz.havefunace.top/gthuoxxsxz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhengqikj.top/gtvxrigomm.html

[T34] Lua：遍历表
来源：http://hz.meibo888.top/gtvjrpdjdc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cashguo.top/gtwtgoplol.html

[T35] Lua：字典表
来源：http://hz.gaohongyu789.top/gtpdnowupg.html

local d = { a = 1 };  d.b = 2
来源：http://hz.nanxinkj.top/gtwenobwpm.html

[T36] Lua：函数
来源：http://hz.hongshengwenyu.top/gtjcimnkdh.html

function add(a, b) return a + b end
来源：http://hz.jinghuilouyu.cn/gttvucvxth.html

[T37] Lua：字符串拼接
来源：http://hz.zhoulong.xyz/gtjfaizcrw.html

"a" .. "b"
来源：http://hz.nanxuanxn.top/gtsptgzogq.html

[T38] Lua：条件
来源：http://hz.nwbrower.top/gtnhvkmxqk.html

if x > 0 then print("正") end
来源：http://hz.hongshengwenyu.top/gtfncuqhru.html

[T39] Lua：模式匹配
来源：http://hz.svipenyu.cn/gtiegszzhl.html

string.find(s, "%d+")
来源：http://hz.haohaochexian.top/gtplxhnweq.html

[T40] Lua：元表
来源：http://hz.xuetiantiany.cn/gtuockwluq.html

setmetatable({}, { __index = base })
来源：http://hz.yongpay.top/gtspdiohzf.html

[T41] Perl：Hello World
来源：http://hz.ydzc1.top/gtsjpeajpg.html

print "Hello\n";
来源：http://hz.hnxiangtu.top/gtthhkmwvi.html

[T42] Perl：变量类型
来源：http://hz.pycfn.com/gtpwwzvmun.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fzhhl.top/gtgrycexil.html

[T43] Perl：字符串插值
来源：http://hz.shangyingyoupin.top/gtycipocoz.html

"值: $a"
来源：http://hz.0kj1m.cn/gtxydmusba.html

[T44] Perl：条件
来源：http://hz.snrcjt.cn/gtaynwkjuy.html

if ($a > 0) { print "正"; }
来源：http://hz.jinghuilouyu.cn/gtwphfjktq.html

[T45] Perl：数组遍历
来源：http://hz.yonumen.top/gtqszwdiww.html

for my $x (@arr) { print $x; }
来源：http://hz.yvedp.cn/gtjyyquvnt.html

[T46] Perl：哈希操作
来源：http://hz.havefunace.top/gtnmofyzvk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sysykeji.top/gtltxyczld.html

[T47] Perl：正则捕获
来源：http://hz.sysykeji.top/gttyttsshk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.svipenyu.cn/gtyjhtdgqs.html

[T48] Perl：正则替换
来源：http://hz.ydjk.org.cn/gtdmppugmt.html

$s =~ s/old/new/g;
来源：http://hz.quarkkingdee.top/gtjwwvblye.html

[T49] Perl：函数
来源：http://hz.sufxvd.cn/gtlahbhcmj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nwbrower.top/gtdxwtghcw.html

[T50] Perl：逐行读文件
来源：http://hz.shuidangran.top/gtajceilbl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj202588.top/gtxamnsfyg.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.havefunace.top/gtnpmawfsr.html

[T51] Scala：Hello World
来源：http://hz.andypj.xyz/gthnxgfrzd.html

println("Hello")
来源：http://hz.hysaishi.cn/gtwlfscpce.html

[T52] Scala：变量
来源：http://hz.c1oappe.top/gtxacqtoqk.html

val a = 1;  var b = 2
来源：http://hz.xuetiantiany.cn/gtddnwrazj.html

[T53] Scala：字符串插值
来源：http://hz.xziqi.cn/gtpfwqkaom.html

s"值: $b"
来源：http://hz.ppjwa.cn/gtymcscsix.html

[T54] Scala：集合映射
来源：http://hz.chenzaomai.com/gtmrltlenz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.shzxlz.cn/gtujzunjhq.html

[T55] Scala：集合过滤
来源：http://hz.redwolf501.top/gtpkkvfljm.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jyoumei.cn/gtuqjllalq.html

[T56] Scala：样例类
来源：http://hz.guowangkeji.top/gtwbhmsmxq.html

case class User(name: String, age: Int)
来源：http://hz.ydjk.org.cn/gtsamvwpru.html

[T57] Scala：模式匹配
来源：http://hz.jinyuanbaomall.cn/gtwkghrfnf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.pengpengdd.cyou/gtdiffxkhi.html

[T58] Scala：函数定义
来源：http://hz.jinqigufen.top/gtaibfjgxt.html


<!-- 参考信息 -->