代发 wailian999

files=$(ls -1)
来源：http://hz.zhijiandao.cn/gtbonaeupl.html

[R38] 管道串联
来源：http://hz.hfpthk.cn/gtepsbtxeh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.havefunace.top/gtufuykbgs.html

[R39] 重定向标准输出与错误
来源：http://hz.shzxlz.cn/gtuhckzhhc.html

cmd > out.log 2>&1
来源：http://hz.jiagoushi.top/gtstjaamks.html

[R40] 追加写日志
来源：http://hz.xuetiantiany.cn/gtmgqsnqgj.html

echo "log" >> out.log
来源：http://hz.bjfxy.top/gtrxwhtore.html

[R41] 丢弃输出
来源：http://hz.zhiwuduotai.top/gtwnlbeizr.html

cmd >/dev/null 2>&1
来源：http://hz.nanxinkj.top/gtipqnzjzf.html

[R42] 输入重定向
来源：http://hz.yanxiufei.cn/gtohdnxrog.html

wc -l < a.txt
来源：http://hz.bjfxy.top/gtcehgbbjh.html

[R43] 按名字查找文件
来源：http://hz.ybcxt.top/gtlhzlqoql.html

find . -name "*.log" -type f
来源：http://hz.birdmap.top/gtxteiskzj.html

[R44] 按修改时间查找
来源：http://hz.sysykeji.top/gtsvuqojlu.html

find . -mtime -7 -type f
来源：http://hz.shangyingyoupin.top/gtiyuwuoiu.html

[R45] 批量删除
来源：http://hz.c1oappe.top/gtublhxeru.html

find . -name "*.tmp" -delete
来源：http://hz.daria6918.cn/gtaraielod.html

[R46] 递归替换文件内容
来源：http://hz.xingfuxueyuan.xyz/gtxlsklcnn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xylfe.cn/gtgevzjiex.html

[R47] sed 单行替换
来源：http://hz.hammf.cn/gtypifbgwm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xuetiantiany.cn/gtpoyessxy.html

[R48] awk 取指定列
来源：http://hz.chenzaomai.com/gterqldkgf.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258888.top/gtyhhlodmb.html

[R49] awk 带条件
来源：http://hz.yuanzhike.top/gtacdjxtdm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yueranfly.top/gtlbittvud.html

[R50] awk 求和
来源：http://hz.hfpthk.cn/gtibdcifqp.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinqigfzy.top/gtvdcyewor.html

[R51] 排序去重取前几
来源：http://hz.jyoumei.cn/gtbpruicbw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gogol.net.cn/gtnirnbwmv.html

[R52] 统计行数
来源：http://hz.aizwys.cn/gtcoceatmb.html

wc -l a.txt
来源：http://hz.shangyingyoupin.top/gtdikvtpxj.html

[R53] 查看文件头与实时尾
来源：http://hz.aizwys.cn/gtgmrzcfei.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenzaomai.com/gtdpjpdyjr.html

[R54] 比较两个文件
来源：http://hz.nanxinkj.top/gtbbpqokue.html

diff a.txt b.txt
来源：http://hz.cqqwz.cn/gtuthyvogr.html

[R55] 压缩与解压
来源：http://hz.daxiang520.top/gtnvemdsds.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jiagoushi.top/gttzpumuhx.html

[R56] 远程拷贝
来源：http://hz.zhongyouzk.top/gtodyowycs.html

scp file user@host:/path/
来源：http://hz.wangshuangyany.cn/gtkjwlbrob.html

[R57] 远程执行命令
来源：http://hz.jinghuilouyu.cn/gtkyhzfozm.html

ssh user@host 'uptime'
来源：http://hz.ppjwa.cn/gtvmoglvuv.html

[R58] 下载文件
来源：http://hz.shzxlz.cn/gtvhzuqqwm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.bjfxy.top/gtsmonajam.html

[R59] 发 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtbouipscc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.daria6918.cn/gtrhmworpj.html

[R60] 只看 HTTP 状态码
来源：http://hz.ydzc1.top/gtuoivpjor.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tianlin.xyz/gtlaeligpe.html

[R61] 磁盘占用
来源：http://hz.nwbrower.top/gtyyvvfjhb.html

df -h;  du -sh *
来源：http://hz.bjfxy.top/gtuhpusrjl.html

[R62] 找最占空间的文件
来源：http://hz.ydjk.org.cn/gtqcnkcmzf.html

