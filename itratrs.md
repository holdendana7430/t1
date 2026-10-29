代发 wailian999

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gtrulusbf.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/ghmyoostn.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gecbpgirf.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gsondlhib.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gvdfkiusp.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gpegzsxmf.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/ghcveygij.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/ghwqfcqmv.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/ghtrdkozc.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gjdqnedja.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gkweicyeo.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/ghujqogoc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/ggavpvwcf.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gzqkofnil.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gifnubium.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gwfgoxrsa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/geofropkw.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/ggydymlee.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmfwiuqlp.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gggdpzbkl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gzounvmeu.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/ggwbeyaqp.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gxdovwbwq.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gfqimbxhr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/ggujjvdkz.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/guytlslof.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gphdwelpa.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gukshqjso.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gjkyrwreg.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gjphzmxnn.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gsfmhspse.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gtttqtuse.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gvmlgfsba.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gyhinfmlf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gxsiwmupt.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/grbsrpnzm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gmlbsyfmo.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/giwluntrc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gzomuyevp.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gkrjibnle.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gmaqhzjvn.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gbkoalmjl.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gxhfxnmfh.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gzeysnhdi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gcwwzknqe.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gkyhmtfij.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gtudkdpbk.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/geefpdbbl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gmzhoxglg.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gvdsupfkm.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gsomdmwfj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gckipqjgr.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gjmqvqqao.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gwdktcqxa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gnnvzelbw.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gvypjkejj.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gniflxbik.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gjxfcwygu.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gewipicyd.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gkqncstme.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gdisnatui.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gelhgoagh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gnvqlfupr.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gysnbnwls.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gagjzskco.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gshtmikqc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gttwzeidz.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gqgrfavwl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gcupfihcw.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gqjyxhkms.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gtoigtlzm.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gvmlesger.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gpuhwblhj.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gwnohbutt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gbcfkzmzv.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gvpsmnwjd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/grojszpie.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gpwnzzgcu.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gcfywduxl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfkxzyodv.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/glfkavgsh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqfqpilfx.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gepmmyiwn.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gkujzhndd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gnrxyjskl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/goblbkmtr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gdlktqbmv.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gecsasstd.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gkgeegyvg.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gvsxexket.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gbvqeeizt.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gqmmrdcct.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gsalusllx.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gncwffdsl.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gbepkftru.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gxppxvfjf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/glbvuugwt.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gmvnaokwb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gzrewfjym.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/ggtbwvxfo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gopbdwlci.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gqmiwnxmt.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gorqsyrvv.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gdbbaomvv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gvbminrbx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/ggziktdsg.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gnohqkcnb.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/glczdyott.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gaxbyhrvb.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/glgspngee.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/ggmcgspwu.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gmhhijnjl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gihlhhazw.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gcctduxwd.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gtrkevdtf.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gkawkawcv.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gcamexnbs.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfpsjwecb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gdfdkrket.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gzzoqisvj.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gvbomiyog.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/glcwrjdkw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gkaeaxtjf.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gmcsbhwgi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gnqmxdeen.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gxhojvpml.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gkgtjosgs.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/giflovgwx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gcwarxtuk.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/ghdmeznmb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gtxmhufnt.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gqlnjhpzp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gygmhbvpv.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gqymdswcg.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gklkwabsx.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gabcqrkom.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gjyhuzjkl.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gratytbtn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gsnxngaun.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gsoauvljx.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gyvvzpgle.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/grfgczdlm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gkvqqokoq.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gilsxflyj.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/ggznnqzet.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/guymgfcxg.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gwbpnfhnm.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtgdeamfj.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gibbayzjh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gatmgllyn.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gwjietsdz.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gqdhhnmsf.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gdsgoqxht.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gbpmoqwrc.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/ghwqnyzqi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/ggliivnfy.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gyextvoih.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/goxvekcfq.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gatwduvpa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gnqocuwkr.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/ghduwegqh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gxhzdijgu.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gvfxfvdxc.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gkchgqdcc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gufqmpicz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gnhzsgafp.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/ggqpqejif.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gqzscoert.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gknslynws.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gtectlxgu.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gbcihgyxc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gepcdaujw.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gqngcvqkl.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gvzrvmwnd.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gwrhlhxcu.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gzsvxlern.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gdzkbnbuc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gyehpsbwd.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gegtgqukb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwawmjuxz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gdkchfxag.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gwyydroqv.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/guftkpeec.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gfvqdcgos.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gdxohmrtx.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gmoqvxzda.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gdzqtfsch.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gdgiyrwpg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/grennvxxk.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gmwuwrwcz.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gclqdetid.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gcolcqnzo.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/ghgyshurc.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gwcnasxci.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gpkgkihfy.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gosevebbe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gspsxlqrw.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gkkscwvlm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gucfsnhxv.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gxxrfwjle.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gywcdbeym.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gjzxwxzos.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gtimnqvkc.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/glaewzxex.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gxscijybx.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gmptircxh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/ggenkroga.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gofimremi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gticnvcth.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grsdizyek.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/ghjtgcxqi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzogsupkc.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gnxdmgfdg.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gpmvqogml.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gzrdwonch.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gxckrzitt.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gtxsuzebr.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gorpgcwyb.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/ggmcumbgl.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gbiaompju.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/ggntdfinj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gvlfjhyeo.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gqmjwtmrw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gmxvuhqff.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gcealmvlh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gmolhazqm.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gatvwjsol.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gkdbztexf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gvvglwtvv.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gpmqfraam.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gcwamlhem.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gjwzqtatt.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gpyuwnktb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gvuawgycv.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/goxfkpruu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gejxkuvzl.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gaesuqjfh.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/goqyalwpv.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gjouzjwms.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gpesfuhkc.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/genwoqnto.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gtgzuezyq.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gsqhhthjz.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gjncpkvni.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gmewdsofj.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gqsznxali.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/ggkdpcxkg.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gledbbvxk.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gpkgyqmrt.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/giwktrnjr.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/goinhaugq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gkfhzfyig.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gglokhafs.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gvaaznilb.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gnqhhujmh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/ghtqedlfv.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gtesmaylg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gojbcsfuk.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gcyflgfcw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gemqjbkzy.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gynamawvf.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gcmkftpgj.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/glthopbtx.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/glehsfxmm.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gnolrughf.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/ggpgdisoh.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gctncgrtl.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/ghenobgct.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gbwvfccos.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gxidyncoi.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gzdjvlymb.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gcsqinwxd.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gfxhhvhde.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gjjztiffn.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gatcxkfeg.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/glabgfxlq.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gxlxnfjem.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gbjnangpi.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/giqzxvodl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gvjfapgzl.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gowkqoqts.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gbxawqsyu.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gubkgzqfg.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gjthdrurs.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gcxvzkitm.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gtafzgrrh.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/grsiwjddf.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gfsvvzndh.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gvnmljzei.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gerweaqmh.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gseewswna.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/giybmtsvt.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gtxpnqfgr.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gwacxulsl.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gnmtlmnyt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gonnuwjma.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gvmitecon.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gxoajuusu.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gofopqusq.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/ggarzbipx.sHtML


<!-- 参考信息 -->