代发 wailian999

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/ghdhwessw.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gvzivlafj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gwbitindd.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gdeulyzsi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gxoegssbb.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gcyjgkkvi.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gxnawlhng.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gazynbjtf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gfzznxmou.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gabnmgaso.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gcdjqqtae.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gmlghgjzt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gyvyplcna.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gupeivhgd.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/ggycgwfzh.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gcjgxcxhp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gzftpgcfy.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/grkskesqn.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gtyovhsuh.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gsmqfttpj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gyqleadni.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gzoafpjzk.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gnwxcnsne.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/guwvjubgp.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gxyzlcjrs.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gudqgavdc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gikqtpspd.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gmkaotppv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gfqzwqaya.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gufdszfwn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/geqkwoxds.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gcepsnkbq.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gdwudzyge.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gtkfhtvnt.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gdwpjvaar.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/giemkcmji.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gcrhgszhz.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gfexkhtee.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gheskphzx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gwoctfacc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gtkfotabr.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/grmtgbhrg.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gzmeodoxl.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gevnglivo.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gnzwwslkn.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gayjhiday.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/grniszycl.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gwxvyxlcg.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gucyiwqyd.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gzzuyncpl.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gzgnrmcsn.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/geaxuwdtn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gpucctylx.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gozbitbxa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gskignnkw.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gvhbecoaw.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gexvfomzz.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gdnajoknm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gtojpdpim.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gxtfexzvc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gichqdthn.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gazwhefaw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gpbeslyjp.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gipraeumc.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gdfypfota.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/goxrvpukh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gpfgyyzay.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gxtfonbwt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gopjcradu.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gmxplexwb.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gwjqxcbpe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gakixgldu.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gkgxmcjfj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzdtaglqa.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gemxjbwkc.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gaaydppzf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gexfqxcqe.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gdwsikzai.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gbqwvykbb.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/ghocbngbw.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gvzkyhzmh.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gfvhrjsnm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gciwskdjr.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gcebzxszd.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gdjaodvrd.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gdsnlichd.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gltallnvv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/guvpplwmg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gghrvjnfl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gvcfteybh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gzlstluaa.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/glnxmcrub.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gapcyoawf.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/getyeujav.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gqlbpyelz.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gkivwdzzs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gfjhiegan.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gkxezxnam.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gkrfckkrm.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gjtnivmvt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gghhuwmso.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gaaftuguw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gmniregcc.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/ghkzmhmxj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gxdqwemid.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gwfojdxfo.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gtqqwulxr.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gicjmdifu.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gmcdmxumf.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gkqrwwnlm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gvtadnytl.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/ggmarrjep.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gvfbnqark.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gfvmzliwy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gymhrthxj.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gyjgzafro.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gqzinmqjz.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gnbuitwlf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gruagwrwt.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/ggggbjirz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gcslsduuw.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gnastpqfr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gmzlugyvb.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gsoxradlm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gcpqihxqb.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gmwhmyhwb.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gcailherw.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gnmclkzhp.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gqxvmakbi.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gmeasbbiq.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gnvrunsul.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gkjntbenn.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/guqojmxok.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gdnqnflrr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gaceqkqfc.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gouynbjzl.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gxvdxmmos.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/ghnkzsgpr.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gsydzfngr.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gmhulucrg.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gvtzvfrrk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gorbozkss.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gjsjimaxt.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/garaxfxqc.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/geourczig.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/giaqffozj.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gfdxrrjee.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/ggnoyxtrg.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gjfejnvux.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/geburuewa.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gtqduqvdv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gloxkczja.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/grnjxovau.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gmsdajfur.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/ggmuswsvo.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gqusulsde.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gpkiwfgcq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gbonrpgqu.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gtejcssai.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gbvudrlmz.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gkiovqkwz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gmopshevy.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gcoigeuvm.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gvmxeazwf.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gctfrmcrx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/goxpucseq.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gctfazavq.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gdgqzwjfe.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gfahkewfb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gurionfcz.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gkogosjzf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gijezcylj.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gdsmpkoin.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gamcpygnq.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gkwhwnpaq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gcmczbajm.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/ghuzmraqs.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/ghibllqce.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gdtmsyxry.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gbtgvoxgo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/geqnkovfe.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gumqjhnuv.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gghfystnq.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gjsldehrr.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/grepqngxu.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gejiafnic.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gftpyxmyh.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gupdzdkvt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gszvqhrhm.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gyfqfnuud.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/giihgfxpz.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gopwlenry.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gvaqjcjzb.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gwwssllcl.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gqjpdlsgt.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/giysxhmmc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/ghzrxfgur.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gqpdbrtil.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gskyfkycs.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gqjyliqlf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/grlcdnrvb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsdktihgw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gibkcwoab.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghdmuduvz.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/giqmdfprt.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gfjfwkydx.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gstjgcanh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gyqhoklnr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gpdqpketg.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/grrhbumxt.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gwfvkapvr.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gegrodnge.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gxpyizgkd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gqjysnhom.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gtjejqewh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gxiaruujf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/ggjqcmfaq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gfekqmhzm.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gwfryqzpf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gdbbysqib.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gispbnonj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gsnwqkspg.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gylwkckyp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gzruuhpjc.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gvactwdmi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/guqugurkr.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gfebaoots.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gwjxgwvco.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/godqnkoth.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/giyijjcmk.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gohonaimt.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gwwqcwjyu.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gwubmjhdj.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gcuvurolw.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gibduldds.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gvjqzqali.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gqgjawkna.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gpppbmnlm.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gusjadybv.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/ghjmjxjte.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gxbkahrav.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gpilryuif.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gcfgyivzp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gngxfvecn.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gsnhckmgr.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gquleuwkj.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gqquvulev.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gxlyagzoh.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gfcwcocgs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gmkipvysa.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gecwtvver.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gweklytiw.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gmwyjremm.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/ghavjbobg.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/glxyyxpde.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gqlbmopvi.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/geqcbudwz.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gjmpwplqd.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gketfotup.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gdvymkfvx.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/ggtavhjiz.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gmbexkavm.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gmzqrdbwr.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gtbzcgxbc.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gohxqequb.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gxyyzxdyi.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gnidrrlwa.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gexzzpkmk.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gjbtjoalp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/geuzamwoh.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/grdgolwik.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gukbqhpca.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/ggzyhlvhr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gxsgurirg.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gmgxvjukz.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gyzfkglgk.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gxazkyujc.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gbhzpmrxz.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gjcdwahba.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gpeagqkox.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gkadaqsgi.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gbgjlglsa.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gsvrganlc.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gechxnksc.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ggyqomave.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gfgynmdmn.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gpcgoveei.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gklkzmmtz.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gavhojufk.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/glattqfno.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gvkniagsg.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gyshxjtfe.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gkzbynamx.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gyyodvbfd.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gmtxnfolt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gtycqsqoo.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gvmvfvcal.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gycusqapw.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gyzzxukka.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/goixbajag.sHtML


<!-- 参考信息 -->