du -ah . | sort -rh | head -10
来源：http://hz.guannengcc.top/gtxfgzftjl.html

[R63] 内存与进程
来源：http://hz.jqgufenzy.top/gtxqyahjsv.html

free -h;  ps aux | grep nginx
来源：http://hz.gogol.net.cn/gtmfktsscc.html

[R64] 结束进程
来源：http://hz.zhiwuduotai.top/gtzxevqtub.html

kill -9 $(pgrep -f app.py)
来源：http://hz.aibaodan.cn/gtxojnttwb.html

[R65] 查看端口占用
来源：http://hz.aibaodan.cn/gtyoahaoiv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhengqikj.top/gtkwqqgkmc.html

[R66] 定时任务
来源：http://hz.vqdsnc.cn/gtwpdilbfs.html

crontab -e;  crontab -l
来源：http://hz.yuxming.cn/gtqtkupnlr.html

[R67] 生成随机十六进制串
来源：http://hz.zhixingplan.top/gtirjreych.html

openssl rand -hex 16
来源：http://hz.jlsjyb.cn/gtdxpchufc.html

[R68] 计算文件校验值
来源：http://hz.gotoacloud.top/gthkzhgatr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.iojbl.cn/gtmxwltnau.html

[R69] 生成随机密码
来源：http://hz.shanyushiyangkeji.top/gtkorpqxfg.html

head -c 16 /dev/urandom | base64
来源：http://hz.daria6918.cn/gtbownhiuu.html

[R70] 时间戳与互转
来源：http://hz.jinyuanbaomall.cn/gtaiwaveqf.html

date +%s;  date -d @1700000000
来源：http://hz.zycfv.cn/gtldkdsjwe.html

[R71] 日期格式化
来源：http://hz.zhiwuduotai.top/gtnadujqud.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cheryme.top/gtpevewcgy.html

[R72] 等待端口就绪
来源：http://hz.gogol.net.cn/gtdfxvffxx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.tian-w.cn/gtkbhuiuso.html

[R73] 分割大日志
来源：http://hz.bjfxy.top/gtuouudhrs.html

split -l 1000 big.log part_
来源：http://hz.yj20258.top/gtzejrovoo.html

[R74] 批量重命名
来源：http://hz.hywenlv.cn/gtvtczfzks.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hfpthk.cn/gtsvxrnnzm.html

[R75] 导出环境变量
来源：http://hz.52xcode.cn/gtslfjyepk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.snrcjt.cn/gtecfowaft.html

[R76] 使用临时文件
来源：http://hz.yj20258.top/gtjuyclmzo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhiwuduotai.top/gtfjacmjgl.html

[R77] 读取用户输入
来源：http://hz.chenlongwang.top/gtvinehhzu.html

read -rp "请输入: " ans
来源：http://hz.cqqwz.cn/gtpghtvzwr.html

[R78] 交互式菜单
来源：http://hz.guowangkeji.top/gtjqwyaiqc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jqgfzy.top/gttknytwuh.html

[R79] 解析命令行选项
来源：http://hz.tianlin.xyz/gtmvweally.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.c1oappe.top/gtsjimtimx.html

[R80] 查看脚本执行耗时
来源：http://hz.jianghu66.top/gtkcztjcjx.html

time ./run.sh
来源：http://hz.zhijiandao.cn/gtenywhhkj.html

================================================================================
来源：http://hz.haohaochexian.top/gtxafhzxbk.html

S. C / C++ 专题
来源：http://hz.316326.xyz/gtxvdmmugo.html

================================================================================
来源：http://hz.guannengcc.top/gtbrsykayd.html

[S01] C：Hello World
来源：http://hz.jiagoushi.top/gttchjzshf.html

#include <stdio.h>
来源：http://hz.svipenyu.cn/gtmdhryufu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ydjk.org.cn/gtzzorslcg.html

[S02] C：变量与格式化输出
来源：http://hz.ydzc1.top/gtyrfqxbnp.html

int a = 10; printf("%d\n", a);
来源：http://hz.shangyingyoupin.top/gtlwkapozp.html

[S03] C：读入整数
来源：http://hz.birdmap.top/gtkvbrdegv.html

int x; scanf("%d", &x);
来源：http://hz.yongpay.top/gtgrdufiim.html

[S04] C：字符串复制
来源：http://hz.yanxiufei.cn/gtlcmubudz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jiagoushi.top/gtpeizlwgk.html

[S05] C：字符串长度
来源：http://hz.shuidangran.top/gtzlqzodch.html

