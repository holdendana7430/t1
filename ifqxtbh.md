代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gixsxvapg.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnlikctnb.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqbgmihj.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsbsnfhd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/geektrsrh.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gzufyjknq.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqgyokul.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/geaxcjjhm.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhllzwwe.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gudmmdoqr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gmfhzdunq.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gzxrzvwtd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvsbsyby.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/guvcdjgzw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gdgbxqyen.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gsznutygi.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gonciiaoh.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxayibbl.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gkkqvbxis.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gwartbhsg.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfnbrjtj.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmbhkgca.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfluqimhd.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gqpmttmrn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gmacpsgpb.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gsbqexqvh.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gmzemtahc.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrrslvxw.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gjryykkmo.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoauvxcn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpulfgezh.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkqaowtz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/grhnzxqei.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfhvvsql.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqmtdklf.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gvecptlsp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gawuzeqgc.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gybemdrpe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gaocgsizj.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjtubpcx.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlnxcnut.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gduftubri.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxdhwmly.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gibrmoemf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gymqtfcet.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghceerzba.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gjvinxtcg.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwtcxziv.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmhpzyxa.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gctedcbyg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gziffilua.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/ghehlaqbp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuahdemt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrboavom.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/grvgnbksh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojtkhjzm.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrmoyxmg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnnyeehc.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gammebusj.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmghcgzi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmqeumowm.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gjzfjdsed.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoyarjjf.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gniqikbhy.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gjidnrlio.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjjujdgo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gphbzomcq.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhxjlhid.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gxqymuegb.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiienvcm.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gihhzaexl.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gjhpyzohd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gwftixqww.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvqbmicj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gansxrjnf.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gamwgwsjm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeukdkyx.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaqjcmqi.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/grmbvduux.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkztfbze.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gautqhwce.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gwwkszijd.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gomxcqrtz.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokixushn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkhjrlxk.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxieztmkd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/goroamomu.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/giovfhoah.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gwvczvklf.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gynvsygnv.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gtopeoymp.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbpfqqex.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gthcuvfhj.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/glyyqphzd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwuowaou.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gesvvovlm.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gcbbyitpi.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gaukaeekc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkidopsz.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqseaemb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gljtmlasl.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gqfehxywu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/giwsyybbf.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gainvgaps.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gztxkzmlz.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/grekuyblw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/giiborkyh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getmwbybo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glibyqzym.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvubilnk.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoyphhkh.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgafumpd.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvwvnnec.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gqbmqcntp.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqufvdwgv.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gabhxwryx.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglqwvwhb.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvugcitni.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/guquwbcfo.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxqeumhd.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gvvrlfpcv.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsfsjrlu.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gjrschrzl.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gtnuxttyk.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gymuzcdgj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlkzkzuy.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjorrrsnv.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gfbrqkghl.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gjojcyzbc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnaednsr.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsnwjost.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsqxswozw.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlukqqnb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjovnptsr.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gfkvugcez.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzxeolji.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gefiqutxp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtrurwrx.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gpmxdcjxe.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkinwmiaf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkujxdhi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gwhqvljwy.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzllrise.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwgrxzxq.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gompcfltr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gmjrmfhhl.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/guirxbomi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfqqlaba.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsgjpbcl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvitpsfsu.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaraocsf.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gupowlsrl.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gtymudjtq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gnghoafcc.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gfsnulzld.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gweybnhet.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcqxsoqz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gevgfweyu.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/goxutomch.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrtuexle.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gicxhfvbw.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gajfbfkmy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gakupufpw.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gnxnvqcea.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzledcsa.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmtyxtjs.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gansigeec.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gwgjuxpmr.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gadevbdam.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdvomjiw.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/guxgfegao.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gekqxseeb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojinzlgd.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gltcptlol.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/galjqhyxc.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/glunotvvb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpctdbyjb.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/goutkbtwf.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxstcvkvk.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrvshnfj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgcobajw.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gfplckwiw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/guuzqpyxf.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gqkerluvd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqvdjbro.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwusmucei.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfcxkaie.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiupjlwg.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxbujnid.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gsatezgft.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdacfkskg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gseackshz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjcftyqo.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvtqdeig.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaoujroz.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gssbtxwru.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsjmmbyv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/geazkcwpj.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnadfltv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/ghoriihvg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupnuoanj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjijzfxso.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdokjcoj.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwiakcht.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/geucpkomp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuxkptds.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxamgkle.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmzokust.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgjwatxp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftbugpdd.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhefxoqb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmojmlgn.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gckrrfckn.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gyoiovyjf.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqalyccc.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gokloojrm.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gwqnlswhk.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gupcgoavp.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsznihtxd.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/govgpqcqc.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmbiujeq.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpitxxka.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwmxytrt.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gzlrtgdcw.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gqcelxeuu.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzubqmdol.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/goectnolv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyryfkebl.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gylyzigfm.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutjnosbh.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gsmmgumsz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/ggrcqfpic.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmalpyjga.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gowciayla.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gtcrzetxe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gotdyftin.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszvbkooj.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gemjrilrh.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecpbxvcf.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfyefudc.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwprczvy.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gdstsrhza.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjjcqoyd.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzedqgass.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gskcfncxq.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtpgqblb.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyxvjlex.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gczoauuln.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gjljepcpj.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gfzzmopfm.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gptcxrmob.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gfrhibmjf.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gvvobhgmr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gczhujkng.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/grbdsgimm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpdtngjd.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffxhivnk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gcgcpzbwn.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaghjcpii.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwlqgabm.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gxdxsndqe.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/givtpiutz.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvntuefwt.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gaxbjqpmz.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/grvpxuqny.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/goaxviwoy.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhxknnoh.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/ggjugzkez.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gzsrdetmh.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gqwufrsqd.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gamoqheoi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gutwfvyaj.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdscmvjok.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfheudgfy.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoxppokr.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/grquqypxm.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/glgjgbjpv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaogsejb.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsqaqdxg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/guoterjtp.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfekytdk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjndapgj.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gqrpxinyp.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gzfxloxcl.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsngnsoy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gztbogtqw.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqozmqncr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbempxlee.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvqffxfq.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gezbffxpx.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gjxroqbke.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvrzwzvgz.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/guoiamjxi.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpfxyjot.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/grykkxeop.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gyzkfdbkw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzguspavu.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/glucsmyfy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrpkuowi.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/giufmmeug.sHtML


<!-- 参考信息 -->