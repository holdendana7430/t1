代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gdscwisds.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcozgxcua.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmqwthvrm.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gyxmkvaki.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gpopqxhpv.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyiyhxfh.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/geucppxov.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gahzierwu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfswcbba.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafayyjjr.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/giyenrqpn.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gmaigvxja.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtqrdzqd.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqcdjrea.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/guciexjug.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuknqkfj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gghthengx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gegvdjruc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsjcdhgd.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjplykqqm.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcusgbvkf.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gohkxsymz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giytqrevo.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqdyvtxy.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gdakeunay.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkseivkaw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbvmzjqz.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gklrvscob.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnichgfcv.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/grasjtqbq.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gzxeiadeh.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gwefarclt.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gblhcjqqk.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzkmdepa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzusqenib.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/goqsqzkeo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/grywgqhbb.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gpmemrtsv.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuqhonmz.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gevxakgyo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gwrlhgrwo.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/goqlzgibp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnisczmjw.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdehjwjm.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gciphudbz.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwwrlgwb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzthimfjo.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuidnjlo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gpbfbyzcy.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/giffgzbpw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gipbffrlp.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/goofsyesg.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gehcqzznr.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/grpuevxgp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gakkfotuy.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gsgohnbeh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gitlgxfex.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/goojlsmps.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gossmryun.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwbhoyzi.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gaioyvezp.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxriwscbt.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grgbpqhef.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsesuffi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdqqpmfqm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/guyytrstk.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gsleuvcud.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusunxscy.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goojbouuf.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gggkezfhc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gaxbkrvpx.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ghymwsbhy.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gtyadtnzu.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/guweevpmh.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/grntgjysu.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gzebdybin.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gebjbltrh.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gwmgmpecr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giurjyxlp.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gnkymxsri.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/grilgzjuj.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/glmsvdxch.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwsszsry.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggqjhwlof.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfyahxkk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmlwoagl.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiunyhuc.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqkmsfumq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwwighgc.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcclyupgh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzimnaty.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gfjwwbeah.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcbwluuu.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gxmmvyuhm.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gsipggcin.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/ginxqpgnh.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxckevhaa.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gauxmksvu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzdldpej.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/glxkpktxx.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvhqcgvg.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjfwjibu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbvtoecz.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyasotfzo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gbrbmvrwk.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gqdxeajis.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlwvqrxj.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/ghhqoiabv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggekigjap.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzagejvji.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtupcjhkf.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gphgndnay.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gvxjffgfv.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/geiwkgmex.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvumkoga.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrsbtgvb.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgasrmpj.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggipvvmsi.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoejqqcv.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxptkugum.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gptdfhaah.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grgwfdfld.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gpnbksjho.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpbphnub.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gnfbodrae.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gwhytlhkz.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/guayadhbj.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuyyvilg.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gibmjfvmx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvwtzcie.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gajscphdn.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvreshsws.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/glpwjxkwe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grifnsotd.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqinpxpmv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfyqmnxy.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gohyqgyby.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcqsftpj.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gvwpjtmbh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/galnngbub.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gihhlklsz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtdvfqbd.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvpbykryl.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbgtmmnq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gghkvkolt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/grktcsoky.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gesoxgwms.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/galummyrx.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgmrjkcj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gfsvbshjn.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvizvteqh.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gyjjlhfbk.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimqncutu.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gszznwaxd.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhswwgkb.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/genjyucgn.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcsanhhh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjhpmwnx.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gijaelcoo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggtbfgmkn.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/guvpubkko.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsiysqnf.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giglfbfkd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gthnxgyde.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnporlsa.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxyyfnoe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gkjspsvat.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gugirvpzi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksvrdcjk.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdbqtjbo.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpqpntob.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiyrofgv.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmvoptgiu.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbksnwbt.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gbcddsxki.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/grpettaqj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdricbpkr.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxrkbogk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfrwsdwp.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvgzdcak.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gudkdevky.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmivwutsd.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gfxawyoxz.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/groznaztg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/giqgrmvbe.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/ggokcbsrk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkvkuaku.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/grlmdbyhz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gvedvqssc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyxcdvms.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggocwfznt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/govgblqyr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsrgzxrhx.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gyqosvdbv.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/glrmcekix.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcnfcybu.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gznvzwvaj.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gedvnzrrj.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdjkphvg.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/ghssisllz.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/guxfzlija.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gxkmcbgmo.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/giqufpskl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtzobwpz.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/ghxikiagc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuvmuflq.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gijvounpn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuklcrjt.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gftofihhq.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gipnuegrm.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfghxypec.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gucbiqgyl.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/grvlwzugw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/grzgeycsd.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdddwhqu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnykgpkwh.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gvbgkgfqz.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/geromlfpn.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxqmjpwq.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvphepxz.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gwdfgyvxk.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlkqaetg.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdgxueqbp.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwxznbyq.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadkeudwa.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gjzzvzidq.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/givzgxibq.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwtbjgwn.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcrjmhqy.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gcuvabtqs.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzfiuokf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gouzlifuk.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gxisoyull.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gbafeyhfd.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/grdqdtguc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfihsisgt.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthydtxlb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfzwbtfe.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjtlgtih.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrxfjtue.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gjigfeier.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnndkzkv.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gwtdcezhu.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gpagbgrdi.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gikgogegq.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrevqqqr.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/glylbbatq.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gueftdqgj.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdwvkmjz.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gqusiharr.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gngebriro.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxjanbhl.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbhrihqw.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gdhtjpbxj.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/giqpgabmd.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/glqlqhzhp.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/glinpkzje.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gegyoqkoh.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqcmbafl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gztsyosvj.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gtqyztcgm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gmgbxiwkd.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grlasbqcn.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gchpryxuz.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtneoanhi.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjblbumtu.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gyscaefoz.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/getblqlvk.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gotlkljub.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gnsjytpbe.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoegymdl.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gkcrgakha.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxdxepec.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gznloesjp.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gateffwjz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgrkwcrv.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gqtpatfxr.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gckmerxog.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfznyzte.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzyzfkwf.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gcbgntict.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtcjlkqz.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/guvwslcrh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzskzbsut.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gvzqtxhxa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpldfrzvt.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdurzwnc.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gubokqtrv.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gflavosoa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gijuxoodz.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxogcalke.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkrwhjzu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfilxcrbu.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxlrbdcm.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gzdgygzol.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmpvlqgh.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdjxlmjv.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqfszynj.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpdcyjro.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gtirkjhgr.sHtML


<!-- 参考信息 -->