strlen(s)
来源：http://hz.nanxinkj.top/gtybwniofq.html

[S06] C：字符串比较
来源：http://hz.sysykeji.top/gtjzytqhvp.html

strcmp(a, b) == 0
来源：http://hz.sysykeji.top/gtajwzmqhw.html

[S07] C：数组遍历求和
来源：http://hz.hnxiangtu.top/gtkzryskjq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sxryk.cn/gtbdkmuojm.html

[S08] C：动态内存分配与释放
来源：http://hz.chenjidiqi.icu/gtrhqyaccn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj202588.top/gtcymytiqu.html

[S09] C：结构体定义与初始化
来源：http://hz.jianghu66.top/gtmrxenyje.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.daxiang520.top/gtcfkhltso.html

[S10] C：指针与解引用
来源：http://hz.guowangkeji.top/gtnxuvenya.html

int *p = &a;  *p = 5;
来源：http://hz.sufxvd.cn/gtfvvzasyt.html

[S11] C：逐行读文件
来源：http://hz.hysaishi.cn/gtempetcjb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhongyouzk.top/gtlpwkeifl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinyuanbaomall.cn/gtgdjpdryi.html

fclose(f);
来源：http://hz.svipenyu.cn/gtxheppwsg.html

[S12] C：写文件
来源：http://hz.daria6918.cn/gtsdqmskzh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhiwuduotai.top/gtxnarxqpt.html

[S13] C：宏定义
来源：http://hz.meibo888.top/gtjoeqbvgt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jianghu66.top/gtmqmdbrkx.html

[S14] C：枚举
来源：http://hz.cucudq.cn/gtfjhslskb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.snrcjt.cn/gtsktquqyg.html

[S15] C：类型转换
来源：http://hz.hysaishi.cn/gtdvgnjxbd.html

(double) a / b
来源：http://hz.hysaishi.cn/gtyoqkyyln.html

[S16] C：位操作置位
来源：http://hz.jyoumei.cn/gtazvfypqg.html

x |= (1 << 3);
来源：http://hz.sysykeji.top/gtrfylgoma.html

[S17] C：安全拼接字符串
来源：http://hz.chenlongwang.top/gtfwviaaxf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.9152youxi.cn/gtvsqwsfok.html

[S18] C：命令行参数
来源：http://hz.jinqigfzy.top/gtcjqssidw.html

int main(int argc, char **argv)
来源：http://hz.gaohongyu789.top/gtjetcvxms.html

[S19] C：快速排序
来源：http://hz.zhixingplan.top/gtqxuzxttf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.dashuyun.cn/gtduvrbhmz.html

[S20] C：二分查找
来源：http://hz.havefunace.top/gtpmaojuvp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.feifeiyinyue.top/gtcxupitwe.html

[S21] C：字符类别判断
来源：http://hz.sysykeji.top/gtesdbrnzp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hfpthk.cn/gtnanbofiy.html

[S22] C：字符串转数字
来源：http://hz.hnqzz.top/gthwbgvili.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj20258888.top/gtklkrzyub.html

[S23] C：随机数
来源：http://hz.snrcjt.cn/gtqzyfbtcy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yongpay.top/gtkqnieunv.html

[S24] C：获取本地时间
来源：http://hz.shzxlz.cn/gtsueyaeex.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xingfuxueyuan.xyz/gtjskpyiyj.html

[S25] C：内存拷贝
来源：http://hz.xingfuxueyuan.xyz/gtkmeuragq.html

memcpy(dst, src, n);
来源：http://hz.chenjidiqi.icu/gtyryjvsyj.html

[S26] C：内存清零
来源：http://hz.jianghu66.top/gtjqtttbnc.html

memset(a, 0, sizeof a);
来源：http://hz.nwbrower.top/gtqfmfnvxf.html

[S27] C：定义常量
来源：http://hz.xziqi.cn/gtstvyudwd.html

const double PI = 3.14159;
来源：http://hz.c1oappe.top/gtgfkesabd.html

[S28] C：静态变量
来源：http://hz.hammf.cn/gtggkomfoh.html

static int counter = 0;
来源：http://hz.svipenyu.cn/gtssdvxyfx.html

[S29] C：变参函数
来源：http://hz.9152youxi.cn/gtupwzgbvn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.birdmap.top/gtagwwdmlk.html

[S30] C：头文件保护
来源：http://hz.sufxvd.cn/gtmbceauvz.html

