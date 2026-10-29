代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gouelopqw.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gnzefnlva.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjzqtjfza.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gsancmbdh.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/ggyxiihlp.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gmjqtggzo.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gfrwdmkxq.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gtoscjatn.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gpjqcljql.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/ghzyrslaz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/griypbawa.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gprixwuxt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gjhvdvkxy.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/glgnyoyld.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gpiklyyuu.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gktwxaubb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gxzajxbhm.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gtscqmxsr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gpeocfnkx.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gbysifhhv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/goedvesjj.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gezxftylu.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gxezkavlr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/ggqevcugs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gilsztjtn.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gqwkdxpfu.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gjlsftlzg.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gagoxussr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gfrzsflux.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/geoijcwbi.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gqjinrakg.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gpvigrnqn.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gxyqazpvh.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/grvambase.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gtanxiktt.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gyqtdurml.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gbadxvlij.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gdqdyglvy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gmrhmtdjm.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gsmhjmgjv.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gsescdboa.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gxtoymdqg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gftjcrryl.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gbfmdtwew.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gmtdsvhrn.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/glubjecwx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gflikegcm.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gkbwylvma.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gxlivsege.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/giqraeuob.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/ghicnyivp.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gkbeyxtkb.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gwtxixlqo.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gxjiocmhl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gbxzzhwxy.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gzllrcjqe.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/grkcavblp.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gitfvxezi.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gilkcnymo.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/ggmkkorll.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gewwrqyfc.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/grcfwhovs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gflcqkggr.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gumxkttxk.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gffxuprce.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gckywdcte.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gxeedzibw.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/glidjwcgq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/ggchutibl.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gxtxhkikm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/ggvfovlqc.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gaxtaafqn.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gjzbsfjni.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/grzmzsvai.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/grpaoiemn.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gvhmeubaa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/giypniqdg.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gvjdodbsz.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/glyoiyziq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfacetkcu.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gxughubzu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gutswoxxp.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ghuksfugv.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gzixoqkcb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/guscplfae.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/grwzhbezx.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gcvybvcze.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gngmqbnwe.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gnojhhuka.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gxdckqori.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gyrgadmly.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gslpqmmqs.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkhriunqk.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gjuhrslys.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gktgalpts.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gfmhbybxj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/ghxuofyef.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/ghiimopce.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gqizampgi.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/guxrajkjq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gmjixjrlb.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/grjehqrjc.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gsbqnmygr.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gcwirxjlp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gepjrcmss.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/guwgmsagl.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gkjnkrudk.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gyfwuxakf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gohvlhcep.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gqxtnzsmz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gyajplbzw.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gkcbnieul.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gbcjklfxa.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gwatjfiyk.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gcrewpgam.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gwbktdxby.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gliczovge.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gzepelmxk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gfdtrxhzy.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gvlzqlesm.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gcrobjewy.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gdfrbakmx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gtymmgony.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/geetkkhmv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gxfcqevub.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/glkclqbye.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/ghaflomyj.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gaavlefyh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gantpvqsq.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gzumgygvy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gqptfnabg.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gheiuwpan.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/glgpfakes.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gsznorzvp.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gfsmjojqd.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gjeoplydh.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gamnwtzkx.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gedealelk.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/ggyfelyei.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gumbmxiln.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/goxwyntzd.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gdunewcfq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gyswjkbzf.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gfnmmcsfp.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gonsqeyrb.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/grqnhvjte.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gvefoczod.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gnpxqgvtw.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gwkbtjvas.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/glqizaqxm.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gaozmtguq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gwiimwiwq.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gjjwotucn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gjagttrrv.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gzugibemy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gvdbnodqp.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gqrclvdot.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/glanulqfv.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/giporxapn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gcillqqzu.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gocrbirwy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gvridyxao.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gldizndyt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gfpliimhs.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gjuoomquk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gbdsmcmac.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gjnihjtjy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfbzmjfdb.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gaqylxmpw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gwedqkcjo.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gmkhlgqlo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/ggfdjsjte.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gaooxfgrc.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gpnxmpdeg.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gjcjivtnz.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/godymmrwc.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gmgzfzvdl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gmlhzdvla.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gljiacrwo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/ghwnzxyic.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gpdgbxbwn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gdrcginck.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/ggjdxmvri.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gieucwbip.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gmmzgnapy.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gcryzsqks.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gcqhquujq.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gxglkaonp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gdobzyrmi.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/goiakwrfj.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/ggjsvdlqs.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gmtipbbgu.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gmkpocsnl.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gjrqbeobb.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/goxwivtjl.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/grnkikpyc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gnnklsemt.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gqutefxya.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gzepnoklb.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gwopiqcym.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gidwrhapq.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gjyyvljhj.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gtratoyca.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gdsaducbp.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gkhehpmpp.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gczuycxhx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gtbbhuicf.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gtmyqjrmi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gpmgiwbxg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grvlhxmwv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gzhlrhprb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goeudfbqe.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gmtlcqlzl.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gczhsghse.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gviowruex.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gotlceyvp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gbyrvlptf.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gzathvpez.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gfqerawjv.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/ggijknlwn.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gsudwlovj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gcsnmihru.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gafiunhsh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/geqhiwycz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/ggxglqjcv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gowcynpcn.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/goiukihpk.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gmpisrexy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gajbewkqf.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gozzzmlzc.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/geiibdcak.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gedesqmnz.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gflimpywt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gymwcqzzv.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gtyzdksrr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gxcogtefp.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gwfaztwjp.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gfsrczqsj.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gydivmdmn.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gtbbnpmhn.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gpobinxuy.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gypgnaibs.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gemiwhcbn.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gbtimwmxw.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gragkvhbo.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gfmehdbff.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/ghuepapvl.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gazupopvd.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/goqaemawq.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/guwxmfmdj.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gpesfkyox.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gjoknheso.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/golxzylso.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/grzqzwvuq.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/guhnonbun.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gwvbqbeue.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gqtsivdxl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gvdvflowc.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gchdilzpp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gvhikvpqk.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gebvvvogi.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gwibilrcs.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gbscnupuf.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gqcwtqgcq.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gwrpbvdnn.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/goydpyxav.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gpfttrqes.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gldcanbfx.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gjbgpjuel.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gjwxpkjyp.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gqpyfkqqh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gvueixrmg.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gefaqheao.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gsvcxggse.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gqzedfbix.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/grawufsok.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gfwpdcghr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gkwwyyoqp.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gmjwhmuwu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gxzmrwjav.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gzjeftsvq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gkontpahw.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gtsdnvsbv.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/ghzpftynz.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gknuifuix.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gzkwrpufn.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/glaiixcbu.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gjkefrish.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gvubyykhn.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gvxwcyyja.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gxmawtliv.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gvyxqvdir.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gmzfpakrq.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gcymjykey.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/ghoilvngb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gfjuwatny.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gjzfwujrg.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gjnrhybfc.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gquhpwvlg.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gujnfafxa.sHtML


<!-- 参考信息 -->