#ifndef X_H
来源：http://hz.nanxinkj.top/gtsroflnmc.html

#define X_H
来源：http://hz.hammf.cn/gtcquaollp.html

#endif
来源：http://hz.yj20258.top/gtaxdoulfy.html

[S31] C++：Hello World
来源：http://hz.yueranfly.top/gtktvbwtxa.html

#include <iostream>
来源：http://hz.mhx1999.top/gtcyypdtpm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jlsjyb.cn/gtaxjhwbep.html

[S32] C++：字符串
来源：http://hz.iojbl.cn/gtarauosus.html

std::string s = "hi";  s += "!";
来源：http://hz.ydzc1.top/gtggqdxpte.html

[S33] C++：vector 增删
来源：http://hz.nwbrower.top/gtmqeqjrmu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jinqigfzy.top/gtkbefscww.html

[S34] C++：遍历 vector
来源：http://hz.shuidangran.top/gtmcmzjcpv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.kuanghao11.cn/gtztxrtqma.html

[S35] C++：map
来源：http://hz.yuxming.cn/gtvhemtdnv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.9152youxi.cn/gtngyjqodp.html

[S36] C++：unordered_map
来源：http://hz.jqgufenzy.top/gtjqotshkc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.mhx1999.top/gtmmnxrcxd.html

[S37] C++：set
来源：http://hz.xziqi.cn/gtqvizbsmv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydzc1.top/gtekunhimv.html

[S38] C++：排序
来源：http://hz.shzxlz.cn/gtdbsofcdq.html

std::sort(v.begin(), v.end());
来源：http://hz.yuanzhike.top/gtisenuqdc.html

[S39] C++：自定义比较器排序
来源：http://hz.jqgufenzy.top/gtqrvxqbar.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.mhx1999.top/gtqonwctca.html

[S40] C++：查找元素
来源：http://hz.jianghu66.top/gtrfoltxkf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xziqi.cn/gtiszetmcu.html

[S41] C++：类与构造函数
来源：http://hz.shanyushiyangkeji.top/gtavhdqnpd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hysaishi.cn/gteshnqgki.html

[S42] C++：继承与虚函数
来源：http://hz.aizwys.cn/gtsoxfcwju.html

class B : public Base { public: void f() override {} };
来源：http://hz.52xcode.cn/gtqcdhenxc.html

[S43] C++：智能指针
来源：http://hz.ydjk.org.cn/gtaqcqqvtt.html

auto p = std::make_unique<int>(5);
来源：http://hz.jianghu66.top/gtieziusgr.html

[S44] C++：引用传参
来源：http://hz.shangyingyoupin.top/gtjkfejwlg.html

void inc(int &x) { ++x; }
来源：http://hz.hfpthk.cn/gtrffktvzd.html

[S45] C++：lambda
来源：http://hz.aizwys.cn/gtzdfkdhlo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.haohaochexian.top/gtyiqdlklz.html

[S46] C++：函数模板
来源：http://hz.chenlongwang.top/gtbypxebrz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.guannengcc.top/gtntqaijla.html

[S47] C++：结构化绑定遍历
来源：http://hz.snrcjt.cn/gtkalrecvk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenzaomai.com/gtzlzwvbta.html

[S48] C++：逐行读文件
来源：http://hz.xuanzx.com/gtxnakuzzr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xuanzx.com/gttsjuyarb.html

while (std::getline(in, line)) { }
来源：http://hz.xinyue.icu/gtcalndfiy.html

[S49] C++：写文件
来源：http://hz.sysykeji.top/gtkfuwtift.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenjidiqi.icu/gtavnkvkad.html

[S50] C++：格式化数字
来源：http://hz.gaohongyu789.top/gtixzjoosr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258888.top/gtyzpgemar.html

[S51] C++：显式类型转换
来源：http://hz.daria6918.cn/gtkdeowecm.html

static_cast<double>(a) / b
来源：http://hz.jyoumei.cn/gtgskrnnth.html

[S52] C++：const 与 noexcept
来源：http://hz.ydzc1.top/gtyryexfsz.html

int size() const noexcept { return n_; }
来源：http://hz.chenlongwang.top/gtpszinfla.html

[S53] C++：移动语义
来源：http://hz.ywan-chungtsiang.top/gtazaxqzel.html

std::vector<int> w = std::move(v);
来源：http://hz.ywan-chungtsiang.top/gtclvtkunx.html

[S54] C++：异常处理
来源：http://hz.xylfe.cn/gtdomprqai.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhengqikj.top/gtxeemwpxi.html

[S55] C++：结构化绑定
来源：http://hz.smart0.xyz/gtpgupdmtl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jiagoushi.top/gtjvbjtjdq.html

[S56] C++：optional
来源：http://hz.hfpthk.cn/gtvjyxxcnh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gogol.net.cn/gtyypfubxi.html

[S57] C++：编译期常量
来源：http://hz.nanxuanxn.top/gtiskofiwl.html

constexpr int N = 10;
来源：http://hz.zycfv.cn/gtzzeipkiw.html

[S58] C++：命名空间
来源：http://hz.jinyuanbaomall.cn/gtnakwlzij.html

namespace ns { int f() { return 1; } }
来源：http://hz.haohaochexian.top/gtukufpqws.html

[S59] C++：静态断言
来源：http://hz.tanke756.top/gtfetrxpto.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj202588.top/gtcmbpptss.html

[S60] C++：遍历并删除元素
来源：http://hz.sxryk.cn/gtnkkktehr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jlsjyb.cn/gtuqyilbck.html

================================================================================
来源：http://hz.fzhhl.top/gtydbugrld.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sufxvd.cn/gtfhxjojbr.html

================================================================================
来源：http://hz.zhijiandao.cn/gtultfwnrh.html

[T01] Kotlin：Hello World
来源：http://hz.yangfankeji.com/gtkxbdgpnm.html

println("Hello")
来源：http://hz.zhengqikj.top/gtwzszcisr.html

[T02] Kotlin：变量
来源：http://hz.xuanzx.com/gtfwhcamof.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yj20258888.top/gtauwfjvdz.html

[T03] Kotlin：字符串模板
来源：http://hz.andypj.xyz/gtdemccsme.html

"值: $b"
来源：http://hz.mhx1999.top/gtxedchcvt.html

[T04] Kotlin：空安全
来源：http://hz.cucudq.cn/gtkgtcaiug.html

val n: String? = null;  n?.length
来源：http://hz.gogol.net.cn/gtmrhlzqjf.html

[T05] Kotlin：when 表达式
来源：http://hz.yj20258888.top/gtlainwxwe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.aibaodan.cn/gtvxnrswyb.html

[T06] Kotlin：集合映射
来源：http://hz.yangfankeji.com/gtrpoasgba.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.havefunace.top/gtxxetjgzn.html

[T07] Kotlin：集合过滤
来源：http://hz.chenlongwang.top/gttwrxngbe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.redwolf501.top/gtkpuilywr.html

[T08] Kotlin：数据类
来源：http://hz.yj20258888.top/gtqfxalbwr.html

data class User(val name: String, val age: Int)
来源：http://hz.ivvv.top/gtsjjmmaeg.html

[T09] Kotlin：扩展函数
来源：http://hz.guowangkeji.top/gtcdtsqgnq.html

fun String.exclaim() = this + "!"
来源：http://hz.xinyue.icu/gtxcxnvyri.html

[T10] Kotlin：默认参数
来源：http://hz.nanxuanxn.top/gtgwvoqera.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ydzc1.top/gtcmxmmqtv.html

[T11] Kotlin：协程
来源：http://hz.zycfv.cn/gtjpaalepc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.9152youxi.cn/gttgtjlymj.html

[T12] Kotlin：解构声明
来源：http://hz.yanxiufei.cn/gtimmgincg.html

val (a, b) = Pair(1, 2)
来源：http://hz.aibaodan.cn/gtimwqyowo.html

[T13] Kotlin：只读 Map
来源：http://hz.redwolf501.top/gtkzeygjcf.html

val m = mapOf("a" to 1)
来源：http://hz.bjfxy.top/gtnsllrgbw.html

[T14] Kotlin：循环
来源：http://hz.zhaomingkeji.xyz/gtytllefux.html

for (i in 1..10) println(i)
来源：http://hz.jinghuilouyu.cn/gtzrraymfq.html

[T15] Kotlin：接口
来源：http://hz.gogol.net.cn/gtzpbznmkq.html

interface Shape { fun area(): Double }
来源：http://hz.chenjidiqi.icu/gtektomvuk.html

[T16] Swift：Hello World
来源：http://hz.gzhubu.top/gtxkbmihat.html

print("Hello")
来源：http://hz.birdmap.top/gtodcskhzb.html

[T17] Swift：变量与常量
来源：http://hz.andypj.xyz/gtksugeaki.html

var a = 1;  let b = 2
来源：http://hz.xuanzx.com/gtsiyjvrlr.html

[T18] Swift：字符串插值
来源：http://hz.ydzc1.top/gtpovzlegd.html

"值: \(b)"
来源：http://hz.wangdashe.top/gtjanpysdw.html

[T19] Swift：可选绑定
来源：http://hz.jiagoushi.top/gthddqjdkc.html

if let n = opt { print(n) }
来源：http://hz.c1oappe.top/gtziwouofb.html

[T20] Swift：数组操作
来源：http://hz.shanyushiyangtech.top/gtfmdvauco.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gaohongyu789.top/gthncwxdaz.html

[T21] Swift：遍历
来源：http://hz.zhongyouzk.top/gthyggkwbj.html

for x in a { print(x) }
来源：http://hz.zhiwuduotai.top/gtredrchhd.html

[T22] Swift：字典
来源：http://hz.nanxinkj.top/gtfasbvulw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.nanxinkj.top/gtbpulxvfv.html

[T23] Swift：函数
来源：http://hz.haohaochexian.top/gtsmrinsyh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.andypj.xyz/gtfmjsgdmq.html

[T24] Swift：闭包
来源：http://hz.dianchejie.cn/gtvwzislbu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jqgufenzy.top/gtlvwilatk.html

[T25] Swift：结构体
来源：http://hz.hywenlv.cn/gtcaycjuka.html

struct P { var x: Int }
来源：http://hz.zhoulong.xyz/gtoqhobspo.html

[T26] Swift：类与重写
来源：http://hz.meibo888.top/gtrdtmsjlh.html

class A: Base { override func f() {} }
来源：http://hz.bjfxy.top/gtsdvaptep.html

[T27] Swift：错误处理
来源：http://hz.dashuyun.cn/gtfsurcdbp.html

do { try f() } catch { print(error) }
来源：http://hz.aibaodan.cn/gtpcyslqfh.html

[T28] Swift：枚举
来源：http://hz.guowangkeji.top/gtpsoeorok.html

enum Color { case red, green }
来源：http://hz.bjfxy.top/gtkmkstlpk.html

[T29] Swift：guard 提前返回
来源：http://hz.dianchejie.cn/gtojjampam.html

guard let x = opt else { return }
来源：http://hz.iojbl.cn/gtzknftpxx.html

[T30] Swift：协议
来源：http://hz.bjfxy.top/gtganyxzef.html

protocol Shape { func area() -> Double }
来源：http://hz.c1oappe.top/gtrsgisuvf.html

[T31] Lua：Hello World
来源：http://hz.daria6918.cn/gtqsmvrlhq.html

print("Hello")
来源：http://hz.52xcode.cn/gtfdjgscdf.html

[T32] Lua：局部变量
来源：http://hz.yueranfly.top/gtljtbjliy.html

local a = 1
来源：http://hz.zhoulong.xyz/gtgkzimxep.html

[T33] Lua：表（数组）
来源：http://hz.cashguo.top/gtstfolthm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yangfankeji.com/gtqypwkowj.html

[T34] Lua：遍历表
来源：http://hz.sweek.top/gtqrcmpvcs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.fengsongda.top/gtuncfzulh.html

[T35] Lua：字典表
来源：http://hz.wangdashe.top/gtrftvmyim.html

local d = { a = 1 };  d.b = 2
来源：http://hz.smart0.xyz/gthdbvexxw.html

[T36] Lua：函数
来源：http://hz.chenlongwang.top/gtwnldongl.html

function add(a, b) return a + b end
来源：http://hz.sweek.top/gtebdevtbd.html

[T37] Lua：字符串拼接
来源：http://hz.sxryk.cn/gtnkzxlmpk.html

"a" .. "b"
来源：http://hz.xingfuxueyuan.xyz/gtjalyewzz.html

[T38] Lua：条件
来源：http://hz.havefunace.top/gtfbanmagu.html

if x > 0 then print("正") end
来源：http://hz.nwbrower.top/gtbhxkvtvl.html

[T39] Lua：模式匹配
来源：http://hz.havefunace.top/gthhnglkrn.html

string.find(s, "%d+")
来源：http://hz.yueranfly.top/gtfhhdnzhs.html

[T40] Lua：元表
来源：http://hz.jqgfzy.top/gtofmdmbpp.html

setmetatable({}, { __index = base })
来源：http://hz.sysykeji.top/gtwktcmgjf.html


<!-- 参考信息 -->